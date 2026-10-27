# Decision log — NIS2 Tool & scope governance

Registro append-only delle decisioni di governance che riguardano lo `scope:` tagging dei nodi del vault e l'export della Project Knowledge del NIS2 Tool. Ogni voce: data, decisione, motivazione, stato. Le decisioni pianificate (non ancora eseguite) restano in cima alla propria voce con lo stato `PIANIFICATA` finché non vengono attuate.

Convenzione stato: `ATTUATA` | `PIANIFICATA` | `REVOCATA`.

---

## [2026-07-02] DEC-001 — Retag `Coordinamento DORA-NIS` a `scope: both`

**Stato:** ATTUATA (2026-07-02)

**Nodo:** [[concepts/Coordinamento DORA-NIS]] — `scope: grc_personal` → `scope: both`.

**Decisione:** portare il nodo nell'export della Project Knowledge del tool v0.1.0.

**Motivazione:** DORA è una delle domande binarie di disambiguazione del wizard; il nodo compare nel catalogo eccezioni del gate v0.1.0 con citazioni puntuali (art. 3 c. 14 D.Lgs. 138/2024; esoneri via [[sources/Determinazione ACN piattaforma e procedure - 2026-04-13|Det. 127437/2026]]); il copy del verdetto dovrà segnalare l'esonero DORA. Escluderlo dall'export rendeva impossibile validare i contenuti DORA del corpus contro la KB e creava un'incoerenza tra ciò che il tool cita e ciò che pubblica. Costo del retag: una riga di frontmatter.

**Impatto operativo:** nessuna modifica a `index.md` (la riga del catalogo non espone lo `scope`, non esiste un tally aggregato per valore). Voce corrispondente in `log.md`.

---

## [2026-07-02] DEC-002 — Retag `Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002` a `scope: both`

**Stato:** ATTUATA (2026-07-02) — anticipata rispetto al trigger originario (kickoff v0.2)

**Nodo:** [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] — `scope: grc_personal` → `scope: both`.

**Decisione:** portare il nodo nell'export della Project Knowledge. Originariamente pianificata come retag differito al kickoff v0.2; anticipata su richiesta dell'utente il 2026-07-02.

**Motivazione:** il cross-walk a 4 framework è la base dell'estensione controlli (Fase 3, v0.2). Nella v0.1.0 (verdetto di sola ambito) il cross-walk resta out-of-MVP, ma il retag anticipato evita di dover rifare l'export della Project Knowledge a metà sviluppo v0.2 e allinea da subito il tag alla natura dual-purpose del nodo (asset GRC/ISO LA + base controlli tool).

**Impatto operativo:** aggiornata anche la prosa del nodo (riga che dichiarava `scope: grc_personal`) per coerenza col frontmatter. Nessuna modifica a `index.md`. Voce corrispondente in `log.md`.

---

## [2026-07-02] DEC-003 — Credito stop-and-ingest NON consumato + correzione identità Det. 127434/127437

**Stato:** ATTUATA (2026-07-02)

**Contesto:** la direttiva "STOP-AND-INGEST — Det. ACN 127437/2026" (annunciata come secondo e ultimo credito) partiva da una premessa falsa (`251218` = Det. 379887 abrogata; `Det_127437_2026.pdf` = piattaforma corretta). La verifica sul testo ha invertito entrambe le premesse: il nodo piattaforma era già costruito sul testo corretto (Det. 127437/2026 vigente); `Det_127437_2026.pdf` era la determinazione **termini** (protocollo 127434) con filename errato.

**Decisione:** poiché l'operazione si è risolta in una **correzione di attestazione** (no-op di re-ingest, il testo era già quello giusto) e la sua premessa era falsa, **il secondo credito stop-and-ingest NON è consumato**. **Residuo: 1 credito fino a v0.1.0.**

**Azioni attuate:** `source_path` del nodo piattaforma agganciato al PDF firmato reale; DIV-P1 chiusa (esoneri DORA verificati sul testo, corpus v0.2.1); `Det_127437_2026.pdf` rinominato `Det_127434_2026_termini.pdf` e agganciato al nodo termini; micro-verifica art. 3 c. 4 vs c. 12 (funzioni distinte, citazione allineata). Analisi dell'errore e checklist di ingest estesa in `nis2-check/docs/decisions/0007-*`.

