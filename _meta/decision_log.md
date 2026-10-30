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

**Nota (2026-10-28):** riscontro con esito no-op: non consuma il credito stop-and-ingest (DEC-003); residuo 1.

### Parte B — Correzione di contenuto: ambito PA

**Stato:** ATTUATA (2026-10-27)

**Classe:** correzione di contenuto (stessa classe di DEC-006 e delle correzioni `lint` del 2026-10-26). Non è un ingest.

**Nodi:** [[sources/D.Lgs. 138-2024 (Decreto NIS)]], [[concepts/Ambito di applicazione NIS2]], [[concepts/Identificazione dei soggetti NIS]], [[concepts/Size-cap rule]], [[concepts/Settori altamente critici e critici]], [[concepts/Perimetro Legge 90-2024]], [[concepts/Soggetti essenziali e importanti]]; nota redazionale in [[sources/FAQ NIS - Ambito]]. Scope dei nodi invariato (tutti `both`).

**Decisione:** sostituire "PA centrali" con la PA dell'Allegato III lett. a)-d) (art. 3 c. 6), con rinvio al nodo D.Lgs., che ora riporta le 15 categorie testuali, l'estensione con DPCM (art. 3 c. 7, art. 40 c. 2 lett. b), le esclusioni (art. 4 cc. 2-3) e le qualifiche (art. 6 c. 1 lett. e) e cc. 2-3).

**Nota:** la restrizione è nata in sintesi (*inferenza dell'agente:* la qualifica di essenziale delle PA centrali, art. 6 c. 1 lett. e), letta come perimetro dell'intero rientro PA) e si è propagata in sette nodi e nel corpus del tool (categoria d) ridotta agli enti a struttura associativa, qualifiche a) e b)). Seconda occorrenza di una restrizione di sintesi propagata, dopo Size-cap rule del 2026-10-26.

**Impatto operativo:** `index.md` solo nella riga "Ultimo aggiornamento", contatori invariati. README, sezione "Stato di verifica": riga datata. Voce corrispondente in `log.md`. Corpus non modificato: pacchetto C1-C6 registrato come punto aperto in `nis2-check/docs/STATUS.md`, per corpus 0.5.0 dopo S2.

---

## [2026-10-28] DEC-008 — Correzione di contenuto: soggetti critici, DORA, Cloud PA, Reg. UE 2024/2690

**Stato:** ATTUATA (2026-10-28)

**Classe:** correzione di contenuto (stessa classe di DEC-006 e DEC-007 parte B). Non è un ingest: nessuna fonte nuova, nessun nodo creato in `wiki/`.

**Nodi (16):** [[sources/D.Lgs. 138-2024 (Decreto NIS)]], [[sources/FAQ NIS - Settori, sottosettori e tipologie di soggetto]], [[sources/FAQ NIS - Ambito]], [[sources/FAQ NIS - Registrazione]], [[sources/FAQ NIS - Categorizzazione]], [[sources/Determinazione ACN categorizzazione - 2026-04-13]], [[sources/Regolamento di esecuzione UE 2024-2690]], [[sources/Direttiva (UE) 2022-2555 (NIS2)]], [[concepts/Ambito di applicazione NIS2]], [[concepts/Settori altamente critici e critici]], [[concepts/Size-cap rule]], [[concepts/Identificazione dei soggetti NIS]], [[concepts/Coordinamento DORA-NIS]], [[concepts/Categorizzazione dei soggetti]], [[synthesis/Stratificazione delle norme cybersecurity in Italia]], [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]]. Scope invariato.

**Decisione:** correggere, dopo riscontro sul testo in `raw/`, le imprecisioni critiche della lettura del 2026-10-28: (1) testo dell'art. 3 cc. 5, 9, 10, 14, 15, art. 2 c. 1 lett. bbb) e art. 40 c. 5 lett. a) nel nodo D.Lgs., numerazione dei Capi IV-V; (2) soggetti critici (art. 3 c. 5 lett. a), art. 6 c. 1 lett. b)) negli elenchi "a prescindere dalla dimensione", con c. 9 e c. 10; (3) DORA su due livelli, legge (art. 3 c. 14: settori 3-4, art. 17 e Capi IV-V) e determinazione (Det. 127437/2026: entità DORA in ambito NIS, art. 7 c. 6, 16 c. 13, 20 c. 6), con nota sull'incoerenza interna di `AMB.NO.2`; (4) Cloud PA secondo la condizione dell'art. 4 Det. 155238/2026 ("hanno svolto la classificazione"), FAQ `CAT.8` e `A1.8.2`; (5) FAQ Settori, sottosettore elettrico; (6) Reg. UE 2024/2690 riferito agli Allegati I pp. 8-9 e II p. 6, definizione cloud testuale; (7) "CER" nudo sostituito da "soggetti critici (D.Lgs. 134/2024)", con regola in `_meta/convenzioni_di_naming.md`.

**Nota:** seconda ricorrenza dello schema DEC-007: un'omissione nata in sintesi si è propagata in sette nodi e nel corpus del tool. *Inferenza dell'agente sull'origine:* la mappa size-blind è stata costruita sulla FAQ Settori, che non tratta i soggetti critici, e poi letta come elenco completo dell'art. 3 c. 5. Contromisura per i lint successivi: ogni elenco "a prescindere dalla dimensione" si confronta con il testo dell'art. 3 cc. 5, 6, 8, 9 e 10, ora nel nodo D.Lgs.

