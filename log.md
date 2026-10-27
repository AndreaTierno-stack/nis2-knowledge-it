# Log — LLM Wiki

> Cronologia append-only. Ogni voce ha header in formato `## [YYYY-MM-DD] <op> | <oggetto>` per essere parsabile via `grep "^## \[" log.md | tail -N`.

---

## [2026-04-28] init | Bootstrap della wiki
Pagine create:
- [[CLAUDE]] — schema completo (regole, workflow, convenzioni)
- [[index]] — catalogo content-oriented (vuoto)
- [[log]] — questo file

Cartelle create:
- `raw/{articles, papers, notes, assets}` — fonti immutabili
- `wiki/{entities, concepts, sources, synthesis}` — pagine generate dall'LLM

Note: wiki avviata da Andrea. Lingua di default: italiano. Front-end: Obsidian. Pattern: LLM Wiki (second brain).

## [2026-04-28] cleanup | rimossa demo Memex + correzione nome utente
Motivo: Andrea ha chiesto di cancellare la fonte demo (off-topic rispetto al dominio NIS2) e di correggere "Francesco" → "Andrea" (il path Windows era ingannevole).

Pagine cancellate:
- `raw/articles/As We May Think — Vannevar Bush (1945).md`
- `wiki/sources/As We May Think — Bush 1945.md`
- `wiki/entities/`: Vannevar Bush, Ted Nelson, Douglas Engelbart, Tim Berners-Lee, Belinda Barnet, The Atlantic Monthly, Office of Scientific Research and Development
- `wiki/concepts/`: Memex, Trail associativi, Ipertesto, Knowledge management

Pagine aggiornate:
- [[CLAUDE]] — sostituito "Francesco" con "Andrea", aggiunta nota sul nome
- [[index]] — reset, dominio attivo dichiarato (NIS2)
- Memoria interna agente — user_profile e project aggiornati

## [2026-04-28] ingest | Wave 1 — Normativa primaria NIS2 [in corso]
Fonti previste:
- `Publications Office.pdf` — Direttiva (UE) 2022/2555 (NIS2)
- `Decreto NIS2.pdf` — D.Lgs. 4 settembre 2024, n. 138
- `La normativa - ACN.pdf` — pagina-panoramica ACN

Ritmo: Wave 1 → review da Andrea → Wave 2 (8 determinazioni ACN).

## [2026-04-29] ingest | Wave 1 — Normativa primaria NIS2 [chiusa]
Pagine create (34):

Sources (3):
- [[sources/Direttiva (UE) 2022-2555 (NIS2)]]
- [[sources/D.Lgs. 138-2024 (Decreto NIS)]]
- [[sources/La normativa NIS - Pagina ACN]]

