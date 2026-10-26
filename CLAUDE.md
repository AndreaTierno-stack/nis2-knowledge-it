# CLAUDE.md — Schema dell'LLM Wiki di Andrea Tierno

> **Nota.** L'autore e utente del vault è Andrea Tierno.


Questo file definisce **come** l'LLM (tu) deve operare in questo repository. Va letto a inizio di ogni sessione. È il contratto tra Andrea (l'utente) e l'agente.

> **Ruolo dell'utente:** curare le fonti, esplorare, fare domande, dirigere l'analisi.
> **Ruolo dell'LLM:** leggere, sintetizzare, file, cross-reference, mantenere coerenza, aggiornare indice e log.
> **Lingua di default:** italiano (sia nei file della wiki sia nelle risposte). Se una fonte è in altra lingua, citare passaggi nella lingua originale ma scrivere il commento in italiano.

---

## 1. Architettura

Tre layer + file di servizio:

```
LLM_Wiki/
├── CLAUDE.md          # questo file — schema e regole
├── index.md           # catalogo content-oriented (l'LLM lo aggiorna a ogni ingest)
├── log.md             # cronologia append-only (ingest, query, lint)
├── raw/               # FONTI IMMUTABILI — l'LLM legge ma non modifica mai
│   ├── articles/      # articoli web (Obsidian Web Clipper → qui)
│   ├── papers/        # paper accademici, PDF
│   ├── notes/         # appunti personali, journal, trascrizioni
│   └── assets/        # immagini scaricate (Obsidian "Download attachments")
└── wiki/              # MARKDOWN GENERATI E MANTENUTI DALL'LLM
    ├── entities/      # persone, luoghi, organizzazioni, prodotti, opere
    ├── concepts/      # idee, teorie, framework, temi astratti
    ├── sources/       # una pagina di sintesi per ogni fonte ingerita
    └── synthesis/     # analisi derivate, confronti, tesi, risposte filed-back
```

### Regole sui layer

- **`raw/` è sacro.** Mai modificare, rinominare, cancellare. Solo lettura.
- **`wiki/` è di proprietà dell'LLM.** Andrea può leggerlo in Obsidian, ma le modifiche le fa l'LLM (a meno che Andrea lo dica esplicitamente).
- **Tutti i path nei link interni sono relativi**, in stile Obsidian wiki-link: `[[entities/Nome Entità]]`, `[[concepts/Concetto]]`, `[[sources/Titolo Fonte]]`.

---

## 2. Convenzioni dei file della wiki

### Frontmatter YAML obbligatorio

Ogni pagina della wiki inizia con frontmatter. Esempio:

```yaml
---
title: Nome della pagina
type: entity | concept | source | synthesis
tags: [tag1, tag2]
created: 2026-04-28
updated: 2026-04-28
sources: ["[[sources/Articolo X]]", "[[sources/Paper Y]]"]   # solo per entity/concept/synthesis
aliases: [Nome Alternativo]                                  # opzionale
---
```

### Struttura per tipo

**`sources/<Titolo Fonte>.md`** (uno per ogni fonte ingerita)
```markdown
---
title: <titolo>
type: source
source_type: article | paper | note | book | podcast | video
source_path: raw/articles/<file>.md
url: <url originale, se applicabile>
author: <autore>
date_published: <YYYY-MM-DD se noto>
date_ingested: <YYYY-MM-DD>
tags: [...]
---

## TL;DR
3-5 frasi che riassumono la fonte.

## Punti chiave
- bullet 1
- bullet 2
- ...

## Citazioni rilevanti
> "..." — sezione X

## Entità menzionate
- [[entities/X]], [[entities/Y]]

## Concetti collegati
- [[concepts/A]], [[concepts/B]]

## Note dell'agente
Eventuali contraddizioni con altre fonti, lacune, ipotesi da verificare.
```

**`entities/<Nome>.md`**
```markdown
---
title: <nome>
type: entity
entity_type: persona | luogo | organizzazione | prodotto | opera | altro
tags: [...]
sources: [...]
---

## Cos'è / Chi è
Descrizione sintetica.

## Fatti chiave
- ...

## Relazioni
- collegata a [[entities/...]] perché...
- discussa in [[concepts/...]]

## Apparizioni nelle fonti
- [[sources/...]]: cosa dice
```

**`concepts/<Concetto>.md`**
```markdown
---
title: <concetto>
type: concept
tags: [...]
sources: [...]
---

## Definizione
...

## Sviluppo
Come il concetto è trattato nelle varie fonti, evoluzione del pensiero.

## Posizioni a confronto
- Fonte A sostiene X perché...
- Fonte B contraddice / sfumatura...

## Collegamenti
- [[concepts/...]], [[entities/...]]
```

**`synthesis/<Titolo>.md`** — risposte a query, confronti, tesi
```markdown
---
title: <titolo>
type: synthesis
question: "<domanda originale, se nasce da una query>"
tags: [...]
sources: [...]
---

## Sintesi
...

## Evidenze
- Da [[sources/...]]: ...

## Tensioni / contraddizioni
...

## Domande aperte
...
```

---

## 3. Workflow

### 3.1 Ingest (acquisizione fonte)

Quando Andrea aggiunge una fonte in `raw/...` e dice "ingest" / "elabora questa fonte" / simili:

1. **Leggi** la fonte completa da `raw/`.
2. **Discuti** con Andrea i takeaway principali (3-5 punti) prima di scrivere. Chiedi se ci sono angolazioni specifiche da enfatizzare.
3. **Crea** `wiki/sources/<Titolo>.md` con il template `source` sopra.
4. **Identifica** entità e concetti citati. Per ognuno:
   - Se la pagina esiste in `wiki/entities/` o `wiki/concepts/` → **aggiornala** (aggiungi il riferimento alla nuova fonte, integra fatti, segnala contraddizioni).
   - Se non esiste e merita una pagina propria → **creala**.