**Impatto operativo:** `index.md` solo nelle righe "Ultimo aggiornamento", FAQ Ambito e Coordinamento DORA-NIS; contatori invariati. README, sezione "Stato di verifica": riga datata; il "Backlog lint" con le 29 imprecisioni non critiche della lettura è da aggiungere. Voce corrispondente in `log.md`. Corpus non modificato: allineamento da registrare come punto aperto in `nis2-check/docs/STATUS.md`.

---

## [2026-10-30] DEC-009 — Lint 2026-10-30: correzioni minime dopo il registro citazioni del corpus 0.6.0

**Stato:** ATTUATA (2026-10-30)

**Classe:** correzione di contenuto (stessa classe di DEC-006, DEC-007 parte B, DEC-008). Non è un ingest: nessuna fonte nuova, nessun nodo creato, credito stop-and-ingest non usato (residuo 1).

**Origine:** correzioni minime proposte e non eseguite in `nis2-check/docs/verifications/2026-10-28-registro-citazioni.md`, più una voce nuova (V8). Report di verifica: `nis2-check/docs/verifications/2026-10-30-lint-kb.md`.

**Nodi (6):** [[sources/FAQ NIS - Settori, sottosettori e tipologie di soggetto]], [[sources/D.Lgs. 138-2024 (Decreto NIS)]], [[sources/Determinazione ACN piattaforma e procedure - 2026-04-13]], [[sources/FAQ NIS - Profili generali]], [[sources/FAQ NIS - Ambito]], [[concepts/Clausola di salvaguardia]]. Scope invariato.

**Voci ed esiti** (verifica sul PDF in `raw/`, estrazione `pdftotext -enc UTF-8`):
- V1, interconnessione diretta: **attestato** in `A1.9.2` (criterio ed esempi, p. 16); `A1.9.3` e `A1.9.4` riprendono il requisito con rinvio ad `A1.9.2` (p. 17), ora esplicito. Citazione in coda invariata.
- V2, etichette `A1.8.1` e `A1.9.1`: **attestato**; etichette aggiunte a cluster, giurisdizione e tipologie.
- V3, art. 7 c. 1 lett. d) D.Lgs. 138/2024: **attestato**, pertinente; testuale nel nodo D.Lgs.
- V4, art. 11 c. 2 lett. g) Det. 127437/2026: **attestato**; lettere a)-g) esplicite, lett. g) in testo; rettifica della lett. f) (per la PA facoltativi fatturato e bilancio, non i dipendenti).
- V5, `GEN.6`: **attestato in parte**: selezione di "uno o più settori/sottosettori" e della "relativa tipologia"; nessun riferimento a "tutte le tipologie". Passo testuale nella tabella degli obblighi.
- V6, rinvii: **rettificato** (forma): "(c. 1)" nel nodo D.Lgs.; "art. 3 cc. 8 e 13" in due righe della FAQ Settori.
- V7, ASL `A3.c.4.1`: **rettificato**: "doppia registrazione" → registrazione "per entrambi i settori e le tipologie di soggetto cui appaiono riconducibili".
- V8, salvaguardia dimensionale (DPCM 221/2024): **rettificato**. La frase di `AMB.GI.2` è della FAQ: testo lasciato, nota redazionale datata. Il decreto distingue l'applicazione dell'ACN (art. 3 c. 12) dall'individuazione delle Autorità di settore (art. 11 c. 4 lett. c)); "d'intesa" non attestato per la salvaguardia, riga "Chi decide" riformulata.

**Nota:** la premessa di V8 ("il decreto attribuisce l'applicazione all'ACN", quindi divergenza piena con la FAQ) era incompleta: l'art. 11 c. 4 lett. c), richiamato dalla stessa FAQ, assegna alle Autorità di settore l'individuazione dei soggetti cui si applica la deroga. La nota registra entrambe le attribuzioni del decreto, non una divergenza piena. Rilievo nuovo, non corretto (fuori dalle voci): nel concept Clausola di salvaguardia, righe 30 e 54, l'art. 12 della Det. 127437/2026 è descritto come "modalità riservate" per sicurezza nazionale e difesa, ma l'art. 12 disciplina la salvaguardia dimensionale; nel backlog del README.

**Impatto operativo:** `index.md` solo nella riga "Ultimo aggiornamento", contatori invariati. README, sezione "Stato di verifica": riga datata e una voce nel Backlog lint. Voce corrispondente in `log.md`. Corpus non modificato: `faq_a1_9_2` resta corretto per il criterio; ID ora attestabili (`dlgs_138_2024_art_7_c_1_lett_d`, `det_piattaforma_127437_2026_art_11_c_2_lett_g`, `faq_a1_8_1`, `faq_a1_9_1`, `dlgs_138_2024_art_3_c_1`; `faq_gen_6` solo per la selezione di settori e tipologia) da valutare per il corpus 0.6.1 (`nis2-check/docs/STATUS.md`, punto 9).