Entities (12):
- [[entities/ACN]]
- [[entities/CSIRT Italia]]
- [[entities/ENISA]]
- [[entities/Tavolo per l'attuazione della disciplina NIS]]
- [[entities/Comitato Interministeriale per la Cybersicurezza]]
- [[entities/Nucleo per la Cybersicurezza]]
- [[entities/Gruppo di Cooperazione NIS]]
- [[entities/EU-CyCLONe]]
- [[entities/Rete di CSIRT nazionali]]
- [[entities/Autorità di settore NIS]]
- [[entities/Ministero della Difesa]]
- [[entities/Comitato per la Cybersicurezza]]

Concepts (18):
- [[concepts/NIS2]]
- [[concepts/Soggetti essenziali e importanti]]
- [[concepts/Identificazione dei soggetti NIS]]
- [[concepts/Size-cap rule]]
- [[concepts/Ambito di applicazione NIS2]]
- [[concepts/Settori altamente critici e critici]]
- [[concepts/Misure di gestione del rischio cyber]]
- [[concepts/Notifica di incidente significativo]]
- [[concepts/Incidente significativo]]
- [[concepts/Approccio multi-rischio]]
- [[concepts/Categorizzazione dei soggetti]]
- [[concepts/Specifiche tecniche di base]]
- [[concepts/Sanzioni NIS2]]
- [[concepts/Strategia nazionale di cybersicurezza]]
- [[concepts/Piattaforma digitale ACN]]
- [[concepts/Clausola di salvaguardia]]
- [[concepts/Coordinated Vulnerability Disclosure]]
- [[concepts/Responsabilità degli organi di gestione]]

Synthesis (1):
- [[synthesis/Cronologia attuativa NIS2 in Italia]]

Pagine aggiornate:
- [[index]] — riempito con i contatori e i cataloghi della Wave 1.

Note:
- Le 9 autorità di settore italiane sono trattate **collettivamente** in [[entities/Autorità di settore NIS]] + entità autonoma per [[entities/Ministero della Difesa]] (per il suo ruolo speciale su crisi cyber). Promozione individuale degli altri 8 ministeri rinviata alla Wave 4 (FAQ ACN settoriali) o quando emergeranno informazioni specifiche.
- File `_tmp/01_direttiva_ue.txt`, `_tmp/02_decreto138.txt`, `_tmp/03_normativa_acn.txt` mantenuti per consultazione cross-reference durante le Wave successive. Cleanup possibile a fine Wave 5.
- Lacune note (segnalate nelle pagine "Note dell'agente"): attese specifiche tecniche dalle determinazioni ACN (Wave 2) per soglie incidente, regime transitorio NIS1→NIS2, rapporto NIS2/perimetro D.Lgs. 105/2019, traduzione concreta della responsabilità del board per soggetti con governance dualistica e per PA.

Prossimo passo previsto: review da Andrea, poi **Wave 2 — 8 determinazioni ACN** (atti tecnici di dettaglio del Direttore generale ACN).

## [2026-04-29] ingest | Wave 2 — Determinazioni ACN [chiusa]
Fonti elaborate (8):
- `_tmp/04_det_tavolonis_funzionamento.txt` — det. funzionamento Tavolo NIS (16/07/2025, prot. 276206)
- `_tmp/05_det_comptavolo.txt` — det. composizione Tavolo NIS (sost. Vinciguerra MEF)
- `_tmp/06_det_gestione_incidenti.txt` — Linee Guida NIS gestione incidenti (dic 2025, v1.1 apr 2026)
- `_tmp/07_det_categorizzazione.txt` — det. categorizzazione (13/04/2026)
- `_tmp/08_det_terminisoggetti2026.txt` — det. termini soggetti 2026 (n. 127434/2026)
- `_tmp/09_det_accordicondivisione.txt` — det. accordi di condivisione (10/04/2025)
- `_tmp/10_det_obblighi.txt` — det. specifiche di base n. 379907/2025 (19/12/2025)
- `_tmp/11_det_piattaforma.txt` — det. piattaforma e procedure (13/04/2026)

Pagine create (28):

Sources (8):
- [[sources/Determinazione ACN funzionamento Tavolo NIS - 2025-07-16]]
- [[sources/Determinazione ACN composizione Tavolo NIS - 2026]]
- [[sources/Linee Guida NIS - Gestione incidenti - 2025-12]]
- [[sources/Determinazione ACN categorizzazione - 2026-04-13]]
- [[sources/Determinazione ACN termini soggetti 2026 - 2026-04-30]]
- [[sources/Determinazione ACN accordi condivisione - 2025-04-10]]
- [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]]
- [[sources/Determinazione ACN piattaforma e procedure - 2026-04-13]]

Entities (5 nuove):
- [[entities/Punto di contatto NIS]]
- [[entities/Referente CSIRT]]
- [[entities/Rappresentante NIS in Italia]]
- [[entities/Framework Nazionale per la Cybersecurity]]
- [[entities/NIST SP 800-61]]

Concepts (15 nuovi):
- [[concepts/Misure di sicurezza di base]]
- [[concepts/Incidenti significativi di base]]
- [[concepts/Categorie di rilevanza]]
- [[concepts/Macro-aree NIS]]
- [[concepts/Accordi di condivisione delle informazioni]]
- [[concepts/Fornitori rilevanti NIS]]
- [[concepts/Verifiche di coerenza]]
- [[concepts/Verifiche di conformità categorizzazione]]
- [[concepts/Aggiornamento annuale informazioni]]
- [[concepts/Aggiornamento continuo informazioni]]
- [[concepts/Regime transitorio OSE]]
- [[concepts/Regime transitorio telco]]
- [[concepts/Soggetti PSNC-NIS]]
- [[concepts/Processo gestione incidenti NIS]]
- [[concepts/Coordinamento DORA-NIS]]

Pagine aggiornate (10 esistenti + index):
- [[entities/ACN]] — corpo determinazioni 2025-2026 + linee guida + piattaforma
- [[entities/CSIRT Italia]] — referente CSIRT, linee guida gestione incidenti
- [[entities/Tavolo per l'attuazione della disciplina NIS]] — funzionamento operativo (convocazione/quorum/durata) + composizione aggiornata + salvaguardia DORA
- [[concepts/Identificazione dei soggetti NIS]] — calendario annuale completo + termini coorte 2026
- [[concepts/Notifica di incidente significativo]] — incidenti significativi di base + soglie telco + processo IR + termini avvio per coorte
- [[concepts/Misure di gestione del rischio cyber]] — det. 379907/2025 misure di sicurezza di base + termini coorte
- [[concepts/Categorizzazione dei soggetti]] — modello attuativo (10 macro-aree + 4 categorie) + automatismo PSNC + esonero DORA
- [[concepts/Specifiche tecniche di base]] — corpo regolamentare 2025-2026 (tabella) + concetti figli operativi
- [[concepts/Piattaforma digitale ACN]] — ruoli operativi + verifiche + finestra accordi condivisione
- [[concepts/Clausola di salvaguardia]] — salvaguardia DORA nel Tavolo + art. 12 det. piattaforma
- [[index]] — contatori 11 sources / 17 entities / 33 concepts / 1 synthesis, riorganizzato per cluster tematici

Note:
- Stato totale wiki dopo Wave 2: **11 sources, 17 entities, 33 concepts, 1 synthesis** (era 3/12/18/1).
- Decisione architetturale: **misure** e **incidenti significativi di base** creati come concetti distinti figli di [[concepts/Specifiche tecniche di base]] (concetto-ombrello mantenuto).
- Decisione architetturale: 4 ruoli operativi (pdc, referente CSIRT, rappresentante NIS) e 1 framework + 1 standard creati come entities.
- File `_tmp/04..11` mantenuti per consultazione cross-reference durante le Wave 3-5. Cleanup possibile a fine Wave 5.
- Lacuna nota: pagina **synthesis** dedicata alla **stratificazione delle norme cybersecurity in Italia** (PSNC + NIS2 + DORA + cloud PA + Legge 90/2024) — segnalata in [[concepts/Soggetti PSNC-NIS]] e [[concepts/Clausola di salvaguardia]]. Da considerare per Wave 5.

Prossimo passo previsto: review da Andrea, poi **Wave 3 — 6 allegati tecnici** (allegato-1-v2, allegato-2-v2, allegato-3-v2, allegato-4-v2, allegato_1_modello260409-v1, allegato_2_modello260409-v1).

## [2026-04-29] ingest | Wave 4 — FAQ ACN [chiusa]
Fonti elaborate (8):
- `Domande frequenti NIS - Profili generali - ACN.pdf` → [[sources/FAQ NIS - Profili generali]]
- `Domande frequenti NIS - Ambito - ACN.pdf` → [[sources/FAQ NIS - Ambito]]
- `Domande frequenti NIS - Settori, sottosettori e tipologie di soggetto - ACN.pdf` → [[sources/FAQ NIS - Settori, sottosettori e tipologie di soggetto]]
- `Domande frequenti NIS - Registrazione - ACN.pdf` → [[sources/FAQ NIS - Registrazione]]
- `Domande frequenti NIS - Ruoli e procedure - ACN.pdf` → [[sources/FAQ NIS - Ruoli e procedure]]
- `Domande frequenti NIS - Categorizzazione - ACN.pdf` → [[sources/FAQ NIS - Categorizzazione]]
- `Domande frequenti NIS - Misure di sicurezza e notifica di incidenti - ACN.pdf` → [[sources/FAQ NIS - Misure di sicurezza e notifica di incidenti]]
- `Domande frequenti NIS - Aggiornamento delle informazioni - ACN.pdf` → [[sources/FAQ NIS - Aggiornamento delle informazioni]]

Pagine create (8 source):
- 8 FAQ ACN sopra elencate (uno per cluster tematico).

Pagine aggiornate (Wave 2 — protocol numbers):
- [[sources/Determinazione ACN piattaforma e procedure - 2026-04-13]] — aggiunto **Det. ACN 127437/2026** (frontmatter, TL;DR, disposizioni finali, note dell'agente). Linea di successione: 333017/2025 → 379887/2025 → 127437/2026 (citato da `CAT.4` FAQ + `FRN.2-3` FAQ).
- [[sources/Determinazione ACN categorizzazione - 2026-04-13]] — aggiunto **Det. ACN 155238/2026** (frontmatter, TL;DR, bullet finestra annuale, note dell'agente). Confermato da `CAT.1`, `CAT.5`, `CAT.7`, `CAT.8`, `CAT.9` di FAQ Categorizzazione.

Pagine aggiornate (entities/concepts):
- [[entities/Punto di contatto NIS]] — riferimenti a FAQ Ruoli (`PDC.1-7`, `ODA.1-10`, `RR.1-3`) + FAQ Registrazione; chiarita catena tripartita CDA → pdc → referente CSIRT.
- [[entities/Referente CSIRT]] — riferimento a FAQ Ruoli (`RCS.1-6`, `RR.1-3`); esternalizzazione esplicita, sovrapposizione con pdc per piccoli soggetti, dialogo con CSIRT Italia in inglese.
- [[concepts/Fornitori rilevanti NIS]] — sezione "Tassonomia CPV (FAQ `FRN.2-4`)" con 3 cluster CPV (non-fungibili energia/connettività + ICT-infrastrutture digitali 8 categorie + ICT-servizi gestiti+sicurezza); citato art. 18 Det. 127437/2026.
- [[concepts/Coordinamento DORA-NIS]] — sezione "Chiarimento ambito (FAQ Ambito `AMB.NO.2`)" — entità DORA = soggetti NIS solo per Allegato I p. 3-4 e con il solo art. 7 c. 1.
- [[concepts/Notifica di incidente significativo]] — sezione "Chiarimenti operativi (FAQ ACN)" rimanda a FAQ Misure+Notifica.
- [[concepts/Misure di sicurezza di base]] — sezione "Roadmap normativa misure" con 3 tappe (base → aggiuntive entro fine 2026 → lungo termine) ex `CAT.3`.
- [[concepts/Categorizzazione dei soggetti]] — sezioni "Processo suggerito (`CAT.7`)", "Coordinamento Cloud PA (`CAT.8`)", "Coordinamento PSNC (`CAT.9`)".
- [[concepts/Identificazione dei soggetti NIS]] — sezione "Chiarimenti operativi" + frontmatter sources allargato a 8 (4 originali + 4 FAQ).
- [[concepts/Aggiornamento annuale informazioni]] — sezione "Chiarimenti FAQ (`FRN.*` e altri)".
- [[concepts/Soggetti essenziali e importanti]] — frontmatter sources + FAQ Profili generali e Ambito.
- [[concepts/Settori altamente critici e critici]] — sezione "Chiarimenti operativi (FAQ ACN)" con NACE, size-blind, eccezioni di prevalenza, identificazione autoritativa Allegato IV, 13 servizi gestiti di sicurezza, doppia identità ASL.
- [[concepts/Categorie di rilevanza]] — sezione "Conferma ordinale (FAQ `CAT.6`)" con ordine crescente minimo→alto.
- [[index]] — contatori 17→25 sources, aggiornati N fonti per le 13 entity/concept page toccate, aggiunto cluster Wave 4.

Note:
- Stato totale wiki dopo Wave 4: **25 sources, 17 entities, 33 concepts, 1 synthesis** (era 17/17/33/1).
- Decisione architetturale: nessun nuovo concept o entity creato in Wave 4. Le FAQ aggiungono **chiarimenti operativi** che si annestano nelle pagine esistenti come sezione dedicata "Chiarimenti FAQ" o equivalente. Eventuali nuovi concetti (es. Roadmap normativa misure, Tipologie di soggetto, Servizi di sicurezza gestiti, Pubbliche amministrazioni NIS, Imprese collegate, Eccezioni di prevalenza, Organi di amministrazione e direttivi, Portale dei Servizi ACN, Autovalutazione NIS PDA1/2/3) restano da promuovere su esplicita richiesta di Andrea.
- **Conferma protocollo numbers (anchor)**: Wave 4 ha ancorato due numeri di protocollo precedentemente "lacuna nota": **155238/2026** (categorizzazione, citato in 5 FAQ) e **127437/2026** (piattaforma+procedure, citato in 3 FAQ). La linea di successione 333017/2025 → 379887/2025 → 127437/2026 è ora documentata.
- *Sintesi dell'agente:* Wave 4 ha confermato l'**architettura roadmap** delle misure NIS in 3 tappe (base / aggiuntive / lungo termine, ex `CAT.3`), che non era esplicita nelle determinazioni base. Da considerare per pagina synthesis dedicata in eventuale Wave 5.
- File `_tmp/faq_*.txt` mantenuti per consultazione cross-reference. Cleanup possibile a fine Wave 5.

Prossimo passo previsto: review da Andrea. Possibile **Wave 5** (lacune note non ancora coperte): pagina synthesis stratificazione norme cybersecurity IT (PSNC + NIS2 + DORA + Cloud PA + Legge 90/2024); pagina synthesis roadmap misure NIS (base → aggiuntive → lungo termine); promozione concetti citati nelle FAQ ma non ancora promossi (Tipologie di soggetto, Servizi gestiti, Servizi di sicurezza gestiti, Pubbliche amministrazioni NIS, Eccezioni di prevalenza, Organi di amministrazione e direttivi, Portale dei Servizi ACN, Autovalutazione NIS PDA1/2/3). Wave 5 da pianificare con Andrea.

## [2026-04-29] synthesis | Stratificazione delle norme cybersecurity in Italia
Pagina creata:
- [[synthesis/Stratificazione delle norme cybersecurity in Italia]] — risponde a "in quale regime ricade un soggetto e cosa deve fare?"; mappa i 5 regimi (PSNC, NIS2, DORA, Cloud PA, L. 90/2024); matrice di intersezione su 9 tipi di soggetto; punti di coordinamento normativo concreti (rinvii, esoneri, automatismi); decision tree pratico; tensioni e domande aperte.

Pagine aggiornate:
- [[concepts/Soggetti PSNC-NIS]] — backlink + rimossa "lacuna nota" (la synthesis copre il punto).
- [[concepts/Coordinamento DORA-NIS]] — backlink in Collegamenti.
- [[concepts/Clausola di salvaguardia]] — backlink + sostituita la "Sintesi dell'agente" con rinvio alla synthesis.
- [[index]] — Synthesis 1 → 2.

Note:
- Approvata da Andrea come unica pagina ad alto ROI tra le proposte Wave 5 (le altre — synthesis roadmap misure, promozione concetti minori — rinviate per evitare over-engineering).
- *Sintesi dell'agente:* la synthesis chiude formalmente la "lacuna nota" segnalata da Wave 2 (Soggetti PSNC-NIS, Clausola di salvaguardia). Stato wiki: 25 sources, 17 entities, 33 concepts, 2 synthesis.

## [2026-04-28] ingest | As We May Think — Vannevar Bush (1945) [DEMO — cancellata]
Fonte: `raw/articles/As We May Think — Vannevar Bush (1945).md`

Pagine create:
- [[sources/As We May Think — Bush 1945]] — pagina di sintesi della fonte
- [[entities/Vannevar Bush]] (nuova) — autore della fonte
- [[entities/Ted Nelson]] (nuova, stub) — coniatore di "hypertext"
- [[entities/Douglas Engelbart]] (nuova, stub) — NLS, ispirato da Bush
- [[entities/Tim Berners-Lee]] (nuova, stub) — Web, cita Bush
- [[entities/Belinda Barnet]] (nuova, stub) — critica accademica
- [[entities/The Atlantic Monthly]] (nuova, stub) — testata di pubblicazione
- [[entities/Office of Scientific Research and Development]] (nuova, stub) — contesto istituzionale di Bush
- [[concepts/Memex]] (nuovo) — dispositivo concettuale di Bush
- [[concepts/Trail associativi]] (nuovo) — innovazione centrale del Memex
- [[concepts/Ipertesto]] (nuovo) — concetto eredità del Memex
- [[concepts/Knowledge management]] (nuovo) — disciplina inquadrante

Pagine aggiornate:
- [[index]] — aggiornati contatori e cataloghi

Note:
- Ingest demo per mostrare il workflow. Rimovibile su richiesta di Andrea.
- Cifra "6.000 scienziati OSRD" segnata come da verificare con altre fonti.
- *Sintesi dell'agente* aggiunta sui collegamenti meta tra il Memex e il pattern LLM Wiki di questa wiki — segnalata esplicitamente come inferenza, non fatto della fonte.

## [2026-04-29] ingest | Wave 3 — Allegati tecnici (4 specifiche di base + 2 modelli categorizzazione) [chiusa]
Fonti elaborate (6):
- `raw/articles/allegato-1-v2.pdf` (allegati della det. 379907/2025: misure soggetti importanti)
- `raw/articles/allegato-2-v2.pdf` (misure soggetti essenziali)
- `raw/articles/allegato-3-v2.pdf` (incidenti significativi di base soggetti importanti)
- `raw/articles/allegato-4-v2.pdf` (incidenti significativi di base soggetti essenziali)
- `raw/articles/allegato_1_modello260409-v1.pdf` (modello categorizzazione art. 2 c. 2)
- `raw/articles/allegato_2_modello260409-v1.pdf` (modello categorizzazione art. 2 c. 3)

Pagine create (6 source):
- [[sources/Allegato 1 - Misure di sicurezza di base per i soggetti importanti]] — ~26 misure su 6 funzioni FNCDP/NIST CSF v2.0, Tabella 1 con 16 ambiti politiche, Tabella 2 con 6 requisiti non derogabili
- [[sources/Allegato 2 - Misure di sicurezza di base per i soggetti essenziali]] — strict super-set: +6 misure (`ID.AM-03`, `PR.AT-02`, `PR.PS-01`, `PR.PS-03`, `PR.IR-03`, `RC.CO-03`) + punti aggiuntivi (VA/PT obbligatori, test ripristino backup, hardening, monitoraggio canali fornitori SW critico)
- [[sources/Allegato 3 - Incidenti significativi di base per i soggetti importanti]] — 3 codici IS-1/2/3, soglie qualitative auto-determinate ancorate a `DE.CM-01`
- [[sources/Allegato 4 - Incidenti significativi di base per i soggetti essenziali]] — 4 codici (+IS-4 accesso non autorizzato/abuso privilegi su parametri quali-quantitativi `DE.CM-01` p.6)
- [[sources/Allegato 1 modello - Categorizzazione soggetti art. 2 c. 2]] — 10 macro-aree con categoria di rilevanza pre-assegnata (Logistica = basso)
- [[sources/Allegato 2 modello - Categorizzazione soggetti art. 2 c. 3]] — identico al modello 1 con UNICA differenza: Logistica = minimo

Pagine aggiornate (5 esistenti + index):
- [[concepts/Misure di sicurezza di base]] — architettura 6 funzioni, tabella misure per funzione (importanti vs essenziali), tabella 16 ambiti politiche, tabella 2 non derogabili, riesami obbligatori
- [[concepts/Incidenti significativi di base]] — tabella codici IS-1..4, aggancio operativo `DE.CM-01` (SL → IS-3, parametri quali-quantitativi → IS-4), rimossa "lacuna nota"
- [[concepts/Macro-aree NIS]] — tabella 10 macro-aree con categorie pre-assegnate per entrambi i modelli, descrizioni complete, evidenziato diff Logistica, rimossa "lacuna nota"
- [[concepts/Categorie di rilevanza]] — distribuzione categorie su entrambi i modelli
- [[entities/Framework Nazionale per la Cybersecurity]] — sezione 6 funzioni con prefissi codici (GV/ID/PR/DE/RS/RC) + esempi misure
- [[concepts/Specifiche tecniche di base]] — frontmatter sources allargato a 16, tabella corpo regolamentare con annidamento allegati
- [[index]] — contatori 17 sources / 17 entities / 33 concepts / 1 synthesis, aggiunto cluster Wave 3

Note:
- Stato totale wiki dopo Wave 3: **17 sources, 17 entities, 33 concepts, 1 synthesis** (era 11/17/33/1).
- Decisione architetturale: nessun nuovo concept o entity creato in Wave 3 — l'intero contenuto tabellare degli allegati è confluito nelle source page (loci tabellari unici) E nei concept page esistenti per consultazione rapida (per esplicita scelta di Andrea).
- Pattern di scrittura: ogni allegato di misure ha la propria tabella sintetica delle misure per funzione + Tabella 1 + Tabella 2 in chiaro. Ogni allegato incidenti ha la propria tabella IS. Ogni modello ha la propria tabella delle 10 macro-aree con categorie.
- File `_tmp/all1..4.txt` e `_tmp/mod1..2.txt` (estratti pdftotext) mantenuti per consultazione. Cleanup possibile a fine Wave 5.

Prossimo passo previsto: review da Andrea, poi **Wave 4 — 8 FAQ ACN** (Aggiornamento, Ambito, Categorizzazione, Misure+notifica, Profili generali, Registrazione, Ruoli+procedure, Settori).

## [2026-05-18] ingest | Wave 5 A1 — Guida alla lettura specifiche di base [chiusa]
Fonte elaborata:
- `raw/articles/guida-alla-lettura-specifiche-di-base.pdf` (ACN, settembre 2025, ed. corrente 2.1 aprile 2026; approvata dal Tavolo NIS il 10/04/2025) → [[sources/Guida lettura specifiche di base]]

Estratto in `_tmp/12_guida_lettura.txt` (1055 righe).

Decisione architetturale (concordata con Andrea prima di scrivere): **promozione di 3 nuovi concepts** (A/B/C) anziché solo aggiunte additive alle pagine esistenti. Motivazione: i tre concetti sono trasversali, ricorrono in misure/incidenti, e il loro spazio dedicato evita di gonfiare le pagine già consolidate. Posizionamento prima di Wave 5 A2 (FNCDP) per evitare rework futuro.

Pagine create (4):

Sources (1):
- [[sources/Guida lettura specifiche di base]]

Concepts (3 nuovi):
- [[concepts/Sistemi informativi e di rete rilevanti]] — scoping primario delle misure (clausola C1), processo a 3 step, elenco ex `GV.OC-04`
- [[concepts/Clausole basate sul rischio]] — le 4 clausole standardizzate (C1 rilevanti / C2 valutazione rischio `ID.RA-05` / C3 deroga motivata / C4 forniture rilevanti) con applicazione in cascata e mappatura completa requisiti→clausole (Appendice B guida)
- [[concepts/Evidenze documentali NIS]] — 6 tipologie documentali (elenchi/inventari/piani/politiche/procedure/registri) + i **11 documenti che richiedono delibera degli organi di amministrazione** (Appendice C guida)

Pagine aggiornate (10 esistenti + index):
- [[concepts/Misure di sicurezza di base]] — **fix conteggi**: ~26/~32 → **37/87 importanti, 43/116 essenziali** (decomposizione esatta del super-set); aggiunte sezioni "Approccio basato sul rischio — 4 clausole", "Tipologia requisiti (organizzativi vs tecnologici)", "Evidenze documentali"
- [[concepts/Incidenti significativi di base]] — nuova sezione **"Modello tridimensionale dell'incidente"** (condizione / compromissione / oggetto compromissione), esempi canonici di compromissione, canali di acquisizione dell'evidenza, conferma multi-rischio (anche eventi accidentali)
- [[concepts/Misure di gestione del rischio cyber]] — nuova sezione **"Mappatura art. 24 c.2 → codici misure di sicurezza di base"** (Appendice A guida, "stele di Rosetta" norma astratta ↔ codici tecnici)
- [[concepts/Responsabilità degli organi di gestione]] — nuova sezione **"Gli 11 documenti che richiedono approvazione del board"** (lista esatta con codice requisito); rimossa nota agente "lacuna nota su declinazione concreta art. 23"
- [[concepts/Specifiche tecniche di base]] — sezione Linee Guida riorganizzata; **fix conteggi** ~26/32 → 37/43 + 87/116; sources allargati a 17
- [[concepts/Notifica di incidente significativo]] — chiarimento sul momento di decorrenza dei termini (evidenza acquisita = inizio 24h/72h)
- [[concepts/Approccio multi-rischio]] — conferma su incidenti accidentali notificabili (§ 3.1 guida)
- [[entities/Framework Nazionale per la Cybersecurity]] — sources allargati; conferma denominazione FNCDP edizione 2025; lacuna nota su contenuto preciso del Core riformulata (ingest FNCDP A2 prossimo)
- [[entities/ACN]] — guida menzionata come pubblicazione tra le Linee Guida
- [[entities/Tavolo per l'attuazione della disciplina NIS]] — registrata approvazione del 10/04/2025
- [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]] — callout che indirizza alla guida come meta-documento interpretativo
- [[sources/Allegato 1 - Misure di sicurezza di base per i soggetti importanti]] — fix conteggi ~26/~32 → 37/87
- [[sources/Allegato 2 - Misure di sicurezza di base per i soggetti essenziali]] — fix conteggi → 43/116; riga "Requisiti totali" nella tabella di confronto
- [[sources/Allegato 3 - Incidenti significativi di base per i soggetti importanti]] — riferimento alla guida § 3 (modello tridimensionale)
- [[sources/Allegato 4 - Incidenti significativi di base per i soggetti essenziali]] — riferimento alla guida § 3
- [[index]] — sources 25→26, concepts 33→36, contatori N fonti aggiornati per le pagine toccate, aggiunto cluster Wave 5

Note:
- Stato totale wiki dopo Wave 5 A1: **26 sources, 17 entities, 36 concepts, 2 synthesis** (era 25/17/33/2).
- **Errata corrige importante**: i conteggi delle misure ("~26 importanti, ~32 essenziali") erano stati estratti per ispezione dalle PDF degli allegati nella Wave 3 e si rivelavano inesatti. La guida fissa la cifra autoritativa: **37 misure / 87 requisiti** per gli importanti, **43 misure / 116 requisiti** per gli essenziali. Tutte le occorrenze nelle pagine wiki sono state allineate.
- **Architettura aggregativa**: i 3 nuovi concept funzionano come "vocabolario operativo" delle specifiche di base. Future ingest di FAQ o linee guida settoriali aggiorneranno questi concept invece di stratificare contenuto in pagine già grandi.
- *Sintesi dell'agente:* la guida è il **meta-documento più importante** del corpo regolamentare NIS italiano insieme alla det. 379907 stessa. Senza di essa la determinazione è leggibile ma non operativa.
- File `_tmp/12_guida_lettura.txt` mantenuto per cross-reference durante Wave 5 A2/A3.

Prossimo passo previsto: ingest **Wave 5 A2** — `FNCDP_-_Edizione_2025_v2.1_-_Core.pdf` (chiude la "lacuna nota" su contenuto preciso del Framework Nazionale citata in [[entities/Framework Nazionale per la Cybersecurity]]). Su cue di Andrea.

## [2026-05-18] ingest | Wave 6 — Cluster A: Reg. UE 2024/2690 + scope tagging system [chiuso]
Cambiamenti di sistema:
- Introdotto **scope tagging** in tutto il frontmatter: ogni nodo ora carry `scope:` (`nis2_tool` / `grc_personal` / `both`). Serve a separare il knowledge base del NIS2 Self-Assessment Tool (open source, pilot Energia/Cloud/PA) dal GRC personale di Andrea (ISO 27001 LA prep, ecc.) senza ristrutturare le cartelle.
- Creata cartella `_meta/` con `wave_reports/` per i report iterativi dei wave e `skipped_documents.md` per le decisioni di skip motivate.
- Creata cartella `raw/_archive/` per file ridondanti o sostituiti.

Documenti del Cluster A (2 di 13 del batch 2026-05-18):
- `CELEX_32022L2555_IT_TXT.pdf` → **duplicato** della Direttiva NIS2 già in wiki ([[sources/Direttiva (UE) 2022-2555 (NIS2)]]). Rinominato con suffisso `_DUPLICATE` e spostato in `raw/_archive/`. Nessun nodo creato.
- `OJ_L_202402690_IT_TXT.pdf` → **Regolamento di esecuzione (UE) 2024/2690** della Commissione del 17/10/2024. Ingerito.

Documenti skippati nel batch:
- `acn-lanuovadirettivanis-sapienza-20241127.pdf` (Cluster A3 ex-Wave 5) → skip definitivo, vedi [[_meta/skipped_documents]].

Pagine create (2):

Sources (1):
- [[sources/Regolamento di esecuzione UE 2024-2690]] — `scope: nis2_tool`. Atto UE direttamente applicabile (entrata in vigore 07/11/2024) ex art. 21 par. 5 + art. 23 par. 11 NIS2. 11 categorie DSP (DNS, TLD, cloud, data center, CDN, MSP, MSSP, marketplace, search, social, trust services). Criteri orizzontali (art. 3) + criteri specifici per tipo (artt. 5-14). Allegato in 13 sezioni mappate uno-a-uno sulle lettere dell'art. 21 par. 2 NIS2. Fonti tecniche esplicite: ISO/IEC 27001, ISO/IEC 27002, ETSI EN 319 401, CEN/TS 18026:2024. Abroga Reg. UE 2018/151 (NIS1).

Synthesis (1):
- [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]] — `scope: nis2_tool`. **Deliverable critico del wave**: risolve (parzialmente) la domanda di rapporto regolatorio tra atto UE direttamente applicabile e specifica nazionale ACN per i fornitori cloud italiani. Tesi 3a+3c (applicazione cumulativa con primato UE su conflitti); 5 open question normative esplicitate; avvertenza testuale per il verdetto pilot Cloud del NIS2 Tool.

Pagine aggiornate (29 — solo frontmatter `scope:`):

Sources (8): Direttiva NIS2, D.Lgs. 138/2024, Pagina ACN, Det. specifiche di base 379907, Allegati 1-4, Guida lettura → tutti `scope: both`.

Concepts (19): NIS2, Ambito applicazione, Settori, Soggetti ess./imp., Identificazione, Categorizzazione, Categorie di rilevanza, Incidente significativo, Notifica, Specifiche tecniche di base → `both`; Misure rischio cyber, Misure di sicurezza di base, Incidenti significativi di base, Approccio multi-rischio, Sistemi rilevanti, Clausole rischio, Evidenze documentali, Responsabilità organi, Coordinamento DORA-NIS → `grc_personal`.

Entities (4): ACN, ENISA, CSIRT Italia, Gruppo di Cooperazione NIS → `both`.

Synthesis (2 esistenti): Cronologia + Stratificazione → `both`.

Note:
- Stato totale wiki dopo Wave 6 Cluster A: **27 sources, 17 entities, 36 concepts, 3 synthesis** (era 26/17/36/2).
- Open question normativa principale segnalata: rapporto Reg. UE 2024/2690 ↔ Det. ACN 379907/2025 sulle misure (sui criteri di significatività incidenti il Reg. UE è esaustivo ex cons. 30). Da risolvere con consulenza GRC + monitoring guidance ENISA/ACN.
- I cluster B/C/D/E/F del batch 2026-05-18 sono in **pausa** in attesa di review umana della synthesis (come da brief).
- File `_tmp/13_reg_ue_2024_2690.txt` mantenuto per consultazione.
- Wave report dettagliato: [[_meta/wave_reports/Wave_6_2026-05-18]].

Prossimo passo previsto: **pausa per human review** della synthesis. Su cue di Andrea, resume del Cluster B (ENISA — 4 documenti) o ordine alternativo.

## [2026-05-18] ingest | Wave 6 — Cluster B Sessione 1: ENISA TIG v1.0 + Mapping Table + Q1-Q4 follow-up [chiusa]
Documenti del Cluster B trattati (2 di 4):
- `ENISA_Technical_implementation_guidance_on_cybersecurity_risk_management_measures_version_1.0.pdf` — TIG v1.0 di giugno 2025 (170 pp, soft-law, ENISA + Commissione + NIS Cooperation Group). Verifica pre-ingest: identità confermata, struttura mappata uno-a-uno sull'Allegato Reg. 2024/2690 (13 capitoli).
- `ENISA_Technical_Implementation_Guidance_Mapping_table_version_1.0.pdf` — Mapping Table v1.0. Pre-ingest check: PDF v1.7 testuale (no scan); struttura tabellare appiattita = conversione lossy del file `.xlsx` ufficiale ENISA. Action item: scaricare il `.xlsx` per uso operativo.

Razionale della sessione: la TIG è guidance interpretativa del Reg. UE 2024/2690; una sua lettura mirata può chiudere/ridurre le 4 open question (Q1-Q4) della synthesis di coordinamento prima della review pre-launch del consulente GRC esterno per il NIS2 Tool pilot Cloud.

Pagine create (3):

Sources (2):
- [[sources/ENISA Technical Implementation Guidance v1.0 - 2025-06-26]] — `scope: grc_personal`. TIG completa con disclaimer, 13 capitoli, 10 topic-specific policies elencate, esempi di guidance, caveat di soft-law e di non-equivalenza standard.
- [[sources/ENISA Mapping Table v1.0 - 2025-06-26]] — `scope: grc_personal`. Mapping verso ISO 27001:2022, NIST CSF 2.0, ETSI EN 319 401, CEN/TS 18026:2024, national frameworks. Nota di provenance (PDF lossy, xlsx ufficiale).

Synthesis (1 — deliverable critico):
- [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]] — `scope: nis2_tool`. Analisi sezione per sezione delle 4 Q della synthesis di coordinamento. Conclusione: tutte e 4 le Q sono **ristrette** (non chiuse, per vincolo soft-law TIG); tesi 3a + 3c della synthesis di coordinamento confermata.

Pagine aggiornate:
- [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]] — aggiunte note *"Risposta TIG ENISA: ristretta..."* a ciascuna Q1-Q4 + rinvio al nuovo synthesis nodo. Action items aggiornato. **Non modificati**: callout della tesi (3a+3c+scarto 3b), avvertenza testuale pilot Cloud, Sintesi tabellare.
- [[_meta/wave_reports/Wave_6_2026-05-18]] — sezione "Cluster B Sessione 1" aggiunta con esito pre-ingest, deliverable Q1-Q4, action items, distribuzione scope.
- [[index]] — sources 27→29, synthesis 3→4, cluster B Sessione 1 annotato.

Note:
- Stato totale wiki dopo Sessione 1: **29 sources, 17 entities, 36 concepts, 4 synthesis** (era 27/17/36/3).
- Scope distribution dei nodi creati: 1 `nis2_tool` (Risposta Q1-Q4) + 2 `grc_personal` (TIG + Mapping Table).
- **Risultato critico**: la TIG ENISA conferma esplicitamente la tesi 3a (cumulazione UE+IT) tramite disclaimer di non-sostituzione dei framework nazionali. Q1-Q4 ristrette. Review consulente GRC parte ora da posizione più solida.
- *Sintesi dell'agente:* la sessione dimostra il valore del workflow "ingest reattivo a synthesis aperte": le 4 open question della synthesis di coordinamento hanno guidato la lettura mirata della TIG (170 pp lette in modo orientato anziché esaustivo), producendo un nodo follow-up di alto valore in poche ore.
- File `_tmp/14_enisa_tig.txt` e `_tmp/15_enisa_mapping.txt` mantenuti per consultazione.

Prossimo passo previsto: **pausa per human review** prima del Cluster B Sessione 2 (NIS2↔ECSF mapping + ECSF Role Profiles). Su cue di Andrea.

## [2026-05-19] ingest | Wave 6 — Cluster B+C+D Sessione 2: NIST CSF 2.0 + ISO 27000/27001/27002 + synthesis Cross-walk v1 [chiusa]
Documenti del batch trattati (4 di 9 rimanenti):
- `NIST.CSWP.29.pdf` → NIST CSF 2.0 (NIST CSWP 29 del 26/02/2024). Pre-ingest verification PASSED.
- `[ISO_IEC 27000_2018]...pdf` (copia non ufficiale) → ISO/IEC 27000:2018 (5th edition). Pre-ingest verification PASSED. Standard liberamente disponibile sul sito ISO ITTF.
- `ISO_IEC 27001_2022_...pdf` (copia non ufficiale) → ISO/IEC 27001:2022 (3rd edition 2022-10). Pre-ingest verification PASSED.
- `ISO IEC 27002 ...pdf` (copia non ufficiale) → ISO/IEC 27002:2022 (3rd edition 2022-02). Pre-ingest verification PASSED — verificate edizione, 93 controlli in 4 themes, 5 attributi, tutti gli 11 controlli nuovi rispetto a 27002:2013.

Razionale della sessione: NIST CSF 2.0 e ISO 27001/27002 sono il riferimento di base internazionale per la transizione GRC e ISO 27001 Lead Auditor prep. La wiki deve poterli citare per ID di clausola/funzione/sottocategoria. NIST CSF 2.0 letto prima per fornire la fonte upstream del FNCDP italiano (pending Sessione 3).

Pagine create (5):

Sources (4):
- [[sources/NIST CSF 2.0 - 2024-02-26]] — `scope: grc_personal`. NIST CSWP 29, dominio pubblico. 6 funzioni con focus su GOVERN (novità v2.0). Sezione "Confronto con FNCDP italiano" placeholder per Sessione 3.
- [[sources/ISO IEC 27000-2018]] — `scope: grc_personal`. Vocabolario ISMS. Provenance speciale (publicly available).
- [[sources/ISO IEC 27001-2022]] — `scope: grc_personal`. Requirements ISMS certificabile. Provenance non ufficiale (copia non ufficiale) con politica di citazione per ID di clausola/controllo.
- [[sources/ISO IEC 27002-2022]] — `scope: grc_personal`. 93 controlli in 4 themes con 5 attributi. Provenance idem 27001.

Synthesis (1):
- [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - ISO 27002]] — `scope: grc_personal`. **v1** con placeholder esplicito per FNCDP (sezione 5 del cross-walk pending Sessione 3). Cross-walk mappato sulle 13 sezioni dell'Allegato Reg. UE 2024/2690 con 3 pattern di lettura.

Micro-fix eseguiti:
- **M1 — Mapping Table versioning**: chiarito che "v1.7" osservato in Sessione 1 era la specifica del formato PDF (ISO 32000-1:2008), non la versione del documento ENISA (che è v1.0). Aggiunta sezione "## Versioning" nel nodo `sources/ENISA Mapping Table v1.0 - 2025-06-26.md`. Nessuna rinomina necessaria.
- **M2 — Citazioni TIG in synthesis Q1-Q4**: 15 citazioni inglesi ridotte a esattamente 4 (1 per Q), tutte <15 parole. Le 11 citazioni sostituite con paraphrasi italiane mantenendo riferimenti puntuali alle sezioni TIG.

Pagine aggiornate:
- [[sources/ENISA Mapping Table v1.0 - 2025-06-26]] — sezione "## Versioning" aggiunta (esito M1).
- [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]] — citazioni revisionate (esito M2). Contenuto sostanziale invariato.
- [[_meta/wave_reports/Wave_6_2026-05-18]] — sezione "Cluster B+C+D Sessione 2" aggiunta.
- [[index]] — sources 29→33, synthesis 4→5, cluster B+C+D Sessione 2 annotata.

Note:
- Stato totale wiki dopo Sessione 2: **33 sources, 17 entities, 36 concepts, 5 synthesis** (era 29/17/36/4).
- Scope distribution dei nodi creati: 0 `nis2_tool` + 5 `grc_personal` (4 sources + 1 synthesis).
- **Pre-ingest verification protocollo rigoroso applicato**: tutti e 4 i file ISO/NIST verificati per edizione/versione prima dell'ingest. Nessun mismatch rilevato (a differenza del precedente noto in cui un file etichettato `ISO27001.pdf` era 27002:2005).
- *Sintesi dell'agente:* la sessione produce **due asset critici** per la transizione GRC di Andrea: (1) le 3 source ISO + la NIST CSF danno tutto il riferimento di base per ISO 27001 Lead Auditor prep, (2) la synthesis di cross-walk è il *core skill* del consulente GRC italiano nel contesto NIS2 (tradurre tra norme, framework outcome-based, standard control-based).
- File `_tmp/16_nist_csf.txt`, `_tmp/17_iso_27000.txt`, `_tmp/18_iso_27001.txt`, `_tmp/19_iso_27002.txt` mantenuti per consultazione.

Prossimo passo previsto: **pausa per human review** prima della Sessione 3 (FNCDP 2025 v2.1 + ECSF Role Profiles + NIS2↔ECSF mapping; aggiornamento synthesis cross-walk a v2). Su cue di Andrea.

## [2026-05-19] ingest | Wave 6 — Cluster B+E Sessione 3: FNCDP 2025 v2.1 + ECSF + Mapping NIS2-ECSF + Cross-walk v2 + Profili ECSF [chiusa]

Esecuzione in ordine task non negoziabile (Task 0 → Task 1 → Task 2):

**Task 0 — Audit Sessione 2 (priorità top)**: ✅ tutti i nodi della Sessione 2 PASSED. Il bug di duplicazione riportato in human review NON è confermato sul filesystem. Diagnosi: errore di display nel canale chat, non bug strutturale. Filesystem integro.

**Task 1 — FNCDP 2025 v2.1 + Cross-walk v2**: pre-ingest verification 5 questioni eseguita (Q1-Q4 confermate, Q5 negativa — FNCDP non cita NIS2). Nuovo source FNCDP `scope: grc_personal`. Entity Framework Nazionale aggiornato a `scope: both` con contenuti specifici v2.1, lacuna nota chiusa. Cross-walk synthesis rinominato e portato a v2: aggiunta tabella sommaria delta DP-* + Differenza chiave 4 (Data Protection italiana) + aggiornamento Differenza chiave 2 (GOVERN confermata in FNCDP).

**Task 2 — ECSF Role Profiles + Mapping NIS2-ECSF**: 2 source nodes ENISA (CC-BY 4.0). Synthesis discrezionale "Profili ECSF per il consulente GRC NIS2 italiano" emersa naturale (scope: grc_personal, tripletta consigliata + roadmap certificazioni 24-36 mesi). Audit citazioni inglesi: 2 citazioni totali, 11 + 9 parole, entrambe <15 → PASSED.

Pagine create (5):

Sources (3):
- [[sources/FNCDP 2025 v2.1 Core]] — `scope: grc_personal`. Verifica delle ipotesi del cross-walk v1: 4/5 confermate, Q5 negativa. 9 sottocategorie DP-* + 1 categoria nuova DP-ID.DM.
- [[sources/ECSF Role Profiles - 2022-09]] — `scope: grc_personal`. 12 profili ECSF; CC-BY 4.0.
- [[sources/ENISA Mapping NIS2 obligations with ECSF role profiles - 2025-06-26]] — `scope: grc_personal`. Mapping obblighi NIS2 art. 21/23 ↔ 12 profili ECSF + 2 use cases.

Synthesis (1 nuovo + 1 aggiornato a v2):
- [[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]] — **nuovo**, `scope: grc_personal`. Tripletta consigliata: Cyber Legal/Policy/Compliance Officer + Auditor + Risk Manager. Roadmap 24-36 mesi.
- [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] — **rinominato/aggiornato da v1 a v2**. Conferma ipotesi v1 (FNCDP ≡ NIST CSF nei codici); aggiunta tabella sommaria DP-* + Differenza chiave 4 (Data Protection italiana).

Pagine aggiornate:
- [[entities/Framework Nazionale per la Cybersecurity]] — `scope: both`, contenuti v2.1 popolati, lacuna nota chiusa.
- [[_meta/wave_reports/Wave_6_2026-05-18]] — sezione Cluster B+E Sessione 3 aggiunta.
- [[index]] — sources 33→36, synthesis 5→6.

Note:
- Stato totale wiki dopo Sessione 3: **36 sources, 17 entities, 36 concepts, 6 synthesis** (era 33/17/36/5).
- Scope distribution dei nodi creati: 0 `nis2_tool` + 4 `grc_personal` (FNCDP + ECSF + Mapping NIS2-ECSF + synthesis Profili ECSF) + 0 nuovi `both` (l'entity FNCDP aggiornata da `both` resta `both`).
- **Cluster B, C, D completati** in Wave 6. Cluster E parzialmente (FNCDP ✅; pending Strategia + Misura #82).
- File `_tmp/20_fncdp.txt`, `_tmp/21_ecsf.txt`, `_tmp/22_nis2_ecsf.txt` mantenuti per consultazione.

Prossimo passo previsto: **pausa per human review** prima della Sessione 4 (ACN Strategia + Manuale Misura #82 + Stress Test Handbook verifica autore). Su cue di Andrea.

## [2026-05-19] housekeeping | Wave 6 mini-sessione — 6 fix su Cross-walk v2 e Profili ECSF [chiusa]

Mini-sessione cosmetica/di precisione su due nodi `grc_personal` prodotti in Sessione 3, dopo human review.

**Cross-walk v2** ([[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]]):
- Fix 1: rinumerazione Differenze chiave 3↔4 (Data Protection ora 3, SoA ora 4 — ordine fisico-numerico coerente; backlinks check: nessuno).
- Fix 2: riferimento normativo "D.Lgs. 196/2003" sostituito con "Codice della privacy (D.Lgs. 196/2003 come novellato dal D.Lgs. 101/2018)".
- Fix 3: caveat di lettura aggiunto nelle Note dell'agente per la riga `DP-ID.DM-01..05` — la collocazione "Sez. 12 + Sez. 1" è inferenza dell'agente, non citazione del Reg. UE.

**Profili ECSF** ([[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]]):
- Fix 4: percorso ISO 27001 LA riformulato a **tre tappe** (corso + audit experience + registrazione registro auditor) con tempistiche puntuali per Andrea.
- Fix 5: tariffe attese spaccate in due livelli temporali (ingresso €400-700 mesi 12-24; scaling €700-1.000 mesi 24-36+) + caveat tariffario nelle Note dell'agente.
- Fix 6: **verifica normativa Punto di Contatto NIS eseguita**. Esito: **INTERNO OBBLIGATORIO** (FAQ Ruoli `ODA.1-10`, "esternalizzazione vietata"; nodo [[entities/Punto di contatto NIS]] documenta puntualmente). Paragrafo "Implicazione per Andrea" riformulato: il consulente esterno non può essere PdC, ma può supportare il PdC interno tramite l'avvalimento di personale esterno (art. 4 det. ACN piattaforma).

Wave report aggiornato con sezione "Mini-sessione housekeeping" che documenta i 6 fix.

Stato wiki: invariato (modifiche in-place). **36 sources, 17 entities, 36 concepts, 6 synthesis**.

Prossimo passo previsto: **pausa per human review** prima della Sessione 4. Su cue di Andrea.

## [2026-05-19] mini-fix | Wave 6 — Rinforzo direzionalità FNCDP in synthesis di coordinamento [chiuso]

Mini-fix su singolo bullet di [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]], razionale (ii) del callout tesi 3a+3c. Integrato il risultato della verifica Q5 di Sessione 3 (FNCDP non cita NIS2/Reg. UE/det. ACN): l'aggancio normativo è **monodirezionale**, conferma di *adozione complementare* (non *negoziata*, non *sostitutiva*) dello Stato italiano sul FNCDP come fonte tecnica.

Verifica coerenza Sintesi tabellare + Action items: invariati (entrambi già allineati con la tesi 3a+3c).

Vincoli rispettati: nessuna modifica al callout della tesi (3a+3c, scarto 3b), all'avvertenza testuale per pilot Cloud, al Punto 1, Punto 1-bis (art. 4 NIS2), Punto 2, Punto 4. Solo razionale (ii) del Punto 3 integrato.

Stato wiki: invariato. **36 sources, 17 entities, 36 concepts, 6 synthesis**.

Prossimo passo previsto: **pausa per human review** prima di Sessione 4 o altri deliverable. Su cue di Andrea.

## [2026-05-19] mini-fix | Wave 6 — Riformulazione avvertenza testuale pilot Cloud [chiusa]

Avvertenza testuale del verdetto pilot Cloud nella synthesis [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]] riformulata in sessione collaborativa con Andrea. La sezione era stata esplicitamente protetta nei prompt precedenti per consentire questa riformulazione collaborativa.

Sei cambiamenti applicati (da v1 ~95 parole a v2 ~280 parole):
1. Formulazione difensiva del rientro ("l'analisi suggerisce che... rientri" anziché "il tuo soggetto rientra").
2. Obblighi esplicitati su tre piani: misure tecniche + governance art. 23 D.Lgs. 138/2024 + notifica con tempistiche 24h/72h/1 mese.
3. Riferimenti normativi puntuali: artt. 3 e 7 Reg. UE + art. 23 D.Lgs. 138/2024 + termine "unionale".
4. Soglie quantitative concrete: Reg. UE sostituisce det. ACN per i fornitori cloud sui criteri di significatività incidenti.
5. Nuovo paragrafo "Attenzione" sui regimi italiani correlati possibili (PSNC, DORA, Cloud PA), segnalati come esistenti ma non analizzati dal tool.
6. Chiusura riformulata: "consulente qualificato in normativa cybersecurity italiana" anziché "consulente specializzato in compliance NIS2".

Verifica coerenza con la knowledge base eseguita prima del fix — tutti e 6 i cambiamenti coerenti con: source Reg. UE 2024/2690 (artt. 3/7 verificati in pre-ingest), concepts/Responsabilità degli organi di gestione (art. 23 D.Lgs. 138/2024 = base giuridica esatta), concepts/Notifica di incidente significativo (tempistiche 24h/72h/1m), Sintesi tabellare del nodo (riga 134 già allineata), synthesis/Stratificazione delle norme cybersecurity in Italia (regimi correlati). Backlink a Stratificazione già presente in Collegamenti — nessuna aggiunta.

Vincoli rispettati: callout della tesi (3a+3c, scarto 3b), Punto 1, Punto 1-bis, Punto 2, Punto 3 (corpo + razionale (ii) appena rinforzato), Punto 4, Conseguenze operative, Sintesi tabellare, Tensioni/contraddizioni, Domande aperte Q1-Q5, Action items, Note dell'agente — tutti invariati.

Status: pronto per pre-launch gate (review consulente GRC esterno).

Stato wiki: invariato (modifica in-place). **36 sources, 17 entities, 36 concepts, 6 synthesis**.

Prossimo passo previsto: **pausa per human review** prima di Sessione 4 o altri deliverable. Su cue di Andrea.

## [2026-05-19] retrofit | Wave 6.5 — Tagging `scope:` su 46 nodi pre-esistenti [chiusa]

Esecuzione completa del retrofit `scope:` (pianificata post cluster B-F di Wave 6, anticipata su decisione di Andrea). 6 passate tematiche eseguite in ordine: determinazioni ACN + modelli (8), FAQ ACN (8), concepts procedurali/ambito (15), concepts post-verdetto (1), entities (12), residui (2). Totale: **46 nodi retrofittati**.

Distribuzione finale (95 nodi totali):
- `both`: 63 nodi (66%) — citati o richiamati dal NIS2 Tool nell'esito preliminare
- `grc_personal`: 29 nodi (31%) — strumento per il consulente GRC post-verdetto
- `nis2_tool`: 3 nodi (3%) — esclusivamente del NIS2 Tool (Reg. UE 2024/2690 + 2 synthesis di Wave 6: Coordinamento UE-IT, Risposta TIG Q1-Q4)

Casi ambigui in esecuzione: 0 (pre-classificazione del brief ha eliminato la discrezionalità). Errori fattuali rilevati nei body: 0. Nessuna open question prodotta.

Verifica finale eseguita via grep: **0 nodi senza scope, 95/95 taggati**.

**Status**: script di export filtrato per Project Knowledge del NIS2 Tool ora eseguibile in modo affidabile. Wiki coerente.

Wave report dettagliato: [[_meta/wave_reports/Wave_6_5_2026-05-19]].

Stato wiki: invariato per contatori (i fix sono solo frontmatter). **36 sources, 17 entities, 36 concepts, 6 synthesis**.

Prossimo passo previsto: **pausa per human review** prima di Sessione 4 di Wave 6 (Cluster E residuo + Cluster F) o altri deliverable. Su cue di Andrea.

## [2026-05-19] ingest | Wave 6 — Cluster E (residuo) + F Sessione 4: ACN Strategia + Manuale Misura #82 + ENISA Stress Test [chiusa] — **WAVE 6 COMPLETED**

Sessione 4 di chiusura Wave 6. 3 documenti residui del batch 2026-05-18 gestiti.

**Pre-ingest verification**:
- `ACN_Strategia.pdf` (14.3 MB): PDF scansionato/immagine, 0 righe estratte. Ingest "limitato" con contenuto ricostruito dal Manuale Misura #82 + concept stub esistente + conoscenza pubblica. Caveat di ingest documentato esplicitamente nel nodo.
- `ACN Manuale Operativo implementazione misura-82.pdf`: identità confermata, v3.0 marzo 2023.
- `2025.04311_01_ms_v2.0_Handbook for Cyber Stress Tests_en.pdf`: **autore verificato = ENISA** (non ECB/SSM come ipotizzato dal codice file `_ms_`). Decisione: ingest (skip esclusa).

Pagine create (3 sources):
- [[sources/ACN Strategia nazionale di cybersicurezza 2022-2026]] — `scope: grc_personal`. Strategia adottata 17/05/2022. 3 obiettivi + 4 fattori abilitanti + 82 misure.
- [[sources/ACN Manuale operativo Misura 82]] — `scope: grc_personal`. Manuale ACN per KPI di tutte le 82 misure. Pendant ISO 27001 § 9.1.
- [[sources/ENISA Handbook for Cyber Stress Tests v2.0 - 2025-05]] — `scope: grc_personal`. ENISA maggio 2025, cross-settore. Case studies: ECB 2024 (finanza) + CER 2024 (energia) + Annex A (salute).

Pagine aggiornate (1 concept):
- [[concepts/Strategia nazionale di cybersicurezza]] — stub Wave 1 → riempito con sintesi Strategia 2022-2026. Conformità Art. 7 NIS2 ✓ (verifica coverage). Frontmatter `sources` allargato a 3.

**Open question aperte in Sessione 4**:
1. Lacuna tecnica Strategia 2022-2026 (PDF scannerizzato; ricostruzione vs OCR).
2. Revisione interna ACN su stress test cyber (se esiste).
3. Misura #82 v4.0+ con target/risultati 2024-2026.
4. Strategia 2027-2031 (aggiornamento atteso).

**Stato finale wiki**: **39 sources, 17 entities, 36 concepts, 6 synthesis = 98 nodi totali**. Verifica scope tagging post-Sessione 4: **98/98 nodi taggati** (grep di chiusura: 0 MISSING).

Distribuzione scope finale: 63 both (64%) + 32 grc_personal (33%) + 3 nis2_tool (3%).

**STATUS WAVE 6 — ✅ COMPLETED (2026-05-19)**:
- Cluster A + B + C + D + E + F tutti chiusi
- Sessioni 1-4 + 3 mini-fix housekeeping
- Wave 6.5 retrofit chiuso (95/95 → 98/98 con nuovi nodi Sessione 4)
- Skip definitivi: Sapienza slide + CELEX duplicato

Wave report dettagliato: [[_meta/wave_reports/Wave_6_2026-05-18]] aggiornato con sezione Sessione 4 + STATUS Wave 6 COMPLETED.

Prossimo passo previsto: **pausa per human review** finale. Wave 6 chiusa. Passaggio operativo al lavoro sul NIS2 Tool (incorporamento dell'avvertenza testuale pilot Cloud nel verdetto, review consulente GRC esterno) oppure inizio percorso ISO 27001 LA. Su cue di Andrea.

## [2026-05-19] re-ingest | Wave 6 — ACN Strategia 2022-2026 versione testuale [open question chiusa]

Andrea ha ricaricato `raw/articles/ACN_Strategia.pdf` in versione testuale (5.16 MB, vs 14.3 MB della scansione precedente). Estrazione `pdftotext`: 1040 righe, 27 pagine, contenuto integralmente leggibile.

Source [[sources/ACN Strategia nazionale di cybersicurezza 2022-2026]] aggiornato direttamente dal testo del documento (non più ricostruito):

- "Caveat di ingest" → "Storia di ingest" (documenta prima ingest "limitata" + re-ingest testuale).
- "Struttura ricostruita" sostituita da contenuti puntuali estratti:
  - Struttura documento: Prefazione + Premessa + Cap. #1 (5 sfide) + Cap. #2 (3 obiettivi + 2 fattori abilitanti) + Acronimi (27 pp).
  - **5 sfide** identificate: transizione digitale cyber-resiliente PA/produttivo · autonomia strategica · anticipazione minaccia · gestione crisi · contrasto disinformazione.
  - **Obiettivo PROTEZIONE**: 7 misure-categorie (CVCN/CV/laboratori · quadro giuridico + zero-trust + CVD · situational awareness · maturità PA + PSN/Cloud · infrastrutture nazionali BGP/DNS · crittografia · disinformazione).
  - **Obiettivo RISPOSTA**: 6 misure-categorie (sistema crisi nazionale NCS + Blueprint UE 2017/1584 a 3 livelli · Hyper SOC + ISAC + CSIRT/CERT settoriali federati · esercitazioni · attribuzione (EU Cyber Diplomacy Toolbox + NATO) · contrasto cybercrime · deterrenza).
  - **Obiettivo SVILUPPO**: 5 misure-categorie (NCC ↔ ECCC · tecnologia nazionale/UE · parco nazionale · PSIRT · innovazione PA).
  - **4 pilastri tecnico-operativi** dell'architettura nazionale cyber (D.L. 82/2021): Cyber Sicurezza & Resilienza (ACN) · Criminalità informatica (Forze di polizia) · Difesa militare (Min. Difesa) · Ricerca ed elaborazione informativa (Comparto intelligence). + cyber diplomacy trasversale (MAECI).
  - **Strumenti finanziari**: 1,2% investimenti nazionali lordi/anno · Orizzonte Europa 95,51 mld · Europa Digitale 7,59 mld · **PNRR Investimento 1.5 "Cybersecurity" 623 milioni di euro** (174M servizi cyber + 301,7M resilienza PA + 147,3M scrutinio/certificazione).
  - **Capacity building ACN**: target 800 unità entro 2027.
- "Cornice istituzionale" arricchita: 12 soggetti (era 5) — aggiunti Autorità delegata, CISR, NCS, CSIRT Italia, Min. Difesa, MAECI, Forze di polizia, Comparto intelligence.
- "Lacuna nota tecnica" → ✅ **chiusa**: re-ingest testuale eseguito.

Stato wiki: contatori invariati (modifica in-place). **39 sources, 17 entities, 36 concepts, 6 synthesis = 98 nodi**.

Prossimo passo previsto: pausa per human review. Wave 6 chiusa con tutti i contenuti consolidati (incluso Strategia ora ingerita direttamente dal documento ufficiale).

## [2026-05-23] ingest | Wave 7 — Legge 90/2024 (cybersicurezza nazionale)

Ingest unitario della L. 28 giugno 2024 n. 90 (GU 02/07/2024 n. 153, vigente dal 17/07/2024). 24 articoli su 2 capi: Capo I cybersicurezza/governance PA/contratti pubblici (artt. 1-15-bis), Capo II reati informatici (artt. 16-23) + art. 24 disposizioni finanziarie.

**Decisioni di scope concordate con Andrea pre-ingest**:
- 1 source unitaria (non spezzata in Capo I / Capo II) — Capo II trattato come sezione operativa GRC di 150-200 parole, no concept dedicato.
- 3 concept nuovi (non 4 come proposta iniziale: il concept "Reati informatici Capo II" è stato espunto, off-topic per posizionamento NIS2-GRC).
- Synthesis L. 90 ↔ NIS2 fatta **nello stesso ingest**, non rimandata a Wave 7-bis.
- DPCM attuativi attesi: opzione A (tabella tracker interna alla source), non concept dedicati.
- Angolazione 75% operativa / 25% sistemica.
- Capo II flaggato `grc_personal` nei commenti interni della source; scope source `both`.

Pagine create (5):

Source (1):
- [[sources/Legge 90-2024 (cybersicurezza nazionale)]] — `scope: both`. Atto unitario. Capo I esploso art. per art.; Capo II in sintesi operativa GRC; sezione "Atti attuativi attesi" come tabella tracker (DPCM art. 11 + art. 14 + altri).

Concept (3):
- [[concepts/Perimetro Legge 90-2024]] — `scope: both`. Ambito soggettivo tassativo art. 1 c. 1: PA centrali + locali grandi + trasporto qualificato + ASL + in house qualificate. Esclusioni c. 7. Phase-in 180gg. Sovrapposizione/disgiunzione con All. III NIS.
- [[concepts/Referente per la cybersicurezza (L. 90-2024)]] — `scope: both`. Art. 8 c. 2 + 7 funzioni struttura c. 1. Triplice coincidenza pdc NIS / referente / RTD CAD. Esercizio in forma associata. Esoneri PSNC/intelligence.
- [[concepts/Elementi essenziali di cybersicurezza (procurement)]] — `scope: grc_personal`. Art. 14 + DPCM atteso (120gg, scadenza 14/11/2024). Tetto 10% punteggio economico. Criterio Buy EU/NATO. Estensione privati PSNC.

Synthesis (1):
- [[synthesis/Coordinamento L. 90-2024 e NIS2]] — `scope: both`. Risposta T3 (esclusione asimmetrica con coordinamento operativo). Disambiguazione esclusioni art. 1 c. 7 + ridireccionamento art. 15-bis. Decision tree pratico + tabella casi pratici + tabella riassuntiva adempimenti.

Pagine aggiornate (5):

- [[concepts/Notifica di incidente significativo]] — aggiunta sezione "Disallineamento con la L. 90/2024": tabella 24h+72h+1mese (NIS) vs 24h+72h (L. 90, no report finale). Implicazione per soggetti NIS ∩ L. 90.
- [[entities/Punto di contatto NIS]] — riferimento "Coordinamento Legge 90/2024" arricchito con link al nuovo concept Referente cyber + cenno triplice coincidenza con RTD; sources frontmatter ampliato.
- [[concepts/Sanzioni NIS2]] — aggiunta sezione "Allineamento orizzontale del regime sanzionatorio italiano (PA + L. 90 + PSNC)": forbice 25-125k armonizzata tra 3 regimi, responsabilità personale aggravata su L. 90; DPCM atteso ex art. 11 L. 90 sul procedimento sanzionatorio.
- [[entities/ACN]] — aggiunta sezione "Funzioni e poteri introdotti/rafforzati dalla L. 90/2024" (Centro Nazionale di Crittografia, raccolta notifiche, procedimento sanzionatorio, cooling-off personale, CSIRT pubblico ufficiale, raccordo Procura nazionale antimafia, adeguamento vulnerabilità 15gg, Nucleo allargato, funzione procurement art. 14).
- [[synthesis/Stratificazione delle norme cybersecurity in Italia]] — § 5 Legge 90/2024 sostituito: era ricostruito sommariamente, ora ha riferimenti puntuali (art. 1 c. 1 tassativo, c. 3 phase-in, c. 7 esclusioni, art. 8, art. 14, art. 15-bis come chiave del coordinamento), + accenno Capo II.

Stato wiki dopo Wave 7: **40 sources, 17 entities, 39 concepts, 7 synthesis = 103 nodi** (era 39/17/36/6 = 98). Tutti nuovi nodi taggati: 1 source `both` + 2 concept `both` + 1 concept `grc_personal` + 1 synthesis `both`.

Atti attuativi attesi tracciati nella source (sezione tabella): DPCM art. 11 (90gg, atteso ≈ 15/10/2024) + DPCM art. 14 (120gg, atteso ≈ 14/11/2024) + Determinazione DG ACN art. 1 c. 5 (modalità ispezioni) + Determinazione DG ACN art. 1 c. 1 (tassonomia incidenti L. 90) + Determinazione DG ACN art. 12 (percorsi formativi cooling-off) + Regolamento ex art. 43 L. 124/2007 (art. 13 c. 5) + decreto legislativo via L. 15/2024 (art. 15 DORA-equivalenti intermediari). Al prossimo lint: verificare emanazioni.

Lacune note ancora aperte (al 2026-05-23):
- DL 82/2021 (istituzione ACN) non in `raw/` — la L. 90 lo modifica in 5 articoli, da considerare per Wave 8 se serve.
- DL 105/2019 (PSNC) non in `raw/` — citato 14 volte dalla L. 90.
- L. 124/2007 (Sistema informazione sicurezza) non in `raw/` — richiamata in 6 articoli della L. 90.
- Determinazioni ACN / DPCM attuativi della L. 90 non emanati o non ingeriti.

Prossimo passo previsto: pausa per human review. Wave 7 chiusa. Possibili Wave 8: ingest DL 82/2021 + DL 105/2019 + DPCM attuativi L. 90 quando disponibili; oppure ingest DORA Reg. UE 2022/2554 + D.Lgs. 134/2024 (CER) per chiudere lo stack regolatorio italiano completo.

## [2026-05-30] fix | Responsabilità degli organi di gestione — pulizia stream-of-thought + chiusura tensione interpretativa

Due fix su [[concepts/Responsabilità degli organi di gestione]] dopo human review:

1. **Rimosso riferimento "(Wave 4)"** dalla sezione "Tensioni interpretative" (violazione CLAUDE.md §8: meta-cronologia interna non deve comparire nei file della wiki).
2. **Aggiornata sezione "Tensioni interpretative"** integrando i chiarimenti delle FAQ ACN ingerite in Wave 4:
    - Primo punto (governance societaria non standard) → **chiuso**: FAQ `ODA.1/4/5/8/9` di [[sources/FAQ NIS - Ruoli e procedure]] + art. 1 c. 1 lett. e Det. ACN 379887/2025 (oggi sostituita dalla [[sources/Determinazione ACN piattaforma e procedure - 2026-04-13|Det. 127437/2026]]) declinano tutti i casi (CDA, monocratico, organo analogo, rappresentante legale, delega interna, artt. 2381/2392 c.c.).
    - Secondo punto (PA centrali: Ministro vs Capo Dipartimento vs dirigente apicale) → **resta aperto**: nessuna FAQ ad hoc; applicabile per analogia solo il criterio generale `ODA.5`. Riformulato al presente.

Pagine aggiornate (2):
- [[concepts/Responsabilità degli organi di gestione]] — frontmatter `sources` allargato da 3 a 5 (+ FAQ Ruoli e procedure + Det. piattaforma 2026-04-13); riscritta "Tensioni interpretative".
- [[index]] — contatore fonti aggiornato (3→5) + one-liner integrato con "FAQ ODA chiariscono governance non standard".

Stato wiki: contatori nodi invariati. **40 sources, 17 entities, 39 concepts, 7 synthesis = 103 nodi**.

Note: analoghe formule "Wave N" sono presenti in altri nodi (es. [[sources/Determinazione ACN piattaforma e procedure - 2026-04-13]] linee 127-128). Da valutare se promuovere a lint sistematico cross-wiki o se lasciare circoscritto a fix puntuali su richiesta.

## [2026-06-05] fix | Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025 — numero definizione cloud art. 6 NIS2

Corretto errore fattuale di citazione in [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]]: la definizione di "servizio di cloud computing" nella Direttiva (UE) 2022/2555 è all'**art. 6 punto (30)**, non (33). Il punto (33) definisce la "piattaforma di servizi di social network" (MSP = (39), MSSP = (40)). Verificato su fonte primaria (EUR-Lex + glossario ufficiale Direttiva NIS2).

Occorrenze corrette (4): righe 99, 103, 109, 137. Solo il numero di punto era errato; il testo della definizione (riga 101) era già corretto.

Origine: errore emerso durante la verifica del corpus del NIS2 Tool (`corpus/sectors/sectors__cloud_computing.yaml`), che aveva ereditato l'ID `dir_nis2_art_6_33` da questa synthesis (la wiki è dichiarata "fonte di verità del knowledge model" nel CLAUDE.md del tool). Correzione da propagare a valle nel tool: `dir_nis2_art_6_33` → `dir_nis2_art_6_30` (3 occorrenze, righe 16/29/30 del YAML) — in attesa di conferma.

Pagine aggiornate (1): [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]]. Contatori index invariati.

## [2026-07-02] decision | retag scope DORA + istituzione decision log
Pagine aggiornate: [[concepts/Coordinamento DORA-NIS]] (`scope: grc_personal` → `both`).
Pagine create: [[_meta/decision_log]] (registro decisioni di governance scope/export).
Decisioni registrate: DEC-001 (retag DORA a `both`, ATTUATA) — DORA è domanda di disambiguazione del wizard e voce del catalogo eccezioni con citazioni puntuali, quindi il nodo di coordinamento deve stare nell'export della Project Knowledge; DEC-002 (retag Cross-walk a 4 framework a `both`, PIANIFICATA al kickoff v0.2 per l'estensione controlli Fase 3 — NON eseguito ora, coerente con scope v0.1.0).
Note: `index.md` invariato — la riga del catalogo non espone `scope` e non esiste tally aggregato per valore. Distribuzione scope aggiornata: both 68, grc_personal 32, nis2_tool 3 (su 103 nodi).

