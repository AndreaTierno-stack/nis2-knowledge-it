# Wave 6.5 — Retrofit tagging `scope:` — PLANNED

**Stato**: pianificata, **non eseguita**. Da avviare dopo il completamento dei cluster B-F di Wave 6.

## Obiettivo

Applicare il tagging `scope:` (`nis2_tool` / `grc_personal` / `both`) a **tutti i nodi della wiki che non sono stati toccati dal Cluster A di Wave 6 né dagli eventuali cluster B-F successivi**. Target indicativo: ~50 nodi (da raffinare con conteggio esatto a inizio wave).

## Razionale

Il Cluster A di Wave 6 ha applicato il tagging `scope:` solo ai nodi citati nei due nuovi nodi della wave (33 nodi su ~83 totali). I restanti ~50 nodi non hanno il campo `scope:` nel frontmatter. Fino a Wave 6.5, lo script di export filtrato per Project Knowledge del NIS2 Tool non è eseguibile in modo affidabile.

## Perché dopo i cluster B-F

L'ingest di B/C/D/E/F potrebbe:
- Creare nuovi nodi che citano nodi attualmente non taggati, generando ulteriori aggiornamenti spontanei.
- Modificare la valutazione di scope per alcuni nodi esistenti (es. Strategia nazionale di cybersicurezza potrebbe risultare più rilevante per `both` se la pagina ACN strategica cluster E lo cita estensivamente).
- Ridurre il lavoro residuo di Wave 6.5.

## Regola di scope per Wave 6.5

Regola del brief Wave 6 (decision tree in 6 punti) + **regola di precisazione emersa dalla human review del Cluster A**:

> Un nodo è `both` se è **citato o richiamato dal NIS2 Tool nell'esito preliminare** (PDF di esito, copy del wizard, sezione obblighi-chiave) per orientare il destinatario sugli obblighi derivanti dal rientro nell'ambito.
>
> Un nodo è `grc_personal` se il suo contenuto serve al consulente **dopo** il verdetto, per impostare il lavoro post-rientro (gap analysis, design delle misure, audit), ma non finisce nel PDF di esito.

Test pratico: *"questo nodo finisce in una frase del PDF di esito?" → sì = `both`; no = `grc_personal`.*

## Candidati noti (preliminare, non esaustivo)

### Probabili `both`
- Tutte le altre determinazioni ACN (categorizzazione, piattaforma, accordi, termini soggetti 2026, composizione Tavolo, funzionamento Tavolo)
- Tutte le 8 FAQ NIS (sono dirette al destinatario nel registro che il tool replica)
- `concepts/Sanzioni NIS2` (citato in copertina del PDF)
- `concepts/Clausola di salvaguardia` (caso da segnalare nel verdetto)
- `concepts/Coordinated Vulnerability Disclosure` (citato come obbligo)
- `concepts/Verifiche di coerenza` e `Verifiche di conformità categorizzazione` (procedurale post-registrazione)
- `concepts/Aggiornamento annuale informazioni` e `Aggiornamento continuo informazioni` (obblighi procedurali post-rientro)
- `concepts/Accordi di condivisione delle informazioni` (citato come facoltà)
- `concepts/Fornitori rilevanti NIS` (segnalato nel verdetto se il soggetto rientra come fornitore)
- `concepts/Soggetti PSNC-NIS` (segnalato come automatismo nel verdetto)
- `concepts/Macro-aree NIS`, `Categorie di rilevanza` (già fatti in Cluster A)
- `concepts/Regime transitorio OSE` e `Regime transitorio telco` (segnalati nel verdetto se applicabili)
- `concepts/Piattaforma digitale ACN` (citato come canale procedurale)
- `concepts/Punto di contatto NIS`, `Referente CSIRT`, `Rappresentante NIS in Italia` (ruoli da designare post-rientro, citati nel PDF)
- `entities/Autorità di settore NIS`, `Tavolo per l'attuazione della disciplina NIS`, `Comitato per la Cybersicurezza`, etc. (governance del regime, citati per orientamento)
- `entities/Framework Nazionale per la Cybersecurity` (fonte tecnica della det. 379907)

### Probabili `grc_personal`
- `concepts/Processo gestione incidenti NIS` (procedura interna post-rientro)
- `entities/NIST SP 800-61` (standard tecnico per incident response)
- `entities/Linee Guida NIS - Gestione incidenti - 2025-12` (guida operativa post-rientro)
- `entities/EU-CyCLONe` (rete operativa UE, fuori dal verdetto)
- `entities/Rete di CSIRT nazionali` (idem)
- `entities/Nucleo per la Cybersicurezza` (governance di livello politico-strategico)
- `entities/Comitato Interministeriale per la Cybersicurezza` (idem)
- `entities/Ministero della Difesa` (eccezione clausola di salvaguardia, ma non finisce nel PDF al di fuori di un caso ad hoc)

### Da decidere a lettura
- `concepts/Strategia nazionale di cybersicurezza` (potenzialmente `both` se la posizionamento del PDF la cita come cornice)
- `concepts/Approccio multi-rischio` (principio, attualmente `grc_personal` in Cluster A — confermare)
- Tutti gli altri nodi non elencati sopra (da censire a inizio wave)

## Output atteso

- Tutti i nodi della wiki hanno il campo `scope:` nel frontmatter.
- Report Wave 6.5 con distribuzione finale e razionali per nodo.
- Script di export filtrato per Project Knowledge tool ora eseguibile (lavoro separato, fuori da Wave 6.5).

## Stima effort

~50 nodi × ~2-3 minuti/nodo (lettura frontmatter + decisione scope + edit + razionale nel report) = ~2-3 ore di sessione Claude Code.
