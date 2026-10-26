---
title: ENISA — Handbook for Cyber Stress Tests v2.0
type: source
scope: grc_personal
source_type: article
source_path: raw/articles/2025.04311_01_ms_v2.0_Handbook for Cyber Stress Tests_en.pdf
url: https://www.enisa.europa.eu/publications/handbook-for-cyber-stress-tests
author: ENISA (European Union Agency for Cybersecurity)
date_published: 2025-05
date_ingested: 2026-05-19
tags: [enisa, stress-test, resilience, cybersecurity, cross-settore, supervision-toolkit, salute, finanza, energia]
aliases: [ENISA Stress Test Handbook, Cyber Stress Tests Handbook v2.0]
---

## TL;DR

**Handbook ENISA per i Cyber Stress Tests, versione 2.0 di maggio 2025** (ISBN 978-92-9204-700-9, DOI 10.2824/8248517, **CC-BY 4.0**, ~25 pp). Versione precedente: febbraio 2025 (marcato "DRAFT | APRIL 2025" in alcune intestazioni del PDF — segno di revisione iterativa rapida).

**Autore verificato**: **ENISA** (non ECB/SSM come ipotizzato dal codice file `2025.04311_01_ms_v2.0`). Ambito **cross-settore** (Annex A: settore salute; Annex B: finanza + energia). Decisione di pre-ingest verification: **INGEST come `grc_personal`**, coerente con il pacchetto ENISA del 2025.

Definizione operativa di **cyber stress test** ENISA (citazione testuale, <15 parole):

> *"a targeted assessment of the resilience of individual organisations."* (ENISA Handbook for Cyber Stress Tests v2.0 p. 3 — 9 parole)

(Trad. agente: *"valutazione mirata della resilienza delle singole organizzazioni e della loro capacità di sostenere e recuperare da incidenti significativi di cybersicurezza, garantendo la fornitura di servizi critici in vari scenari di rischio"* — paraphrasi della definizione completa che eccede il limite di 15 parole.)

Per la wiki, è un **complemento di metodologia operativa** alla NIS2: non riguarda il rientro nell'ambito (cui mira il NIS2 Tool), ma riguarda **come testare la resilienza** una volta dentro l'ambito. È strumento per autorità di vigilanza (ACN inclusa) e per soggetti NIS che vogliono auto-valutarsi.

## Struttura

| Sezione | Contenuto |
|---|---|
| Introduction | Scope, target audience, policy context |
| Stress testing for cybersecurity and resilience | Definizione stress test + uso come supervision toolkit |
| Step-by-step guide for cyber stress testing | Metodologia operativa step-by-step |
| National, regional and union cyber stress tests | Esempi di stress test multi-livello |
| Conclusions | — |
| **Annex A** | Esempio del **settore salute** |
| **Annex B** | Case studies su **finanza** (ECB 2024 cyber resilience stress test) + **energia** (2024 hybrid threat stress test ex CER Directive) |
| References | — |

## Contesto storico e policy

Gli stress test nascono nella **regolamentazione bancaria** dopo la crisi finanziaria 2007-2009 (Basel Committee on Banking Supervision). Lo schema viene poi adattato alla cybersicurezza:

- **2022**: Bank of England — cyber stress test dei retail payment services UK.
- **2024**: **ECB** — large cyber resilience stress test delle banche UE (riferimento esplicito Annex B).
- **2024**: **Commissione Europea + Member States** — EU coordinated stress test sulla resilienza del settore energia (in scope **Critical Entities Resilience Directive — CER**, non NIS2).

ENISA pubblica questo Handbook come **toolkit per autorità di vigilanza** che vogliono replicare l'esercizio in altri settori.

## Definizione di cyber stress test (ENISA)

Caratteristiche distintive:

- **Targeted assessment**: non è audit generale, ma valutazione su scenari specifici.
- **Resilience-focused**: misura sia la **preparedness** (misure preventive) sia la **recovery** (capacità di ripristino).
- **Lightweight rispetto agli audit completi**: è un *exercise*, non una *certification*.
- **Scenari di rischio**: per ciascun test si definisce uno *scenario plausibile ma improbabile* di crisi (es. *"perdita simultanea di N data center"*, *"compromissione di un fornitore critico"*).
- **Resilience metrics**: misure di tempo di ripristino (RTO), capacità residua di servizio, escalation, comunicazione.

## Mapping con il regime NIS2

| Aspetto NIS2 | Coerenza con stress test ENISA |
|---|---|
| Art. 21(2)(c) NIS2 — Business continuity, backup, disaster recovery, crisis management | **Allineamento diretto**. Lo stress test verifica empiricamente l'efficacia di BC/DR/crisi |
| Det. ACN 379907/2025 misure `ID.IM-04` (BC/DR/crisi), `RC.RP-01` (Recovery planning) | Lo stress test è la *prova sul campo* di queste misure |
| Tempistiche notifica art. 25 D.Lgs. 138/2024 (24h/72h/1 mese) | Lo stress test può verificare il rispetto delle tempistiche in scenario simulato |
| Vigilanza ACN ex art. 32 D.Lgs. 138/2024 | ENISA suggerisce stress test come strumento di vigilanza — potenzialmente adottabile da ACN in futuro |