## [2026-07-02] decision | retag scope Cross-walk (DEC-002 attuata, anticipata)
Pagine aggiornate: [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] (`scope: grc_personal` → `both`, frontmatter + prosa allineata alla riga 17), [[_meta/decision_log]] (DEC-002 PIANIFICATA → ATTUATA).
Note: retag anticipato su richiesta utente rispetto al trigger originario (kickoff v0.2). `index.md` invariato. Distribuzione scope aggiornata: both 69, grc_personal 31, nis2_tool 3 (su 103 nodi). Con DEC-001 (DORA) e DEC-002 (Cross-walk) l'export della Project Knowledge include ora tutti i nodi di coordinamento/mapping citati dal gate v0.1.0.

## [2026-07-02] fix | Identità documentale Det. 127434/127437 + chiusura DIV-P1 (esoneri DORA)
Contesto: direttiva stop-and-ingest su Det. 127437/2026 con premessa falsa (`251218` = Det. 379887 abrogata; `Det_127437_2026.pdf` = piattaforma corretta). Verifica sul TESTO dei PDF: premesse invertite. `detacn_piattaformanis_251218-v9_signed.pdf` = piattaforma vigente Det. 127437/2026 (24 artt., 6 Capi, "aggiorna e sostituisce" 379887, applic. 15/04/2026, firma 12:13:09); il token `251218` è codice di bozza, non protocollo. `Det_127437_2026.pdf` = determinazione termini (protocollo 127434, 5 artt., applic. 30/04/2026, firma 12:12:15), filename con protocollo errato.
Pagine aggiornate: [[sources/Determinazione ACN piattaforma e procedure - 2026-04-13]] (`source_path` → PDF firmato reale; callout DIV-P1 `warning` → `note` verificato: esoneri DORA art. 7 c. 6, art. 16 c. 13 [c. 3 lett. b) + art. 17], art. 20 c. 6, adesione volontaria fatta salva); [[concepts/Coordinamento DORA-NIS]] (stesso retag doppio del callout); [[concepts/Clausola di salvaguardia]] (allineata la distinzione art. 3 c. 4 = definisce la deroga / art. 3 c. 12 = ACN applica secondo criteri ex art. 40 c. 1 → DPCM 221/2024; procedura di richiesta = art. 12 det. piattaforma); [[sources/Determinazione ACN termini soggetti 2026 - 2026-04-30]] (`source_path` → `raw/articles/Det_127434_2026_termini.pdf`; aggiunti `protocol_number` 127434/2026 e `protocol_source`; nota di provenienza + copia ridondante `detacn_misuresicurezza-v4_post.pdf`).
File raw: `Det_127437_2026.pdf` rinominato `Det_127434_2026_termini.pdf` (override immutabilità raw autorizzato dall'utente per il solo rename). Copia ridondante non rimossa (cancellazione non autorizzata).
Corpus (nis2-check): `regimes/dora.yaml` (open_points → []; citazioni a granularità di comma; header CHIUSO); `fixtures/E06` (open_points → []; corpus_version 0.2.1; citazioni allineate); `signals__cumulative_regimes.yaml` (aggiunta citazione `dlgs_138_2024_art_3_c_12`); `VERSION` 0.2.1; `CHANGELOG` [0.2.1]; ADR `0007-ingest-det-127437-identita-documentale.md` (analisi errore + checklist ingest estesa); ADR 0006 nota di aggiornamento; `fixtures/README.md`.
Contatore crediti: secondo credito stop-and-ingest NON consumato (correzione di attestazione, premessa falsa) — residuo 1 fino a v0.1.0 (DEC-003 nel decision log). Contatori `index.md` invariati (nessun nodo creato/rimosso).

## [2026-07-02] fix | Repoint 6 source_path morti (_tmp) + export Project Knowledge (72 nodi)
Contesto: lo sweep di igiene su `raw/` aveva rilevato 6 nodi `sources/` con `source_path` verso `raw/articles/_tmp/*.txt` (cartella temporanea di estrazione non più esistente). Identità dei 6 documenti già verificate dal testo nello sweep; via libera utente al repoint (solo frontmatter, nessun contenuto).
Pagine aggiornate (6, solo `source_path`):
- [[sources/Determinazione ACN categorizzazione - 2026-04-13]] → `raw/articles/detacn_categorizzazione_260409-v8_signed.pdf`
- [[sources/Determinazione ACN accordi condivisione - 2025-04-10]] → `raw/articles/detacn_nis_accordi_2025_136118_signed.pdf`
- [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]] → `raw/articles/detacn_obblighi_2511-v3_signed.pdf`
- [[sources/Determinazione ACN funzionamento Tavolo NIS - 2025-07-16]] → `raw/articles/2025_276206_determinazioneacn_tavolonis_funzionamento-v4-clean-v1_signed.pdf`
- [[sources/Determinazione ACN composizione Tavolo NIS - 2026]] → `raw/articles/2026_112335_detacn_comptavolo_signed.pdf`
- [[sources/Linee Guida NIS - Gestione incidenti - 2025-12]] → `raw/articles/definizione-del-processo-di-gestione-degli-incidenti-di-sicurezza-informatica.pdf`
Export: generato `nis2-check/export/` (Project Knowledge del NIS2 Tool) filtrando `scope: nis2_tool OR both` — **72** file markdown (25 sources, 31 concepts, 10 entities, 6 synthesis), struttura wiki mirrorata, zero `source_path` morti tra i nodi esportati. Vault verificato pulito (0 residui `_tmp`). `index.md` invariato.

