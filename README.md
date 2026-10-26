# nis2-knowledge-it

Knowledge base navigabile del corpus normativo NIS2 italiano: direttiva UE, decreto di recepimento, determinazioni e FAQ ACN, allegati tecnici, regolamento di esecuzione UE, guidance ENISA, standard di riferimento (NIST CSF 2.0, FNCDP, ISO/IEC 27000-series) e L. 90/2024.

103 nodi in quattro layer, costruiti con la metodologia "LLM Wiki": le fonti sono lette per intero, ogni fonte ha una pagina di sintesi, ogni concetto e ogni entità hanno una pagina propria con i riferimenti incrociati, e le analisi derivate sono pagine separate con la domanda che le ha generate. Il vault è pensato per Obsidian, ma si legge anche da GitHub.

> **Progetto personale di studio. Non costituisce parere legale né consulenza professionale.**
> Le fonti ufficiali (ACN, Gazzetta Ufficiale, EUR-Lex) prevalgono sempre su quanto riportato qui. Ogni nodo cita la fonte da cui deriva; prima di assumere conclusioni operative, verificare sul testo ufficiale e con un consulente qualificato.

## Da dove iniziare

- `index.md`: catalogo di tutti i nodi, raggruppato per layer e per ondata di acquisizione.
- `wiki/synthesis/`: le sette analisi derivate, ciascuna con la domanda di partenza. Tra queste: il cross-walk tra art. 21 NIS2, NIST CSF 2.0, FNCDP 2025 e ISO/IEC 27002:2022; il coordinamento tra Reg. UE 2024/2690 e Det. ACN 379907/2025; il coordinamento tra L. 90/2024 e D.Lgs. 138/2024; la cronologia attuativa italiana.
- `log.md`: cronologia append-only di ogni acquisizione, query e lint.
- `_meta/`: report delle ondate di acquisizione, decision log, documenti scartati con motivazione.

## Come è organizzata

| Layer | Nodi | Contenuto |
|---|---|---|
| `wiki/sources/` | 40 | una pagina per ogni fonte: TL;DR, punti chiave, citazioni con riferimento puntuale, note su lacune e contraddizioni |
| `wiki/entities/` | 17 | organizzazioni, ruoli, strumenti (ACN, CSIRT Italia, Tavolo NIS, ...) |
| `wiki/concepts/` | 39 | istituti e temi: ambito, categorizzazione, misure di base, incidenti significativi, salvaguardia dimensionale, regimi correlati, ... |
| `wiki/synthesis/` | 7 | analisi derivate e risposte a domande |

Ogni nodo ha un frontmatter YAML con tipo, fonti, tag e un campo `scope` (`nis2_tool`, `grc_personal`, `both`) che distingue il contenuto strettamente NIS2 da quello di contesto GRC.

## Fonti coperte

- **Normativa primaria**: Direttiva (UE) 2022/2555; D.Lgs. 138/2024; L. 90/2024; Reg. di esecuzione (UE) 2024/2690.
- **ACN**: determinazioni (specifiche di base 379907/2025 con Allegati 1-4; piattaforma e procedure; categorizzazione con i due modelli; termini soggetti 2026; accordi di condivisione; composizione e funzionamento del Tavolo NIS); Linee guida gestione incidenti; Guida alla lettura delle specifiche di base; le 8 aree di FAQ; la pagina ufficiale "La normativa NIS"; Strategia nazionale 2022-2026 e Manuale Misura 82.
- **ENISA**: Technical Implementation Guidance v1.0; Mapping Table v1.0; ECSF Role Profiles; Mapping NIS2-ECSF; Handbook for Cyber Stress Tests v2.0.
- **Standard**: NIST CSF 2.0; FNCDP 2025 v2.1; ISO/IEC 27000:2018, 27001:2022, 27002:2022.

I documenti sorgente non sono ridistribuiti in questo repository: ogni pagina `sources/` riporta l'identificativo ufficiale del documento (numero, data, protocollo dove attestato) e, dove esiste, il link alla fonte. Gli standard ISO a pagamento sono citati solo per numero di clausola o controllo, mai nel testo.

## Metodo

- **Identità documentale dal testo.** L'identità di una fonte si stabilisce dal contenuto (clausola di successione, data di applicazione, struttura, firma), mai dal nome del file o da fonti secondarie. Il numero di protocollo delle determinazioni ACN è registrato solo dove è attestato; dove non lo è, lo dice la sezione seguente.
- **Citazioni a granularità verificata.** Un riferimento ad articolo, comma, codice FAQ o paragrafo compare solo se riscontrato sul testo. Ciò che non è riscontrato è marcato "da verificare" nel nodo e non viene mai assunto.
- **Acquisizione a ondate** con review tra un'ondata e l'altra e lint periodico (contraddizioni, orfani, cross-reference mancanti). Le contraddizioni tra fonti sono marcate con callout `[!warning]` e non vengono nascoste.
- Il vault è scritto e mantenuto da un LLM (Claude) sotto direzione dell'autore, che cura le fonti, pone le domande e rivede ogni ondata. Il valore sta nella struttura del corpus, non nel modello.