**Impatto operativo:** nessuna modifica a `index.md` (one-liner invariati). Voce corrispondente in `log.md`. Copia ridondante `detacn_misuresicurezza-v4_post.pdf` non rimossa (cancellazione in `raw/` non autorizzata): consolidamento rimesso all'utente. → Consolidata in **DEC-004**.

---

## [2026-07-02] DEC-004 — Archiviazione copia ridondante `detacn_misuresicurezza-v4_post.pdf`

**Stato:** ATTUATA (2026-07-02)

**File:** `raw/articles/detacn_misuresicurezza-v4_post.pdf` → `raw/_archive/detacn_misuresicurezza-v4_post.pdf` (spostato, **non cancellato**).

**Contesto:** verifica di igiene su `raw/`. Nessun nodo KB referenzia il file in `source_path` (le uniche occorrenze sono prose in `log.md`, in questo registro e nella nota di provenienza del nodo termini). Il file è testualmente identico a `Det_127434_2026_termini.pdf` (stessa firma 13/04/2026 12:12:15; differisce solo l'MD5 per metadati PDF): è la copia ridondante segnalata in DEC-003.

**Decisione:** archiviare in `raw/_archive/` (directory già esistente, con precedente `CELEX_32022L2555_IT_TXT_DUPLICATE.pdf`), coerente con la regola "non cancellare in `raw/`". Il nodo termini resta agganciato a `raw/articles/Det_127434_2026_termini.pdf`.

**Impatto operativo:** aggiornata la nota di provenienza in [[sources/Determinazione ACN termini soggetti 2026 - 2026-04-30]] (nuova posizione del file). Nessuna modifica a `index.md`. Voce corrispondente in `log.md`.

---

## [2026-10-26] DEC-005 — Gate pre-lancio: KB esente dalla review GRC terza (opzione B)

**Stato:** ATTUATA (2026-10-26)

**Decisione:** Gate pre-lancio: KB esente dalla review GRC terza (opzione B). Decisione registrata in `nis2-check/docs/decisions/0008`.

**Condizioni:** README con disclaimer e stato di verifica; `raw/` e `_tmp/` mai pubblicati; riferimenti personali generalizzati.

**Impatto operativo:** nessuna modifica a `index.md`. Voce corrispondente in `log.md`.

---

## [2026-10-27] DEC-006 — Correzione di contenuto: attestazione art. 3 c. 6 nel nodo D.Lgs. 138/2024

**Stato:** ATTUATA (2026-10-27)

**Nodo:** [[sources/D.Lgs. 138-2024 (Decreto NIS)]] — `scope: both` invariato.

**Classe:** correzione di contenuto (stessa classe delle correzioni `lint` del 2026-10-26 su [[concepts/Size-cap rule]] e [[sources/Direttiva (UE) 2022-2555 (NIS2)]]). Non è un ingest: nessuna fonte nuova, nessun nodo creato.

**Decisione:** integrare nel nodo l'art. 3 c. 6 D.Lgs. 138/2024 (applicazione alle pubbliche amministrazioni dell'Allegato III indipendentemente dalla dimensione), con citazione testuale verificata sul PDF (`raw/articles/Decreto NIS2.pdf`) e rinvio a [[sources/FAQ NIS - Settori, sottosettori e tipologie di soggetto]], che già lo attestava.

**Motivazione:** il nodo sorgente della norma primaria non attestava un comma che un nodo derivato (FAQ) citava. Il corpus del tool cita già art. 3 c. 6 e non cambia: nessuna voce in `nis2-check/corpus/CHANGELOG.md`.

**Impatto operativo:** una riga aggiunta al nodo, frontmatter invariato. Nessuna modifica a `index.md`. Voce corrispondente in `log.md`.

---

## [2026-10-27] DEC-007 — Ambito soggettivo della PA nel D.Lgs. 138/2024