## [2026-10-26] housekeeping | Pre-pubblicazione vault (provenance, link, report Wave 7)
Contesto: interventi meccanici prima della pubblicazione del repo; nessuna modifica al contenuto normativo dei nodi, nessuna risoluzione dei marcatori "da verificare", nessun ingest.
Repo: `memory/` aggiunta a `.gitignore` e rimossa dal tracking (`git rm -r --cached`, file conservati su disco).
Pagine aggiornate:
- `wiki/README.md` — riga 3: nome utente corretto (Andrea).
- [[sources/ISO IEC 27000-2018]], [[sources/ISO IEC 27001-2022]], [[sources/ISO IEC 27002-2022]] — `source_path` sostituito con riferimento bibliografico (27000: URL ISO Publicly Available Standards); `provenance_note` e paragrafo "Provenance e politica di citazione" riscritti senza nominare la fonte della copia, informazioni di verifica dell'edizione conservate.
- Nome della fonte della copia sostituito con "copia non ufficiale" anche in `_meta/wave_reports/Wave_6_2026-05-18.md` (8 occorrenze) e in questo log (4 occorrenze, voce 2026-05-19).
- Wiki-link corretti verso nodi esistenti (13 link in 7 nodi): Cross-walk v1 → [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] (6 link in [[sources/FNCDP 2025 v2.1 Core]], [[sources/ISO IEC 27000-2018]], [[sources/ISO IEC 27001-2022]], [[sources/ISO IEC 27002-2022]], [[sources/NIST CSF 2.0 - 2024-02-26]]); in [[sources/FAQ NIS - Ruoli e procedure]] 4 link (Punto di contatto NIS, Referente CSIRT → `entities/`; Notifica di incidente significativo; Rappresentante NIS in Italia); in [[sources/FAQ NIS - Settori, sottosettori e tipologie di soggetto]] 3 link (Settori altamente critici / Settori critici → [[concepts/Settori altamente critici e critici]] con alias; Identificazione dei soggetti NIS).
- Lasciati invariati i link a riferimenti non ancora ingeriti (D.L. 105/2019, D.Lgs. 65/2018, D.Lgs. 231/2001, MEF, MiC, MUR) e i casi dubbi (Autorità nazionale competente NIS, 10 concept senza nodo).
Pagine create: `_meta/wave_reports/Wave_7_2026-05-23.md` (ricavato dalla voce di log del 2026-05-23, nessuna informazione nuova). `_meta/wave_reports/index.md`: aggiunta riga Wave 7 (Wave_6_5_PLANNED già marcato superseded). `index.md`: riga "Ultimo aggiornamento" → 2026-10-26.
Contatori `index.md` invariati (103 nodi).

