# Index — LLM Wiki

> Catalogo content-oriented dell'intera wiki. Aggiornato a ogni ingest/lint.
> Contatori `(N)` aggiornati automaticamente dall'agente.

**Ultimo aggiornamento:** 2026-10-27 (correzione di contenuto: ambito PA, DEC-007; contatori invariati)
**Dominio attivo:** NIS2 — Direttiva (UE) 2022/2555, D.Lgs. 138/2024, corpus regolatorio ACN, + Reg. UE 2024/2690 (DSP), + ENISA TIG/Mapping Table/Mapping NIS2-ECSF, + NIST CSF 2.0, + ISO/IEC 27000-series, + FNCDP 2025 v2.1, + ECSF, **+ L. 90/2024 (cybersicurezza nazionale + reati informatici)**.
**Scope tagging**: tutti i nodi toccati dai cluster Wave 6 + Wave 7 carry `scope:` (`nis2_tool` / `grc_personal` / `both`) nel frontmatter — vedi [[_meta/wave_reports/Wave_6_2026-05-18]] e [[_meta/wave_reports/Wave_6_5_PLANNED]].

---

## Sources (40)

### Wave 1 — Normativa primaria
- [[sources/Direttiva (UE) 2022-2555 (NIS2)]] — *direttiva UE che fissa il framework NIS2 (atto UE primario)* — 2022-12-14
- [[sources/D.Lgs. 138-2024 (Decreto NIS)]] — *recepimento italiano: ACN unica autorità + Tavolo NIS, obblighi e sanzioni* — 2024-09-04
- [[sources/La normativa NIS - Pagina ACN]] — *pagina-panoramica ACN: indice vivente del corpus regolatorio NIS* — 2024-10-16

### Wave 2 — Determinazioni ACN
- [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]] — *Allegati 1-4: misure e incidenti di base + regimi transitori OSE/telco* — 2025-12-19
- [[sources/Determinazione ACN piattaforma e procedure - 2026-04-13]] — *piattaforma, ruoli, calendario annuale, verifiche di coerenza* — 2026-04-13
- [[sources/Determinazione ACN categorizzazione - 2026-04-13]] — *10 macro-aree, 4 categorie di rilevanza, automatismo PSNC* — 2026-04-13
- [[sources/Determinazione ACN termini soggetti 2026 - 2026-04-30]] — *termini speciali coorte 2026: misure 31/07/2027, notifica 1/01/2027* — 2026-04-30
- [[sources/Determinazione ACN accordi condivisione - 2025-04-10]] — *notifica accordi ex art. 17 via piattaforma, finestra 15 apr–31 mag* — 2025-04-10
- [[sources/Determinazione ACN funzionamento Tavolo NIS - 2025-07-16]] — *regolamento interno: convocazione, quorum, deliberazione, durata, salvaguardia DORA* — 2025-07-16
- [[sources/Determinazione ACN composizione Tavolo NIS - 2026]] — *aggiornamento composizione (sost. Vinciguerra al MEF)* — 2026
- [[sources/Linee Guida NIS - Gestione incidenti - 2025-12]] — *modello a 5 fasi NIST SP 800-61r3, mappatura misure-fasi (Appendici A-B)* — 2025-12

### Wave 3 — Allegati tecnici (det. 379907/2025 + det. categorizzazione)
- [[sources/Allegato 1 - Misure di sicurezza di base per i soggetti importanti]] — *~26 misure su 6 funzioni FNCDP/NIST CSF v2.0, 16 ambiti politiche, 6 requisiti non derogabili* — 2025-12-19
- [[sources/Allegato 2 - Misure di sicurezza di base per i soggetti essenziali]] — *strict super-set: +6 misure aggiuntive + VA/PT obbligatori, test ripristino backup, hardening* — 2025-12-19
- [[sources/Allegato 3 - Incidenti significativi di base per i soggetti importanti]] — *3 codici IS-1/2/3 con soglie qualitative auto-determinate ex `DE.CM-01`* — 2025-12-19
- [[sources/Allegato 4 - Incidenti significativi di base per i soggetti essenziali]] — *4 codici (+IS-4 accesso non autorizzato/abuso privilegi)* — 2025-12-19
- [[sources/Allegato 1 modello - Categorizzazione soggetti art. 2 c. 2]] — *10 macro-aree con categoria di rilevanza pre-assegnata (Logistica = basso)* — 2026-04-13
- [[sources/Allegato 2 modello - Categorizzazione soggetti art. 2 c. 3]] — *identico modello 1 tranne Logistica = minimo* — 2026-04-13