**Non è obbligatorio**: la NIS2 non impone stress test. Sono **strumento facoltativo** che le autorità di vigilanza nazionali possono adottare per integrare gli obblighi di base.

## Settori coperti nei case study

### Annex A — Salute

Settore sanitario: ENISA fornisce un esempio dettagliato di stress test per ospedali / fornitori sanitari. Coerente con il fatto che la **sanità è uno dei settori NIS2 altamente critici** (Allegato I NIS2).

### Annex B — Finanza ed energia

- **Finanza — ECB 2024 Cyber Resilience Stress Test**: test su circa 109 banche UE (perimetro SSM). Settore disciplinato da **DORA** + NIS2 (con primato DORA cfr. [[concepts/Coordinamento DORA-NIS]]). Lo stress test ECB è coordinato dal Single Supervisory Mechanism.
- **Energia — 2024 Hybrid Threat Stress Test**: in scope della **Critical Entities Resilience Directive (CER)** — direttiva UE 2022/2557, parallela a NIS2 per la resilienza fisica delle infrastrutture critiche. Non è in wiki (out-of-scope NIS2).

## Punti chiave per la transizione GRC italiana

1. **Strumento di consulenza spendibile**: per consulenti che lavorano con clienti NIS2 maturi (già conformi e operativi), proporre uno stress test annuale è un **upselling logico** dopo il primo ciclo di compliance. Mercato emergente in Italia.

2. **Coerenza con ISO 27001 § 8.1 (Operational planning and control) + § 8.3 (Risk treatment)**: lo stress test è la verifica funzionale dell'efficacia dei controlli ISO 27001 Annex A in condizione di stress, non in stato nominale.

3. **Pattern adattabile a NIS2 Tool**: una *"modalità stress test"* del tool potrebbe simulare gli effetti di scenari multi-fattori sul verdetto del soggetto (es. *"se il tuo fornitore cloud è compromesso, qual è il tuo nuovo posizionamento NIS2?"*). Outlook a 12-24 mesi.

4. **Networking opportunity**: ENISA è il pubblicatore + ACN partecipa al NIS Cooperation Group. Una proposta italiana di stress test settoriale (es. PA, telco) tramite ACN potrebbe essere veicolo di visibilità per consulenti specializzati.

5. **Mercato bancario/SSM**: il caso ECB 2024 è il riferimento più maturo. Per consulenti che vogliono entrare nel **settore finanziario italiano**, lo stress test ECB è una porta di ingresso credibile (anche se DORA-driven più che NIS2-driven).

## Entità menzionate

- [[entities/ENISA]] — autore
- ECB (European Central Bank) — caso 2024
- Bank of England — caso 2022
- Commissione europea + Member States — caso 2024 energia
- Basel Committee on Banking Supervision — origini concettuali

## Concetti collegati

- [[concepts/Misure di sicurezza di base]] — `ID.IM-04`, `RC.RP-01` (BC/DR/recovery) sono i pendant micro che lo stress test verifica
- [[concepts/Processo gestione incidenti NIS]] — il modello 5 fasi NIST 800-61r3 può essere scenario di stress test
- [[concepts/Coordinamento DORA-NIS]] — il caso ECB 2024 è in regime DORA, non NIS2
- [[concepts/Notifica di incidente significativo]] — le tempistiche 24h/72h/1m sono verificabili tramite stress test

## Synthesis collegate

- [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] — lo stress test è una capability operativa che attraversa più sezioni del cross-walk (gestione incidenti, BC/DR, crisi)
- [[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]] — il profilo **Cybersecurity Auditor** (P6) può evolvere verso "Cyber Stress Test Coordinator" come specializzazione

## Note dell'agente

- *Sintesi dell'agente:* gli stress test cyber sono **una nicchia in crescita** in UE. Il primo caso ECB del 2024 e l'Handbook ENISA del 2025 sono segnali che la pratica si stia istituzionalizzando. Per l'autore, è una **direzione di specializzazione futura** (anni 3-5 post-percorso ISO LA), non immediata. Da monitorare l'evoluzione in Italia (ACN potrebbe pubblicare un proprio handbook adattato).
- *Sintesi dell'agente:* l'Handbook v2.0 è documento **giovane** (maggio 2025) e **a perimetro variabile**: copre salute, finanza, energia ma non telco, PA, manufacturing. Verosimilmente versioni future amplieranno i settori. Outlook v3.0 atteso entro 12-18 mesi.
- **Skip considerato e respinto**: il brief Sessione 4 prevedeva possibile skip se autore = ECB/SSM. La verifica autore ha rivelato ENISA → ingest legittimo. Documento utile per il GRC personale dell'autore anche se non determinante per il NIS2 Tool.
- *Open question*: la **revisione interna ACN su stress test cyber** (se esiste) non è stata identificata. Possibile lacuna; futuro outlook.