## Stato di verifica

Questa sezione elenca ciò che la KB dichiara di non aver ancora verificato. È parte del metodo, non un difetto da nascondere.

**Punti marcati "da verificare" nei nodi (20):**
- `concepts/Elementi essenziali di cybersicurezza (procurement)`: 3 (DPCM ex art. 14 L. 90/2024 e rinvio a schemi di certificazione UE)
- `concepts/Referente per la cybersicurezza (L. 90-2024)`: 1 (determinazione ACN ex art. 8 c. 1 lett. f)
- `concepts/Settori altamente critici e critici`: 1 (sotto-categorie italiane in Allegato)
- `sources/Direttiva (UE) 2022-2555 (NIS2)`: 1 (rettifiche nella versione consolidata)
- `sources/FAQ NIS - Settori, sottosettori e tipologie di soggetto`: 1 (riferimento al DSA)
- `sources/Legge 90-2024 (cybersicurezza nazionale)`: 7 (atti attuativi: art. 1 c. 1, art. 1 c. 5, art. 11, art. 12, art. 13 c. 5, art. 14 c. 1, art. 15)
- `synthesis/Coordinamento L. 90-2024 e NIS2`: 3
- `synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025`: 1 (più una open question normativa segnalata nel nodo)
- `synthesis/Cronologia attuativa NIS2 in Italia`: 2

A questi si aggiungono 4 punti marcati "da chiarire" (D.Lgs. 138-2024, FAQ Aggiornamento, FAQ Registrazione, Cronologia attuativa NIS2 in Italia) e una nota in ISO IEC 27000-2018 sulla verifica contro la copia ufficiale.

**Determinazioni ACN con numero di protocollo non stampato nel testo (6):** per sei determinazioni il numero di protocollo non è stampato nel testo; l'attribuzione è attestata tramite FAQ ACN o pagina ufficiale ACN. Tramite FAQ ACN: piattaforma e procedure (127437/2026), categorizzazione (155238/2026), specifiche di base (379907/2025). Tramite la pagina ufficiale ACN "La normativa NIS": termini soggetti 2026 (127434/2026), accordi di condivisione (136118/2025), composizione Tavolo NIS (112335/2026); per queste tre la fonte dell'attribuzione è registrata nel frontmatter del nodo (`protocol_source`). Nessuna attribuzione resta senza attestazione.

**Riferimenti citati e non ancora acquisiti (6):** D.L. 105/2019 (perimetro di sicurezza nazionale cibernetica), D.Lgs. 65/2018, D.Lgs. 231/2001, Ministero dell'Economia e delle Finanze, Ministero della Cultura, Ministero dell'Università e della Ricerca. Nel grafo compaiono come nodi non risolti.

**Concetti citati senza pagina propria (7):** Tipologie di soggetto, Servizi gestiti, Servizi di sicurezza gestiti, Pubbliche amministrazioni NIS, Imprese collegate (art. 3 c. 10), Eccezioni di prevalenza, Giurisdizione nazionale.

**Lacune strutturali note:** D.L. 82/2021 (istituzione ACN), D.L. 105/2019, L. 124/2007 e gli atti attuativi della L. 90/2024 non sono acquisiti; DORA (Reg. UE 2022/2554) e D.Lgs. 134/2024 (soggetti critici) sono trattati solo come regimi correlati.

**Ultimo aggiornamento di contenuto:** 2026-05-23 (Wave 7, L. 90/2024). Correzione di contenuto del 2026-10-26 (lint: Size-cap rule allineata alla FAQ AMB.DI.1) e manutenzione, registrate in `log.md`.

## Cosa non è

Non è uno strumento di valutazione: non dice se un soggetto rientra o meno nel perimetro NIS2. Un tool di pre-screening che usa questo corpus è in sviluppo in un repository separato e non è ancora rilasciato.

## Licenza

Contenuto di `wiki/`, `index.md`, `log.md` e `_meta/`: [CC BY 4.0](LICENSE). I documenti ufficiali citati restano dei rispettivi titolari e non sono inclusi.

## Autore

Andrea Tierno. Segnalazioni e correzioni: issue su questo repository.