## [2026-10-26] housekeeping | README pubblico, LICENSE, DEC-005, generalizzazione riferimenti personali
Contesto: preparazione alla pubblicazione (gate pre-lancio, opzione B: KB esente dalla review GRC terza). Nessuna modifica al contenuto normativo dei nodi.
Pagine create:
- `LICENSE` — testo ufficiale CC BY 4.0 scaricato da creativecommons.org (`legalcode.txt`), non riscritto.
- `README.md` (radice) — descrizione, disclaimer, organizzazione, fonti coperte, metodo, stato di verifica. Conteggi della sezione "Stato di verifica" riscontrati sul vault prima del salvataggio: 20 punti "da verificare" (non 22: i due marcatori ⚠ di Macro-aree NIS e Allegato 2 modello segnalano la differenza Logistica tra i modelli, non una verifica aperta); 2 determinazioni con protocollo non stampato e senza attestazione registrata (accordi 136118/2025, composizione Tavolo 112335/2026; categorizzazione 155238/2026 e specifiche di base 379907/2025 risultano attestate tramite FAQ ACN); rimossa la lacuna sulla determinazione ACN identificativa delle PA NIS (non presente nel vault).
Pagine aggiornate:
- `_meta/decision_log.md` — DEC-005 (gate pre-lancio, opzione B, ATTUATA; rinvio a `nis2-check/docs/decisions/0008`).
- 16 nodi di `wiki/` — riferimenti personali generalizzati ("l'autore", "una transizione da software engineering a GRC"), nome del provider di formazione rimosso. In [[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]]: alias personale rimosso, paragrafo "Vincolo del nodo" riscritto, attore della tabella azioni → "Autore", eliminate 2 righe con tempi personali di pianificazione. Analisi dei profili invariata.
Verifica: `git grep "Andrea" -- wiki/` restituisce solo `wiki/README.md`.