### Wave 6 — Corpus UE + standard internazionali (Cluster A + B + C + D + parte E chiusi)
- [[sources/Regolamento di esecuzione UE 2024-2690]] — *atto UE direttamente applicabile: requisiti tecnici art. 21 NIS2 + soglie quantitative incidenti significativi per 11 categorie DSP; abroga Reg. (UE) 2018/151 NIS1* — 2024-10-17
- [[sources/ENISA Technical Implementation Guidance v1.0 - 2025-06-26]] — *TIG soft-law ENISA: guidance + examples of evidence + tips per ciascuno dei 13 requisiti dell'Allegato Reg. 2024/2690* — 2025-06-26
- [[sources/ENISA Mapping Table v1.0 - 2025-06-26]] — *mapping ENISA del Reg. UE 2024/2690 verso ISO 27001:2022, NIST CSF 2.0, ETSI EN 319 401, CEN/TS 18026:2024, national frameworks; xlsx ufficiale scaricato in raw/assets/* — 2025-06-26
- [[sources/ECSF Role Profiles - 2022-09]] — *European Cybersecurity Skills Framework ENISA, 12 profili professionali standard (CISO, Compliance Officer, Auditor, Risk Manager, ecc.); CC-BY 4.0* — 2022-09
- [[sources/ENISA Mapping NIS2 obligations with ECSF role profiles - 2025-06-26]] — *mapping obblighi NIS2 art. 21/23 ↔ 12 profili ECSF; 2 use cases (implementazione misure + post-incident); CC-BY 4.0* — 2025-06-26
- [[sources/NIST CSF 2.0 - 2024-02-26]] — *NIST CSWP 29, framework outcome-based con 6 funzioni (GOVERN nuova in 2.0); fonte upstream del FNCDP italiano* — 2024-02-26
- [[sources/ISO IEC 27000-2018]] — *Vocabolario ISMS (5th edition 2018-02); publicly available* — 2018-02
- [[sources/ISO IEC 27001-2022]] — *Requirements ISMS certificabile (3rd edition 2022-10); 93 controlli Annex A in 4 gruppi; provenance non ufficiale* — 2022-10
- [[sources/ISO IEC 27002-2022]] — *Catalogo controlli ISMS (3rd edition 2022-02); 93 controlli, 5 attributi, 11 controlli nuovi vs 2013; provenance non ufficiale* — 2022-02
- [[sources/FNCDP 2025 v2.1 Core]] — *Framework Nazionale italiano edizione 2025 v2.1; derivato da NIST CSF 2.0 + 9 sottocategorie `DP-*` (data protection) + categoria nuova `DP-ID.DM`; chiude la lacuna nota Wave 1+5* — 2025
- [[sources/ACN Strategia nazionale di cybersicurezza 2022-2026]] — *Strategia adottata 17/05/2022 dal PCdM; 3 obiettivi (Protezione/Risposta/Sviluppo) + 4 fattori abilitanti; Piano di Implementazione con 82 misure; richiamata dal D.Lgs. 138 art. 9* — 2022-05-17
- [[sources/ACN Manuale operativo Misura 82]] — *Manuale ACN v3.0 (08/03/2023) per la Misura #82 = KPI di tutte le 82 misure della Strategia; tre livelli di affidabilità indicatori; pendant ISO 27001 § 9.1* — 2022-12-05
- [[sources/ENISA Handbook for Cyber Stress Tests v2.0 - 2025-05]] — *ENISA Handbook v2.0 maggio 2025, cross-settore (salute/finanza/energia); case studies ECB 2024 + CER 2024; strumento facoltativo di vigilanza* — 2025-05

### Wave 5 — Meta-documenti interpretativi (1 di 3 — A1)
- [[sources/Guida lettura specifiche di base]] — *meta-documento ACN: 37/87 importanti, 43/116 essenziali, 4 clausole basate sul rischio, modello tridimensionale incidenti, mappatura art. 24 c.2, 11 documenti del board* — 2025-09 (ed. 2.1 2026-04)

### Wave 7 — Cybersicurezza nazionale italiana (L. 90/2024)
- [[sources/Legge 90-2024 (cybersicurezza nazionale)]] — *legge unitaria 24 articoli su 2 capi: Capo I cybersicurezza/PA/procurement (artt. 1-15-bis); Capo II reati informatici (artt. 16-23); art. 15-bis chiave del coordinamento NIS1→NIS2* — 2024-06-28

### Wave 4 — FAQ ACN (8)
- [[sources/FAQ NIS - Profili generali]] — *panoramica del regime NIS, ruoli, calendario e roadmap normativa* — 2026
- [[sources/FAQ NIS - Ambito]] — *criteri di rientro/esclusione (`AMB.SI.*`/`AMB.NO.*`); chiarimento DORA → solo art. 7 c. 1 per Allegato I p. 3-4* — 2026
- [[sources/FAQ NIS - Settori, sottosettori e tipologie di soggetto]] — *~70 chiarimenti settoriali con NACE, size-blind, eccezioni di prevalenza, identificazione autoritativa Allegato IV* — 2026
- [[sources/FAQ NIS - Registrazione]] — *procedura su Portale ACN, gruppi di imprese, PA, rappresentante UE* — 2026
- [[sources/FAQ NIS - Ruoli e procedure]] — *catena CDA → pdc → referente CSIRT, tabella riassuntiva 8 ruoli, esternalizzazione esplicita* — 2026
- [[sources/FAQ NIS - Categorizzazione]] — *modello 10 macro-aree, 4 categorie minimo→alto, processo 3 fasi, coordinamento Cloud PA + PSNC; conferma protocolli **155238/2026** e **127437/2026*** — 2026
- [[sources/FAQ NIS - Misure di sicurezza e notifica di incidenti]] — *misure di sicurezza di base, notifica scaglionata, soglie di significatività operative* — 2026
- [[sources/FAQ NIS - Aggiornamento delle informazioni]] — *finestra annuale, aggiornamento continuo, tassonomia CPV fornitori rilevanti (codici `FRN.*`)* — 2026

*Wave 1 + Wave 2 + Wave 3 + Wave 4 chiuse. Wave 5 A1 chiusa. A3 (slide Sapienza) → **skip definitivo** (cfr. [[_meta/skipped_documents]]). **Wave 6 COMPLETED** (2026-05-19): tutti i Cluster A+B+C+D+E+F chiusi (Sessioni 1-4 + 3 mini-fix housekeeping). Wave 6.5 chiusa (retrofit scope completo, 98/98 nodi taggati). **Wave 7 CHIUSA** (2026-05-23): ingest L. 90/2024 con coordinamento esplicito NIS2 (synthesis dedicata + ridireccionamento art. 15-bis). Cfr. [[_meta/wave_reports/Wave_6_2026-05-18]], [[_meta/wave_reports/Wave_6_5_2026-05-19]] per dettagli storici.*

---

## Entities (17)

### Istituzioni
- [[entities/ACN]] — *Agenzia per la Cybersicurezza Nazionale: autorità competente NIS + SPOC + CSIRT* — 12 fonti
- [[entities/CSIRT Italia]] — *funzione di risposta agli incidenti dentro ACN* — 6 fonti
- [[entities/ENISA]] — *agenzia UE per la cibersicurezza, ruolo accresciuto sotto NIS2* — 2 fonti
- [[entities/Tavolo per l'attuazione della disciplina NIS]] — *foro permanente di raccordo tra ACN e 9 ministeri di settore* — 5 fonti
- [[entities/Comitato Interministeriale per la Cybersicurezza]] — *CIC, livello politico-strategico nazionale* — 1 fonte
- [[entities/Nucleo per la Cybersicurezza]] — *gestione operativa delle crisi cyber nazionali* — 1 fonte
- [[entities/Gruppo di Cooperazione NIS]] — *consesso UE strategico (Art. 14 NIS2)* — 2 fonti
- [[entities/EU-CyCLONe]] — *rete UE liaison per gestione crisi cyber su larga scala* — 2 fonti
- [[entities/Rete di CSIRT nazionali]] — *rete UE operativa-tecnica dei CSIRT* — 2 fonti
- [[entities/Autorità di settore NIS]] — *i 9 ministeri designati ex Art. 12 D.Lgs. 138/2024* — 1 fonte
- [[entities/Ministero della Difesa]] — *autorità di settore + coordinamento crisi cyber per sicurezza nazionale* — 1 fonte
- [[entities/Comitato per la Cybersicurezza]] — *organo tecnico-consultivo presso PCM* — 1 fonte

### Ruoli operativi NIS
- [[entities/Punto di contatto NIS]] — *ruolo amministrativo del soggetto sulla piattaforma ACN (art. 4 det. piattaforma)* — 4 fonti
- [[entities/Referente CSIRT]] — *ruolo operativo per notifica incidenti, designazione 31 dic, esonero DORA* — 4 fonti
- [[entities/Rappresentante NIS in Italia]] — *per soggetti extra-UE ex art. 5 c.1 lett. b), finestra 1 set–30 nov* — 2 fonti

### Standard e framework
- [[entities/Framework Nazionale per la Cybersecurity]] — *FNCDP edizione 2025 (CIS Sapienza + CINI + ACN), base delle misure di sicurezza di base* — 3 fonti
- [[entities/NIST SP 800-61]] — *r2/r3, base del modello a 5 fasi del processo di gestione incidenti* — 2 fonti

---

## Concepts (39)

### Framework e ambito
- [[concepts/NIS2]] — *etichetta dell'intero framework UE/IT per la cybersicurezza dei soggetti critici* — 3 fonti
- [[concepts/Ambito di applicazione NIS2]] — *intersezione di settori, dimensione e categorie speciali* — 2 fonti
- [[concepts/Settori altamente critici e critici]] — *Allegati I (11) e II (7) — driver settoriale di NIS2; FAQ con NACE, size-blind, eccezioni prevalenza* — 3 fonti

### Soggetti
- [[concepts/Soggetti essenziali e importanti]] — *classificazione binaria che determina obblighi, vigilanza e sanzioni* — 4 fonti
- [[concepts/Identificazione dei soggetti NIS]] — *procedura annuale di registrazione + classificazione su piattaforma ACN* — 8 fonti
- [[concepts/Size-cap rule]] — *criterio dimensionale automatico per l'applicabilità di NIS2 (soglie Racc. 2003/361/CE ex `AMB.DI.1`)* — 3 fonti
- [[concepts/Categorizzazione dei soggetti]] — *sotto-classificazione interna ex Art. 30 D.Lgs. 138/2024 + processo 3 fasi FAQ + coordinamento Cloud PA/PSNC* — 4 fonti
- [[concepts/Macro-aree NIS]] — *10 macro-aree della categorizzazione (Allegati 1-2 det. categorizzazione)* — 1 fonte
- [[concepts/Categorie di rilevanza]] — *4 categorie: minimo→alto + automatismo PSNC + ordine confermato da `CAT.6`* — 2 fonti
- [[concepts/Soggetti PSNC-NIS]] — *doppia disciplina perimetro nazionale + NIS, impatto alto automatico* — 3 fonti

### Misure e incidenti
- [[concepts/Misure di gestione del rischio cyber]] — *10 ambiti minimi obbligatori (Art. 24) + mappatura art. 24 c.2 → codici misure (Appendice A guida)* — 5 fonti
- [[concepts/Approccio multi-rischio]] — *all-hazards: cyber + fisico + ambientale + umano; copre anche incidenti accidentali* — 3 fonti
- [[concepts/Misure di sicurezza di base]] — *Allegati 1-2 det. 379907/2025: **37/87 importanti, 43/116 essenziali** (numeri ancorati); roadmap base→aggiuntive→lungo termine* — 5 fonti
- [[concepts/Notifica di incidente significativo]] — *obbligo scaglionato 24h-72h-1mese al CSIRT; termini decorrono dall'acquisizione dell'evidenza* — 8 fonti
- [[concepts/Incidente significativo]] — *soglia che fa scattare l'obbligo di notifica (Art. 23(3) NIS2)* — 2 fonti
- [[concepts/Incidenti significativi di base]] — *Allegati 3-4 det. 379907/2025 + modello tridimensionale condizione/compromissione/oggetto* — 2 fonti
- [[concepts/Processo gestione incidenti NIS]] — *modello 5 fasi NIST SP 800-61r3 (preparazione/rilevamento/risposta/ripristino/miglioramento)* — 3 fonti
- [[concepts/Sistemi informativi e di rete rilevanti]] — *scoping primario delle misure: processo 3 step + elenco ex `GV.OC-04`* — 4 fonti
- [[concepts/Clausole basate sul rischio]] — *le 4 clausole standardizzate che modulano i requisiti delle misure di base* — 4 fonti
- [[concepts/Evidenze documentali NIS]] — *6 tipologie documentali + 11 documenti che richiedono delibera del board (Appendice C guida)* — 4 fonti

### Specifiche tecniche
- [[concepts/Specifiche tecniche di base]] — *determinazioni del Direttore generale ACN ex Art. 27* — 17 fonti
- [[concepts/Regime transitorio OSE]] — *art. 5 det. 379907: mantenimento misure D.Lgs. 65/2018 limitatamente a sistemi OSE* — 2 fonti
- [[concepts/Regime transitorio telco]] — *art. 6 det. 379907: mantenimento DM 12/12/2018 + soglie incident telco* — 2 fonti

### Procedure su piattaforma
- [[concepts/Piattaforma digitale ACN]] — *single point of entry per registrazione, notifica, categorizzazione* — 4 fonti
- [[concepts/Aggiornamento annuale informazioni]] — *finestra 15 aprile–31 maggio, lista art. 16 det. piattaforma; FAQ `FRN.*` su CPV fornitori rilevanti* — 3 fonti
- [[concepts/Aggiornamento continuo informazioni]] — *entro 14 giorni dalla modifica (artt. 7 c.7 + 19 det. piattaforma)* — 1 fonte
- [[concepts/Verifiche di coerenza]] — *art. 14 det. piattaforma, 30+20gg, no silenzio-assenso* — 2 fonti
- [[concepts/Verifiche di conformità categorizzazione]] — *art. 21 det. piattaforma + art. 30 c.3 D.Lgs., 90+60gg con silenzio-assenso* — 2 fonti
- [[concepts/Accordi di condivisione delle informazioni]] — *art. 17, notifica obbligatoria a ACN, finestra 15 apr–31 mag* — 2 fonti
- [[concepts/Fornitori rilevanti NIS]] — *criteri di rilevanza ICT/non fungibilità + tassonomia CPV (FAQ `FRN.2-4`)* — 3 fonti

### Trasversali e governance
- [[concepts/Sanzioni NIS2]] — *€ 10M/2% essenziali, € 7M/1,4% importanti, € 25-125k PA + misure non pecuniarie; § L. 90 + PSNC armonizzati* — 3 fonti
- [[concepts/Strategia nazionale di cybersicurezza]] — *documento di indirizzo politico-strategico* — 1 fonte
- [[concepts/Clausola di salvaguardia]] — *eccezioni per sicurezza nazionale, difesa, ordine pubblico* — 4 fonti
- [[concepts/Coordinamento DORA-NIS]] — *esoneri specifici per entità finanziarie + salvaguardia DORA nel Tavolo NIS + FAQ `AMB.NO.2`* — 4 fonti
- [[concepts/Coordinated Vulnerability Disclosure]] — *processo coordinato per la divulgazione delle vulnerabilità (Art. 12 NIS2)* — 2 fonti
- [[concepts/Responsabilità degli organi di gestione]] — *obblighi di approvazione, supervisione, formazione + 11 documenti che richiedono delibera del board (Appendice C guida); FAQ ODA chiariscono governance non standard* — 5 fonti

### Cybersicurezza nazionale italiana (L. 90/2024)
- [[concepts/Perimetro Legge 90-2024]] — *ambito soggettivo tassativo art. 1 c. 1: PA centrali + locali grandi + trasporto qualificato + ASL + in house qualificate; esclusioni art. 1 c. 7* — 2 fonti
- [[concepts/Referente per la cybersicurezza (L. 90-2024)]] — *art. 8 L. 90: struttura cyber con 7 funzioni + referente con specifiche professionalità; cumulo con pdc NIS e RTD CAD* — 2 fonti
- [[concepts/Elementi essenziali di cybersicurezza (procurement)]] — *art. 14 L. 90 + DPCM atteso 120gg: criteri CIA + tetto 10% punteggio economico + premialità Buy EU/NATO* — 1 fonte

---

## Synthesis (7)

- [[synthesis/Cronologia attuativa NIS2 in Italia]] — *qual è la cronologia attuativa del regime NIS2 in Italia?* — 2026-04-29
- [[synthesis/Stratificazione delle norme cybersecurity in Italia]] — *in quale regime ricade un soggetto e cosa deve fare? Come si coordinano PSNC, NIS2, DORA, Cloud PA, L. 90/2024?* — 2026-04-29 (aggiornata 2026-05-23 § 5 L. 90)
- [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]] — *come si coordinano Reg. UE 2024/2690 (DSP) e Det. ACN 379907/2025 per un fornitore italiano di cloud computing? Q1-Q4 ristrette via TIG ENISA* — 2026-05-18
- [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]] — *la TIG ENISA v1.0 risolve le 4 open question della synthesis di coordinamento? Tutte ristrette, nessuna chiusa per vincolo soft-law* — 2026-05-18
- [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] — *come tradurre tra art. 21 NIS2, NIST CSF 2.0, FNCDP 2025 v2.1, ISO 27001:2022, ISO 27002:2022? v2 con FNCDP integrato (Wave 6 Sessione 3)* — 2026-05-19
- [[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]] — *quali profili ECSF per la transizione GRC di Andrea? Tripletta Compliance Officer + Auditor + Risk Manager + roadmap certificazioni 24-36 mesi* — 2026-05-19
- [[synthesis/Coordinamento L. 90-2024 e NIS2]] — *come si coordinano L. 90/2024 e D.Lgs. 138/2024 per un soggetto pubblico italiano? T3 = esclusione asimmetrica art. 1 c. 7 + cumulo ruoli pdc/referente art. 4 c. 8 det. piattaforma* — 2026-05-23

---

## Convenzioni rapide

- `[[sources/...]]` — pagine di sintesi delle fonti raw
- `[[entities/...]]` — persone, luoghi, organizzazioni, prodotti, opere
- `[[concepts/...]]` — idee, framework, teorie
- `[[synthesis/...]]` — analisi derivate, risposte filed-back

Schema completo in [[CLAUDE]].