### Parte A — Riscontro del PDF sulla fonte vigente

**Stato:** ATTUATA (2026-10-27)

**Nodo:** [[sources/D.Lgs. 138-2024 (Decreto NIS)]] — `source_path` invariato (`raw/articles/Decreto NIS2.pdf`).

**Contesto:** gli allegati del PDF portano l'intestazione "SCHEMA DI DECRETO LEGISLATIVO DI RECEPIMENTO DELLA NIS2". Prima di correggere l'ambito PA serviva escludere che il PDF riproducesse uno schema diverso dal testo in vigore.

**Riscontro:** testo vigente scaricato da Normattiva (urn:nir:stato:decreto.legislativo:2024-09-04;138, vigenza 2026-10-27; GU n. 230 del 2024-10-01). Confronto parola per parola, con normalizzazione dei soli spazi e a capo, di: Allegato III (135 parole), art. 3 c. 6 (34) e c. 7 (92), art. 4 c. 2 (57) e c. 3 (79), art. 6 c. 1 (159), c. 2 (42) e c. 3 (31), art. 40 c. 2 lett. b) (24) e c. 5 lett. a) (24). Esito: **identico**, nessuna differenza, refuso "individuatele" compreso. Articoli 3, 4, 6, 40 e Allegato III in versione 1, testo in vigore dal 2024-10-16. L'intestazione "SCHEMA DI DECRETO LEGISLATIVO" compare anche nell'Allegato III su Normattiva: appartiene al testo pubblicato, non indica una bozza.

**Decisione:** nessun file nuovo in `raw/`, PDF non archiviato. Nota di provenienza (`provenance_note`) aggiunta al frontmatter del nodo. Credito stop-and-ingest consumato su indicazione dell'autore: contatore a 0 fino al pre-rilascio v0.1.0 (registrato in `nis2-check/docs/STATUS.md`).

**Impatto operativo:** nessuna modifica a `index.md`. Voce corrispondente in `log.md`. Parte B (correzioni di contenuto) eseguita sul testo così verificato.

### Parte B — Correzione di contenuto: ambito PA

**Stato:** ATTUATA (2026-10-27)

**Classe:** correzione di contenuto (stessa classe di DEC-006 e delle correzioni `lint` del 2026-10-26). Non è un ingest.

**Nodi:** [[sources/D.Lgs. 138-2024 (Decreto NIS)]], [[concepts/Ambito di applicazione NIS2]], [[concepts/Identificazione dei soggetti NIS]], [[concepts/Size-cap rule]], [[concepts/Settori altamente critici e critici]], [[concepts/Perimetro Legge 90-2024]], [[concepts/Soggetti essenziali e importanti]]; nota redazionale in [[sources/FAQ NIS - Ambito]]. Scope dei nodi invariato (tutti `both`).

**Decisione:** sostituire "PA centrali" con la PA dell'Allegato III lett. a)-d) (art. 3 c. 6), con rinvio al nodo D.Lgs., che ora riporta le 15 categorie testuali, l'estensione con DPCM (art. 3 c. 7, art. 40 c. 2 lett. b), le esclusioni (art. 4 cc. 2-3) e le qualifiche (art. 6 c. 1 lett. e) e cc. 2-3).

**Nota:** la restrizione è nata in sintesi (*inferenza dell'agente:* la qualifica di essenziale delle PA centrali, art. 6 c. 1 lett. e), letta come perimetro dell'intero rientro PA) e si è propagata in sette nodi e nel corpus del tool (categoria d) ridotta agli enti a struttura associativa, qualifiche a) e b)). Seconda occorrenza di una restrizione di sintesi propagata, dopo Size-cap rule del 2026-10-26.

**Impatto operativo:** `index.md` solo nella riga "Ultimo aggiornamento", contatori invariati. README, sezione "Stato di verifica": riga datata. Voce corrispondente in `log.md`. Corpus non modificato: pacchetto C1-C6 registrato come punto aperto in `nis2-check/docs/STATUS.md`, per corpus 0.5.0 dopo S2.