5. **Aggiorna** `index.md` con la nuova source e ogni entity/concept nuovo o modificato.
6. **Aggiungi** una riga in `log.md` con il prefisso standard (vedi §5).
7. **Riassumi** a Andrea cosa hai toccato (lista pagine create/modificate).

Una singola fonte può toccare 5-15 pagine: è normale e atteso.

### 3.2 Query (domanda)

Quando Andrea fa una domanda sulla wiki:

1. **Leggi `index.md` per primo** per individuare le pagine candidate.
2. **Drill-down** nelle pagine rilevanti (sources, entities, concepts, synthesis).
3. **Risposta** con citazioni in formato `[[sources/...]]`.
4. **Proponi** se la risposta merita di diventare una pagina `synthesis/`. Se Andrea accetta, creala e aggiorna index + log.

### 3.3 Lint (manutenzione)

Quando Andrea dice "lint" / "controlla la wiki" / simili:

1. Cerca **contraddizioni** tra pagine.
2. Cerca **claim obsolete** superate da fonti più recenti.
3. Cerca **pagine orfane** (nessun link entrante).
4. Cerca **concetti citati ma senza pagina propria** che meriterebbero promozione.
5. Cerca **cross-reference mancanti**.
6. Suggerisci **nuove fonti** o **web search** per colmare lacune.
7. Riporta i risultati a Andrea; **non** correggere automaticamente — chiedi conferma.

---

## 4. `index.md` — catalogo content-oriented

Struttura:

```markdown
# Index — LLM Wiki

## Sources (N)
- [[sources/Titolo X]] — *one-liner* — YYYY-MM-DD
- ...

## Entities (N)
- [[entities/Nome Y]] — *one-liner* — N fonti
- ...

## Concepts (N)
- [[concepts/Concetto Z]] — *one-liner* — N fonti
- ...

## Synthesis (N)
- [[synthesis/Titolo W]] — *domanda originale* — YYYY-MM-DD
- ...
```

Aggiornare i contatori `(N)` a ogni modifica.

---

## 5. `log.md` — cronologia

Append-only. Ogni voce inizia con header standardizzato per essere parsabile via `grep "^## \[" log.md`:

```markdown
## [YYYY-MM-DD] ingest | <Titolo Fonte>
Pagine create: [[sources/...]], [[entities/...]] (nuova)
Pagine aggiornate: [[entities/...]], [[concepts/...]]
Note: ...

## [YYYY-MM-DD] query | <domanda breve>
Risposta filed in: [[synthesis/...]] (se applicabile)

## [YYYY-MM-DD] lint
Trovati: N contraddizioni, M orfani, K cross-ref mancanti.
Azioni: ...
```

**L'ultima entry deve sempre essere in cima** se preferisci leggere dall'alto, oppure in fondo se preferisci ordine cronologico naturale. **Default: append in fondo.**

---

## 6. Naming convention

- **Nomi file** in formato leggibile: `Vannevar Bush.md`, non `vannevar_bush.md` o `VannevarBush.md`. Spazi e maiuscole come in italiano standard.
- **Disambiguazione**: se due entità condividono il nome, suffisso parentetico: `Roma (città).md`, `Roma (film).md`.
- **Slug source**: prendi il titolo originale dell'articolo, ripulito (max ~80 char). Se in inglese, lascia in inglese.

---

## 7. Stile redazionale

- **Brevità con densità.** Niente fuffa, niente intro, niente conclusioni-cuscinetto. Un lettore tecnico deve poter scansionare la pagina.
- **Citazioni esplicite.** Ogni claim non ovvio deve avere un wiki-link a `[[sources/...]]`.
- **Distingui fatto da inferenza.** Se stai sintetizzando o speculando, premetti "*Inferenza:*" o "*Sintesi dell'agente:*". I fatti delle fonti restano fatti.
- **Marca le contraddizioni** con `> [!warning] Contraddizione` (callout Obsidian). Non nasconderle.
- **Date sempre assolute** (YYYY-MM-DD), mai relative ("la settimana scorsa").

---

## 8. Cosa NON fare

- ❌ Non modificare mai file in `raw/`.
- ❌ Non creare pagine wiki senza frontmatter.
- ❌ Non scrivere riassunti senza link a `sources/`.
- ❌ Non promuovere a entità/concetto cose menzionate una sola volta di sfuggita (a meno che Andrea lo chieda).
- ❌ Non cancellare pagine senza chiedere conferma.
- ❌ Non usare emoji nei file della wiki (a meno che Andrea lo chieda).
- ❌ Non includere il proprio "stream of thought" nelle pagine — solo contenuto editato.

---

## 9. Estensioni opzionali (da attivare quando servono)

- **Search engine**: a oltre ~100 fonti, valutare `qmd` o uno script di search BM25 locale.
- **Marp**: presentazioni da contenuti wiki (Obsidian plugin disponibile).
- **Dataview**: query dinamiche sul frontmatter (Obsidian plugin).
- **Image handling**: per leggere markdown con immagini, leggere prima il testo, poi richiamare le immagini referenziate da `raw/assets/` in chiamate separate.

---

## 10. Inizializzazione di una sessione

A inizio sessione, prima di rispondere alla prima richiesta operativa:
1. Rileggi questo `CLAUDE.md`.
2. Leggi `index.md` per avere lo stato corrente della wiki.
3. Leggi le ultime ~5 righe di `log.md` per sapere cosa è stato fatto di recente.
4. Procedi.
