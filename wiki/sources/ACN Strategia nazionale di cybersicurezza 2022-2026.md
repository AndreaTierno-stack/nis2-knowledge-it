---
title: Strategia Nazionale di Cybersicurezza 2022-2026
type: source
scope: grc_personal
source_type: paper
source_path: raw/articles/ACN_Strategia.pdf
url: https://www.acn.gov.it/portale/strategia-nazionale-di-cybersicurezza
author: Presidenza del Consiglio dei Ministri (Comitato Interministeriale per la Cybersicurezza) — Coordinamento Agenzia per la Cybersicurezza Nazionale
date_published: 2022-05-17
date_ingested: 2026-05-19
tags: [italia, strategia, indirizzo-politico, acn, cybersicurezza-nazionale, piano-implementazione, kpi]
aliases: [Strategia Nazionale Cybersicurezza, Strategia ACN 2022-2026, SNC 2022-2026]
---

## Storia di ingest

- **Prima ingest (2026-05-19, Sessione 4)**: PDF originale 14.3 MB era scansione/immagine senza livello testuale; contenuto **ricostruito** dal Manuale Misura #82 + conoscenza pubblica. Caveat di ingest documentato come open question.
- **Re-ingest (2026-05-19, post-Sessione 4)**: l'autore ha ricaricato una **versione testuale** del PDF (5.16 MB con testo selezionabile, 27 pp, 1040 righe estratte). Open question chiusa. Contenuto della presente versione **ingerito direttamente dal testo del documento**, non più ricostruito.

## TL;DR

**Strategia Nazionale di Cybersicurezza 2022-2026** dell'Italia, adottata dal **Presidente del Consiglio dei Ministri il 17 maggio 2022** con il coinvolgimento del [[entities/Comitato Interministeriale per la Cybersicurezza|CIC]] e coordinata operativamente dall'[[entities/ACN]]. Documento di **indirizzo politico-strategico** che definisce la postura italiana in materia di cybersicurezza per il quinquennio 2022-2026. Strutturata in **3 macro-obiettivi** (Protezione / Risposta / Sviluppo) + **4 fattori abilitanti** (Formazione / Cultura / Cooperazione / Metriche e KPI), declinati nel **Piano di Implementazione** che contiene **82 misure** puntuali con responsabili, anno di prevalente implementazione, e indicatori di misurazione.

Per la wiki, è la **cornice politica** entro cui si colloca il regime NIS2 italiano: la Strategia precede l'entrata in vigore del [[sources/D.Lgs. 138-2024 (Decreto NIS)|D.Lgs. 138/2024]] (sett. 2024) ma è esplicitamente richiamata dall'art. 9 del decreto come uno dei pilastri del quadro nazionale. Il regime NIS2 si innesta come una delle linee di lavoro della Strategia (in particolare nelle misure di Protezione e nei fattori di Cooperazione/Formazione).

Per una transizione da software engineering a GRC, è riferimento per:
- Articoli LinkedIn / blog post di posizionamento ("la Strategia nazionale prevede X, il mio NIS2 Tool contribuisce a Y").
- Contesto di sistema per consulenze a clienti italiani (PA in particolare).
- Allineamento con il livello di policy ENISA/UE (cyber resilience, Cyber Solidarity Act, ecc.).

## Struttura del documento

Il documento ufficiale della Strategia ha **27 pagine** con la seguente struttura:

| Sezione | Pagina |
|---|---|
| Prefazione | 2 |
| Premessa | 4 |
| **#1 — Le sfide da affrontare** | 9 |
| **#2 — Visione strategica: gli obiettivi da perseguire** | 15 |
| Elenco degli acronimi | 27 |

Il **Piano di Implementazione** della Strategia (con le 82 misure puntuali, attori responsabili, indicatori) è documento **separato e annesso** — il dettaglio operativo è coperto in [[sources/ACN Manuale operativo Misura 82]].

## Cap. #1 — Le 5 sfide da affrontare

La Strategia identifica esplicitamente **5 sfide** che il sistema-paese deve affrontare nel periodo 2022-2026:

1. **Assicurare una transizione digitale cyber resiliente** della PA e del tessuto produttivo. Include sotto-sfida di forza lavoro qualificata + questione di genere (poche donne in STEM/cyber).
2. **Autonomia strategica nazionale ed europea** nel settore del digitale. Riduzione della dipendenza tecnologica da Paesi extra-UE su EDT (IA, quantum, ecc.).
3. **Anticipare l'evoluzione della minaccia cyber**. Difesa attiva oltre la difesa passiva: aumentare i costi degli attacchi per renderli economicamente svantaggiosi.
4. **Gestione di crisi cibernetiche** in scenari geopolitici complessi: pre-allerta, eventi su larga scala, set predefinito di misure.
5. **Contrastare la disinformazione online** nel più ampio contesto della cd. **minaccia ibrida**: protezione del sistema democratico, specie durante consultazioni elettorali.

## Cap. #2 — Visione strategica: 3 obiettivi + 2 fattori abilitanti

### Obiettivo 1 — PROTEZIONE (7 misure-categorie)

Protezione degli asset strategici nazionali tramite approccio sistemico di gestione e mitigazione del rischio.

| Lett. | Misura-categoria |
|---|---|
| A | **Potenziamento del CVCN** (Centro di Valutazione e Certificazione Nazionale dell'ACN) + Centri di Valutazione (CV) di Min. Interno e Min. Difesa + rete di **Laboratori Accreditati di Prova** |
| B | **Definizione e mantenimento di un quadro giuridico nazionale** aggiornato: schemi di certificazione UE, **zero-trust** per la PA, procurement ICT sicuro, **politica nazionale sulla CVD** (Coordinated Vulnerability Disclosure) |
| C | **Conoscenza approfondita della minaccia + situational awareness**: monitoraggio continuo + scambio informativo pubblico-privato e pubblico-pubblico + canali di comunicazione protetti |
| D | **Maturità delle capacità cyber della PA**: transizione Cloud (Polo Strategico Nazionale **PSN** + Public Cloud); classificazione dati PA (ordinari/critici/strategici) |
| E | **Protezione delle infrastrutture nazionali**: monitoraggio configurazioni BGP via IXP nazionali, infrastruttura **DNS nazionale**, monitoraggio configurazioni DNS/email PA |
| F | **Promozione della crittografia**: crittografia commerciale + sviluppo di **tecnologie/sistemi di cifratura nazionale** |
| G | **Contrasto alla disinformazione online** con coordinamento UE + Paesi like-minded |

### Obiettivo 2 — RISPOSTA (6 misure-categorie)

Risposta tempestiva e risolutiva a minacce, incidenti e crisi cyber nazionali.

| Lett. | Misura-categoria |
|---|---|
| A | **Sistema di gestione crisi cibernetica nazionale e transnazionale** assicurato dal [[entities/Nucleo per la Cybersicurezza\|NCS]]; architettura allineata al **Blueprint UE Raccomandazione 2017/1584**: livello politico (Presidente del Consiglio + Autorità delegata + CISR) + livello operativo (NCS + ACN) + livello tecnico ([[entities/CSIRT Italia\|CSIRT Italia]]) |
| B | **Integrazione dei servizi cyber nazionali**: **Hyper SOC** (raccolta/correlazione/analisi eventi da SOC + ISP), modalità di notifica unitaria al CSIRT, rete di **CSIRT/CERT settoriali federati** con CSIRT Italia, **ISAC** (Information Sharing and Analysis Center) centrale + ISAC settoriali, qualificazione aziende incident response |
| C | **Esercitazioni periodiche** di sicurezza cibernetica e resilienza (PSNC, UE, internazionali) |
| D | **Posizionamento nazionale su attribuzione** di attività cibernetiche ostili: contributo UE (**EU Cyber Diplomacy Toolbox**) + NATO (**Guide for Response Options to Malicious Cyber Activities**) |
| E | **Contrasto al cybercrime**: infrastrutture critiche + financial cybercrime + protezione minori + tutela personale |
| F | **Rafforzamento delle capacità di deterrenza** in ambito cibernetico |

### Obiettivo 3 — SVILUPPO (5 misure-categorie)

Sviluppo consapevole e sicuro delle tecnologie digitali, ricerca e competitività industriale.

| Lett. | Misura-categoria |
|---|---|
| A | **Centro Nazionale di Coordinamento (NCC)** ex Reg. UE 2021/887, coordinato con il Centro europeo di competenza cybersicurezza (**ECCC**); sinergie con Centri di competenza ad alta specializzazione e Digital Innovation Hub (DIH) |
| B | **Sviluppo di tecnologia nazionale ed europea**: riduzione dipendenza extra-UE, startup e PMI innovative |
| C | **"Parco nazionale della cybersicurezza"**: hub centrale + ramificazioni distribuite sul territorio; PA + industria + accademia; ricerca su IA, quantum computing/cryptography, robotica |
| D | **Meccanismi e soluzioni incentivanti** per sviluppo industriale/tecnologico/ricerca; creazione di **PSIRT** (Product Security Incident Response Team) da parte degli operatori privati |
| E | **Innovazione tecnologica e digitalizzazione** della PA e del tessuto produttivo (PNRR-driven) |

### Fattori abilitanti (2 trasversali)

| Fattore | Tema |
|---|---|
| **Cooperazione** | Coordinamento inter-istituzionale (CIC + ACN + autorità di settore + Forze di polizia + Difesa + Intelligence + MAECI per cyber diplomacy) + cooperazione UE/internazionale (ENISA, NIS CG, CyCLONe, rete CSIRT, NATO) |
| **Formazione e cultura della sicurezza** | Capacity building workforce cyber + awareness diffusa (cittadini, imprese, PA); approccio **whole-of-society** |

Nota: il Manuale Misura #82 (cfr. [[sources/ACN Manuale operativo Misura 82]]) usa una declinazione operativa con **4 fattori abilitanti** ribattezzati in modo più granulare: Formazione · Cultura · Cooperazione · **Metriche e KPI** (= la Misura #82 stessa che chiude le 82 misure del Piano).

## I 4 pilastri tecnico-operativi dell'architettura nazionale

La Strategia (riforma D.L. 82/2021) definisce **4 pilastri tecnico-operativi** dell'architettura nazionale cyber, ciascuno con un'amministrazione titolare:

| Pilastro | Titolare |
|---|---|
| **Cyber Sicurezza & Resilienza** | [[entities/ACN]] (pilastro nuovo, creato dal D.L. 82/2021) |
| **Prevenzione e contrasto della criminalità informatica** | Forze di polizia (Polizia di Stato/Servizio Polizia Postale, CNAIPIC, Arma dei Carabinieri/ROS, Guardia di Finanza/NSTPFT) |
| **Difesa e sicurezza militare dello Stato** | [[entities/Ministero della Difesa]] |
| **Ricerca ed elaborazione informativa** | Comparto intelligence (Sistema di informazione per la sicurezza della Repubblica) |

**Ruolo trasversale**: **cyber diplomacy** affidata all'Unità per le politiche e la sicurezza dello spazio cibernetico del **MAECI** (Ministero per gli Affari Esteri e la Cooperazione Internazionale).

## Strumenti finanziari per l'attuazione

| Strumento | Importo | Periodo |
|---|---|---|
| **Fondi nazionali** | **1,2% degli investimenti nazionali lordi** su base annuale | 2022-2026 |
| **Orizzonte Europa** | 95,51 miliardi di euro (bilancio totale UE) | 2021-2027 |
| **Europa Digitale** | 7,59 miliardi di euro (bilancio totale UE) | 2021-2027 |
| **PNRR Investimento 1.5 "Cybersecurity"** | **623 milioni di euro** (174M servizi cyber nazionali + 301,7M resilienza cyber PA + 147,3M laboratori scrutinio/certificazione) | 2021-2026 |

ACN come **Soggetto Attuatore** per l'Investimento 1.5 PNRR; **NCC** ex Reg. UE 2021/887 per fondi Orizzonte Europa ed Europa Digitale.

## Capacity building ACN

- Target reclutamento: **800 unità entro 2027** (campagne mirate dal 2022).
- Obiettivo dichiarato: arginare la fuga delle competenze cyber italiane all'estero + riportare talenti dall'estero.

## Cornice istituzionale (dettaglio post-re-ingest)

| Soggetto | Ruolo nella Strategia |
|---|---|
| **Presidente del Consiglio dei Ministri** | Adotta formalmente la Strategia (17/05/2022); trasmette al Parlamento la relazione annuale entro il **30 aprile** (D.L. 82/2021) |
| **Autorità delegata per la sicurezza della Repubblica** | Livello politico della gestione crisi cibernetica (Blueprint UE) |
| **[[entities/Comitato Interministeriale per la Cybersicurezza\|CIC]]** | Esercita l'**alta sorveglianza** sullo stato di attuazione della Strategia |
| **Comitato Interministeriale per la Sicurezza della Repubblica (CISR)** | Livello politico della gestione crisi cibernetica (Blueprint UE) |
| **[[entities/ACN]]** | Coordinatore operativo dell'attuazione; designata Autorità nazionale cyber + NIS PoC + Autorità certificazione cybersicurezza + NCC + elemento centrale PSNC |
| **[[entities/Nucleo per la Cybersicurezza\|NCS]]** | Livello operativo della gestione crisi cibernetica (Blueprint UE); supportato da ACN |
| **[[entities/CSIRT Italia\|CSIRT Italia]]** | Livello tecnico della gestione crisi cibernetica; dentro ACN |
| **[[entities/Ministero della Difesa]]** | Pilastro Difesa e sicurezza militare dello Stato nel dominio cyber; conduce operazioni cyber offensive/difensive |
| **MAECI — Unità per le politiche e la sicurezza dello spazio cibernetico** | Cyber diplomacy |
| **Forze di polizia** (Polizia Postale/CNAIPIC, Arma/ROS, Guardia di Finanza/NSTPFT) | Pilastro Prevenzione e contrasto criminalità informatica |
| **Comparto intelligence** | Pilastro Ricerca ed elaborazione informativa |
| **Comitato Tecnico Scientifico (CTS)** | Validato il Manuale Misura #82 il 29/11/2022 |
| **Amministrazioni coinvolte nel Piano** | Presidenza del Consiglio, Ufficio Consigliere Militare PCdM, Ministero dell'Istruzione, CINI, Atenei + Ministeri membri del CIC + Operatori privati |

## Mapping con il regime NIS2 italiano

- **D.Lgs. 138/2024 art. 9**: richiama esplicitamente la Strategia nazionale di cybersicurezza come uno dei pilastri del quadro nazionale di cybersicurezza.
- **Misure di Protezione della Strategia**: si sovrappongono in parte con le misure di sicurezza di base del [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19|det. ACN 379907/2025]] (es. supply chain, quadro giuridico, capacità PA — tutte ambiti dell'art. 21 NIS2).
- **Misure di Risposta della Strategia**: si sovrappongono con la disciplina della notifica incidenti ([[concepts/Notifica di incidente significativo]]) + linee guida di gestione incidenti ([[sources/Linee Guida NIS - Gestione incidenti - 2025-12]]).
- **Fattore Formazione**: si sovrappone con l'obbligo di awareness/training ex art. 21(2)(g) NIS2 + misura `PR.AT-*` del FNCDP.
- **Fattore Cooperazione**: si sovrappone con il [[entities/Tavolo per l'attuazione della disciplina NIS]] + cooperazione UE ([[entities/Gruppo di Cooperazione NIS]], [[entities/Rete di CSIRT nazionali]]).

**Direzionalità di aggancio**: la Strategia **precede** NIS2 (maggio 2022 vs settembre 2024); il D.Lgs. 138/2024 art. 9 la **incorpora** come pilastro nazionale. Quindi è la Strategia la cornice, NIS2 ne è una linea di attuazione (insieme a PSNC, CVD, ricerca, formazione, ecc.).

## Cornice UE

La Strategia 2022-2026 si allinea (per anno di adozione) con il quadro UE in evoluzione:

- **Direttiva NIS2** (dicembre 2022, sei mesi dopo la Strategia italiana).
- **Cyber Resilience Act (CRA)** (in preparazione 2022, adottato 2024).
- **Cyber Solidarity Act** (proposta 2023, in iter).
- **eIDAS 2.0** (Reg. UE 2024/1183).
- **Reg. UE 2024/2690** (esecuzione NIS2 per DSP — ottobre 2024).

La Strategia non poteva citare normativa di pubblicazione successiva (NIS2, CRA, ecc.), ma anticipava l'approccio (es. *"sicurezza della catena di approvvigionamento ICT"* coincide con art. 21(2)(d) NIS2).

## Punti chiave per la transizione GRC italiana

1. **Cornice di sistema**: per articoli pubblici sulla NIS2 italiana, citare la Strategia come *"cornice nazionale entro cui NIS2 si innesta"* è move di posizionamento (mostra comprensione del livello policy, oltre alle norme tecniche).

2. **Misura #82 = strumento ISO 27001 § 9.1**: la metodologia di KPI/indicatori della Misura #82 (cfr. Manuale) è una traduzione del Monitoring/Measurement/Analysis/Evaluation della clausola 9.1 ISO 27001. Per il consulente GRC che lavora con clienti PA, leggere la Strategia + il Manuale come *training material* per impostare il proprio framework di misurazione è investimento ad alto ROI.

3. **Cooperazione con Atenei + CINI**: la Strategia coinvolge esplicitamente il sistema universitario (CINI, Atenei) come attori responsabili. Per l'autore, **opportunità di networking** con CIS-Sapienza (autore del FNCDP) e CINI — coerente con l'opportunità già segnalata in [[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]] sezione "Asset di carriera non-certificativi".

4. **Calendario di rilevazione**: la rilevazione dei KPI parte dal **secondo anno** (2023); i target sono definiti annualmente. Wave 6 (maggio 2026) si colloca nel quarto anno di rilevazione — esistono almeno 3 cicli di KPI pubblicati che potrebbero essere fonti di articoli/analisi.

## Entità menzionate

- [[entities/ACN]] — coordinatore operativo
- [[entities/Comitato Interministeriale per la Cybersicurezza]] — alta sorveglianza
- Presidente del Consiglio dei Ministri — adozione formale
- Comitato Tecnico Scientifico (CTS) — validazione del Manuale Misura #82
- CINI (Consorzio Interuniversitario Nazionale per l'Informatica) — attore responsabile su misure di formazione/ricerca
- [[entities/Autorità di settore NIS]] — ministeri membri del CIC

## Concetti collegati

- [[concepts/Strategia nazionale di cybersicurezza]] — concept stub Wave 1, **aggiornato in Sessione 4** con sintesi della Strategia 2022-2026
- [[concepts/NIS2]] — uno dei pilastri operativi della Strategia
- [[concepts/Coordinated Vulnerability Disclosure]] — coperto dalla Strategia (cfr. art. 12 NIS2 + art. 33 D.Lgs. 138)
- [[entities/Framework Nazionale per la Cybersecurity]] — strumento operativo che la Strategia adotta come riferimento

## Synthesis collegate

- [[synthesis/Stratificazione delle norme cybersecurity in Italia]] — la Strategia è il livello "policy" sopra i regimi normativi specifici (PSNC, NIS2, DORA, Cloud PA, L. 90/2024).

## Note dell'agente

- *Sintesi dell'agente:* la Strategia 2022-2026 è il **livello policy** italiano. Non è atto regolatorio (non determina rientro NIS, non impone misure puntuali) ma è il **documento di indirizzo** dal quale derivano successivamente: D.L. 82/2021 (istituzione ACN), D.Lgs. 138/2024 (recepimento NIS2), L. 90/2024 (perimetro nazionale PA), determinazioni ACN, e così via.
- *Sintesi dell'agente:* la coincidenza temporale **maggio 2022 (Strategia) → dicembre 2022 (NIS2 UE)** è significativa: l'Italia ha adottato la propria Strategia nazionale *prima* dell'emissione di NIS2, quindi NIS2 è stato "inserito" nella cornice strategica preesistente — non viceversa. Pattern coerente con quanto osservato per il FNCDP (adottato dalla det. ACN, non viceversa — cfr. [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]] razionale (ii) del callout tesi).
- *Open question — futuro nodo*: la **Strategia successiva 2027-2031** (presumibile) e il suo Piano di Implementazione potrebbero integrare NIS2 nativamente, anziché come overlay sulla Strategia 2022-2026. Da monitorare per future wave.
- ✅ **Lacuna nota tecnica risolta (re-ingest 2026-05-19)**: l'autore ha ricaricato il PDF in versione testuale (5.16 MB, 1040 righe testo estratto, 27 pp). Contenuto del nodo aggiornato direttamente dalle estrazioni testuali del documento ufficiale. Citazioni puntuali ora possibili.