## [2026-10-26] lint | Size-cap rule: soglie dimensionali allineate alla FAQ AMB.DI.1
Contesto: contraddizione rilevata durante una query (caso NACE div. 26, 60 dipendenti). Lint mirato su un nodo, con conferma dell'autore già data.
Trovati: 1 contraddizione. [[concepts/Size-cap rule]] (Definizione) usava un criterio alternativo ("50-250 dipendenti o fatturato 10-50 M€"; "grandi: >250 dipendenti o fatturato/bilancio >50 M€"), in contrasto con [[sources/FAQ NIS - Ambito]] `AMB.DI.1` (Racc. 2003/361/CE: criterio degli effettivi sempre necessario + almeno uno tra fatturato e bilancio; salita di categoria se gli effettivi sono superati oppure se entrambi i parametri contabili sono superati). Prima verifica: `AMB.DI.1` nel nodo FAQ è coerente con la regola e con i 6 esempi riportati.
Azioni:
- [[concepts/Size-cap rule]]: Definizione riscritta (tabella soglie effettivi/fatturato/bilancio, regola di appartenenza, regola di salita, tre punti micro-piccole/medie/grandi), citazione di [[sources/FAQ NIS - Ambito]] `AMB.DI.1` accanto a [[sources/Direttiva (UE) 2022-2555 (NIS2)]]; FAQ Ambito aggiunta a `sources:`; campo `updated: 2026-10-26` aggiunto (assente). Resto del nodo invariato.
- [[concepts/Soggetti essenziali e importanti]]: stessa formulazione alternativa nella definizione dei soggetti essenziali (">250 dipendenti o fatturato >50 M€"), allineata ad `AMB.DI.1`; campo `updated: 2026-10-26` aggiunto (assente).
- `index.md`: riga Size-cap rule aggiornata (3 fonti).
Non corretti, da valutare: la stessa formulazione alternativa compare in [[sources/Direttiva (UE) 2022-2555 (NIS2)]] (Punti chiave, "medio = 50-250 dipendenti o fatturato 10-50 M€; grande = >250 o >50 M€") e in [[sources/FAQ NIS - Registrazione]] `PDA2.1` ("≥50 dipendenti o fatturato/bilancio ≥10M€").

## [2026-10-26] housekeeping | sweep pre-pubblicazione (dati personali, link, formulazioni dimensionali, attestazione protocolli)
Contesto: sweep finale prima della pubblicazione, su indicazione dell'autore. Un solo commit, nessuna riscrittura della storia.
Pagine aggiornate:
- [[CLAUDE]] — nota iniziale ridotta a "L'autore e utente del vault è Andrea Tierno." (rimossi email e path).
- `log.md` — righe 17 e 242: "Francesco" → "Andrea" (righe 20 e 29, che documentano la correzione del nome, invariate).
- `.gitignore` — aggiunto `.claude/settings.local.json`; il file è rimosso dall'indice (`git rm --cached`) e resta su disco.
- [[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]] — nota sullo "strumento privato di pianificazione di carriera" riscritta come nodo di posizionamento su profilo-tipo, non consulenza di carriera.
- Wiki-link con barra nel nome del nodo riscritti con il trattino (10 link in 8 nodi): `D.L. 105/2019 (perimetro)` → `D.L. 105-2019 (perimetro)` (6), `D.Lgs. 65/2018` → `D.Lgs. 65-2018` (2), `D.Lgs. 231/2001` → `D.Lgs. 231-2001` (2). Nessun altro link con lo stesso problema in `wiki/` e `index.md`.
- [[concepts/Size-cap rule]] — Implicazioni: "anche solo per crescita di fatturato" allineata alla regola di salita `AMB.DI.1`.
- [[sources/Direttiva (UE) 2022-2555 (NIS2)]] — Punti chiave: soglie "medio = 50-250 dipendenti o fatturato 10-50 M€" (semplificazione dell'agente; art. 2 par. 1 della direttiva rinvia alla Racc. 2003/361/CE senza valori propri) sostituite dal rinvio alla Raccomandazione.
- [[sources/FAQ NIS - Registrazione]] — `PDA2.1`: la parentesi "≥50 dipendenti o fatturato/bilancio ≥10M€" non è nel testo della FAQ (PDA2.1 dice solo "superano i massimali per le micro e piccole imprese"); allineata con rinvio ad `AMB.DI.1`.
- [[sources/FAQ NIS - Ambito]] — `AMB.DI.1` esempio 4: il PDF usa "almeno 50 milioni" / "almeno 43 milioni", il nodo è fedele; aggiunta nota dell'agente sull'ambiguità al confine rispetto alla definizione "non superiore a".
- [[sources/Determinazione ACN accordi condivisione - 2025-04-10]], [[sources/Determinazione ACN composizione Tavolo NIS - 2026]] — aggiunti `protocol_number` e `protocol_source`: i numeri 136118 e 112335 compaiono sulla pagina ACN "La normativa NIS" ([[sources/La normativa NIS - Pagina ACN]]) associati alle rispettive determinazioni; i testi firmati non li stampano.
- `README.md` — paragrafo protocolli riscritto (6 determinazioni senza numero stampato, tutte attestate); aggiunti i 4 punti "da chiarire" e la nota ISO IEC 27000-2018 in Stato di verifica; pagina "La normativa NIS" in Fonti coperte; riga "Ultimo aggiornamento di contenuto" aggiornata.
Note: i 4 punti "da chiarire" risultano da grep in D.Lgs. 138-2024, FAQ Aggiornamento, FAQ Registrazione e Cronologia attuativa NIS2 in Italia (non in FAQ Ruoli e procedure, che ha solo un "non chiara" senza marcatore).

## [2026-10-26] lint | Direttiva NIS2: formulazione dei soggetti essenziali allineata ad AMB.GE.2
Trovati: 1 imprecisione. [[sources/Direttiva (UE) 2022-2555 (NIS2)]] (Punti chiave, classificazione binaria) descriveva gli essenziali come "medio/grandi in settori altamente critici", in contrasto con [[sources/FAQ NIS - Ambito]] `AMB.GE.2` (essenziali = soggetti Allegato I che superano i massimali delle medie imprese, più le categorie a prescindere dalla dimensione; le medie imprese Allegato I sono importanti).
Azioni: riga allineata ad `AMB.GE.2` con rinvio a [[sources/FAQ NIS - Ambito]] e [[concepts/Soggetti essenziali e importanti]]. Incluso nel commit `.obsidian/graph.json` (configurazione del grafo: filtro `path:wiki -file:README`, colori per layer sources/entities/concepts/synthesis).

## [2026-10-27] lint | D.Lgs. 138/2024: attestazione art. 3 c. 6 (PA indipendentemente dalla dimensione)
Trovati: 1 lacuna di attestazione. [[sources/D.Lgs. 138-2024 (Decreto NIS)]] (Punti chiave, Ambito) non citava l'art. 3 c. 6 (applicazione alle PA di cui all'art. 1 c. 3 L. 196/2009 ricomprese nelle categorie dell'Allegato III, indipendentemente dalla dimensione). La disposizione era già attestata in [[sources/FAQ NIS - Settori, sottosettori e tipologie di soggetto]] (riga 220, Settore PA).
Verifica: comma estratto con `pdftotext -enc UTF-8` da `raw/articles/Decreto NIS2.pdf`. La citazione nel nodo coincide parola per parola con il testo del PDF. Il nodo FAQ è una parafrasi coerente con il comma.
Azioni: aggiunto sotto-punto "Art. 3, c. 6 — Pubbliche amministrazioni" con citazione testuale e rinvio al nodo FAQ (1 riga). Frontmatter e `scope: both` invariati, resto del nodo invariato. Registrata come DEC-006 in [[_meta/decision_log]]. Contatori `index.md` invariati.
Non corretto, da valutare: lo stesso punto Ambito elenca "PA centrali" tra i soggetti inclusi indipendentemente dalle soglie, mentre l'Allegato III comprende anche amministrazioni regionali e locali.
