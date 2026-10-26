---
title: ENISA Technical Implementation Guidance v1.0 (TIG) — Reg. UE 2024/2690
type: source
source_type: article
source_path: raw/articles/ENISA_Technical_implementation_guidance_on_cybersecurity_risk_management_measures_version_1.0.pdf
url: https://www.enisa.europa.eu/publications/nis2-technical-implementation-guidance
author: ENISA (autori Konstantinos Moulinos, Marianthi Theocharidou) — in collaborazione con la Commissione europea e il Gruppo di cooperazione NIS
date_published: 2025-06-26
date_ingested: 2026-05-18
tags: [nis2, enisa, guidance, reg-ue-2024-2690, art-21, misure-gestione-rischio, dsp, cloud, dns, mssp, msp, soft-law]
scope: grc_personal
aliases: [ENISA TIG v1.0, Technical Implementation Guidance, TIG 2024/2690, NIS2 TIG]
---

## TL;DR

Guidance ENISA v1.0 di giugno 2025 (ISBN 978-92-9204-704-7, DOI 10.2824/2702548) sull'implementazione del [[sources/Regolamento di esecuzione UE 2024-2690|Reg. UE 2024/2690]]. **Non vincolante** (soft-law, *advisory character*); contiene per ciascuno dei requisiti tecnici e metodologici dell'Allegato Reg.: (1) **guidance** = consigli operativi, (2) **examples of evidence** = tipi di evidenza che attestano l'implementazione, (3) **tips** = considerazioni aggiuntive (non sempre presenti). Struttura uno-a-uno sulle 13 sezioni dell'Allegato Reg. + 2 appendici (national frameworks + glossary). 170 pagine. Mapping ai principali standard internazionali (ISO/IEC 27001:2022, ISO/IEC 27002:2022, NIST CSF 2.0, ETSI EN 319 401, CEN/TS 18026:2024) e ai framework nazionali NIS2 — il mapping completo è nel file Excel ufficiale separato (cfr. [[sources/ENISA Mapping Table v1.0 - 2025-06-26]]).

Documento **interpretativo chiave** del Reg. UE 2024/2690 a livello UE. Per la wiki, è il pendant UE della [[sources/Guida lettura specifiche di base|guida ACN settembre 2025]] (interpretazione nazionale della det. 379907/2025). La sua lettura mirata risponde — in parte — alle Q1-Q4 della [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025|synthesis di coordinamento]]: cfr. [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]].

## Disclaimer ENISA (testuale, citato letteralmente)

> *"This document is not legally binding and is only of an advisory character. It is not intended to replace the frameworks, guidance, tools or other mechanisms provided by Member States at national level."*

> *"Member States retain the freedom to determine their approach to the supervision of the requirements under this implementing regulation."*

> *"Entities in scope of the regulation should check under whose jurisdiction they fall and they should follow any guidance by national competent authorities."*

Il disclaimer è giuridicamente **determinante** per il rapporto Reg. UE / regimi nazionali: la TIG si pone come strato interpretativo non sostitutivo, riconoscendo esplicitamente la coesistenza dei framework nazionali (in Italia: [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19|det. ACN 379907/2025]] + [[entities/Framework Nazionale per la Cybersecurity|FNCDP 2025]]). Cfr. [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]] (tesi 3a + 3c).

## Ambito soggettivo

Identico al Reg. UE 2024/2690 — le 11 categorie di soggetti pertinenti (DNS, TLD, **cloud**, data center, CDN, MSP, MSSP, marketplace, search engine, social network, trust service providers). La TIG nota che il documento "may provide indications... considered useful by other public or private bodies for improving their cybersecurity" → cioè è utilizzabile come riferimento informale anche fuori dell'ambito Reg.

## Struttura — 13 capitoli mappati uno-a-uno sull'Allegato Reg.

| Cap. | Titolo TIG | Lett. art. 21(2) NIS2 | Sotto-sezioni |
|---|---|---|---|
| 1 | Policy on the security of network and information systems | a) | 1.1 Policy + 1.2 Roles/responsibilities |
| 2 | Risk management policy | a) | 2.1 Framework + 2.2 Compliance monitoring + 2.3 Independent review |
| 3 | Incident handling | b) | 3.1 Policy + 3.2 Monitoring/logging + 3.3 Event reporting + 3.4 Assessment/classification + 3.5 Response + 3.6 Post-incident reviews |
| 4 | Business continuity and crisis management | c) | 4.1 BC/DR + 4.2 Backup/redundancy + 4.3 Crisis mgmt |
| 5 | Supply chain security | d) | 5.1 Policy + 5.2 Directory of suppliers |
| 6 | Security in N&IS acquisition, development and maintenance | e) | 6.1 ICT acquisition + 6.2 SDLC + 6.3 Configuration + 6.4 Change/repairs/maintenance + 6.5 Security testing + 6.6 Patch management + 6.7 Network security + 6.8 Network segmentation + 6.9 Malware protection + 6.10 Vulnerability handling/disclosure |
| 7 | Policies and procedures to assess the effectiveness | f) | (singolo punto 7.1) |
| 8 | Basic cyber hygiene practices and security training | g) | 8.1 Awareness + 8.2 Training |
| 9 | Cryptography | h) | (singolo punto 9.1) |
| 10 | Human resources security | i) | 10.1 HR security + 10.2 Background verification + 10.3 Termination/change procedures + 10.4 Disciplinary process |
| 11 | Access control | i, j) | 11.1 Policy + 11.2 Rights + 11.3 Privileged + 11.4 Admin systems + 11.5 Identification + 11.6 Authentication + 11.7 MFA |
| 12 | Asset management | i) | 12.1 Classification + 12.2 Handling + 12.3 Removable media + 12.4 Inventory + 12.5 Deposit/return/deletion |
| 13 | Environmental and physical security | c, e, i) | 13.1 Supporting utilities + 13.2 Physical/environmental threats + 13.3 Perimeter/physical access |

Più **Annex I** (national frameworks, una pagina per Stato membro che ha contribuito) e **Annex II** (glossary).

## Tre elementi standard per ciascun requisito

Per ciascun requisito del Reg. UE 2024/2690, la TIG fornisce:

1. **Guidance** — *"indicative and actionable advice on parameters to consider when implementing a requirement or further explanation of concepts found in the legal text"*. Non vincolante; è la traduzione operativa del requisito normativo.
2. **Examples of evidence** — *"indicative types of evidence showing that a requirement is in place"*. Lista di artefatti documentali e tecnici che possono attestare l'implementazione. **Non esaustivi e non obbligatori in toto** (cfr. disclaimer).
3. **Tips** — *"extra general tips offered for additional consideration"*. Sezione opzionale (alcuni requisiti la omettono).

Tutti e tre sono **soft-law**: il soggetto può scegliere metodi alternativi per soddisfare il requisito o evidenza diversa per dimostrare la compliance.

## Topic-specific policies — 10 elencate

L'introduzione della TIG (pp. 10-11) integra il punto 1.1 dell'Allegato Reg. elencando **10 politiche tematiche** che il regolamento richiede oltre alla policy generale di sicurezza:

1. Risk management policy (cfr. Allegato Reg. 2.1)
2. Incident handling policy (Allegato 3.1.1)
3. Supply chain security policy (Allegato 5.1.1)
4. Security testing policy (Allegato 6.5.1)
5. Policy to assess effectiveness of risk-management measures (Allegato 7.1.1)
6. Cryptography policy (Allegato 9.1)
7. Access control policy (Allegato 11.1.1)
8. Privileged accounts and system administration accounts policy (Allegato 11.3)
9. Handling of information and assets policy (Allegato 12.2.1)
10. Removable media policy (Allegato 12.3.1)

**Approvazione**: la TIG (punto 1.1, GUIDANCE) distingue **nettamente**:

- La **policy on the security of N&IS** (la "master policy" / overarching corporate policy) **deve essere approvata dai management bodies**.
- Le **topic-specific policies** sopra elencate devono essere approvate **"by an appropriate level of management"** — non necessariamente dai management bodies.

Questo confronta direttamente con il regime IT della [[sources/Guida lettura specifiche di base|guida ACN]] (Appendice C, **11 documenti** che richiedono approvazione degli organi di amministrazione/direttivi). Cfr. analisi in [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]] Q2.

## Mapping ai framework standard (cfr. Mapping Table dedicata)

Ciascun requisito è mappato a:

- **ISO/IEC 27001:2022** — clausole e Annex A controls.
- **ISO/IEC 27002:2022** — controlli specifici.
- **NIST Cybersecurity Framework 2.0** — funzioni, categorie, sottocategorie.
- **ETSI EN 319 401 V3.1.1** (2024-06) — General Policy Requirements for Trust Service Providers.
- **CEN/TS 18026:2024** — specifiche tecniche CEN sulla cibersicurezza.
- **National frameworks** — frameworks nazionali NIS2 (Annex I TIG; il framework italiano [[entities/Framework Nazionale per la Cybersecurity|FNCDP 2025]] sarà raccolto in waves future).

> **Caveat ENISA sulla mappatura** (testuale, p. 9-10): *"The mapping should not be interpreted as a measure of equivalency among different standards or frameworks. It simply refers to relevant requirements in these standards or frameworks without assessing whether these fully cover the requirements of the regulation."*

Il mapping completo è nel file Excel ufficiale ENISA — cfr. [[sources/ENISA Mapping Table v1.0 - 2025-06-26]] per dettagli + nota sul formato.

## Esempi di guidance significativa per la wiki

### Risk management framework (cap. 2.1)

TIG conferma scelta libera del framework: *"The entity can use its current risk management framework or adopt a new one"*. Cita esplicitamente **ISO/IEC 27005:2022** come riferimento e rinvia al *Compendium of risk-management frameworks* ENISA per opzioni multiple. Non impone una metodologia specifica — coerente con `ID.RA-05` della det. ACN che lascia libertà metodologica.

### Compensating controls (cap. 2.2)

La TIG (sezione "Examples of evidence" 2.2.1) tratta le eccezioni di policy con riferimento esplicito al *secondo paragrafo dell'art. 2(2) del Reg.* e al *cons. 5* (microsoggetti). Esempi indicativi:

- Aggiornamenti software incompatibili → eccezione fino a soluzione compatibile;
- MFA non supportata da un sistema legacy → eccezione con misure alternative;
- Sistemi legacy senza supporto crittografia → eccezione fino a sostituzione.

Tutti gli esempi richiedono "*Records of the exception request and approval, along with details of the compensatory controls implemented*". Cfr. confronto con regime IT in [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]] Q4.

### Asset classification + risk-based scoping (cap. 12.1)

Approccio TIG: classificazione asset per sensibilità/criticità → applicazione di misure proporzionate. Confronto con clausola IT "per almeno i sistemi informativi e di rete rilevanti" ([[concepts/Sistemi informativi e di rete rilevanti]]) in Q3 della synthesis dedicata.

## Living document — processo di revisione

La TIG è esplicitamente un **living document** (p. 3): standard e framework nazionali sono soggetti a cambiamento, quindi ENISA + Commissione + NIS Cooperation Group la riesamineranno periodicamente. Possibili versioni future v1.x con aggiornamenti di mapping; v2.0 in caso di revisione del Reg. UE 2024/2690.

## Entità menzionate

- [[entities/ENISA]] — autore
- Commissione europea — collaboratore
- [[entities/Gruppo di Cooperazione NIS]] — collaboratore (NIS CG work stream on security measures)
- ECATS — ENISA expert group for European Competent Authorities for Trust Services
- ECASEC — ENISA expert group for European Competent Authorities for Secure Electronic Communications
- ISO/IEC, NIST, ETSI, CEN — fonti degli standard mappati
- ISACA — citata per glossario residual risk

## Concetti collegati

- [[concepts/Misure di gestione del rischio cyber]] — art. 21 NIS2, di cui la TIG fornisce guidance UE
- [[concepts/Misure di sicurezza di base]] — pendant IT (det. ACN); la TIG e la guida ACN sono livelli interpretativi paralleli (UE/IT) della stessa materia art. 21 NIS2
- [[concepts/Notifica di incidente significativo]] — cap. 3 TIG dettaglia incident handling
- [[concepts/Sistemi informativi e di rete rilevanti]] — confrontare con asset-based scoping TIG (Q3)
- [[concepts/Clausole basate sul rischio]] — confrontare con clausole `se opportuno/se applicabile/nella misura del possibile` del Reg. UE + guida TIG
- [[concepts/Evidenze documentali NIS]] — la TIG fornisce "examples of evidence" per ciascun requisito, livello UE
- [[concepts/Responsabilità degli organi di gestione]] — confrontare con il regime UE (master policy al board, topic-specific a "appropriate level of management") (Q2)
- [[concepts/Approccio multi-rischio]] — cap. 2.1.2 lett. d) Reg. richiama "all-hazards approach", confermato dalla TIG

## Synthesis collegate

- [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]] — **deliverable critico** che usa la TIG per ridurre le 4 open question normative della synthesis di coordinamento
- [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]] — synthesis di coordinamento di cui sopra
- [[synthesis/Stratificazione delle norme cybersecurity in Italia]]

## Note dell'agente

- *Sintesi dell'agente:* la TIG è il **principale strumento operativo di soft-law** del Reg. UE 2024/2690. Per un fornitore cloud italiano, l'uso pratico è triplice: (a) guidance interpretativa per implementare il Reg., (b) examples of evidence per costruire il proprio piano di evidenze documentali, (c) mapping per riconciliare il Reg. con framework ISO/NIST che il soggetto potrebbe già usare.
- *Sintesi dell'agente:* il **valore unico** della TIG rispetto alla guida ACN italiana è che la TIG copre **tutti gli 11 tipi di DSP** (oltre al cloud), mentre la guida ACN copre i soggetti NIS italiani in modo orizzontale. Per la wiki, la TIG è la **fonte di riferimento per i DSP** quando il soggetto è dentro l'ambito Reg. UE.
- *Sintesi dell'agente:* il **disclaimer** della TIG è giuridicamente forte. Riconosce esplicitamente che il regime nazionale resta e che i framework nazionali sono mezzi di compliance equivalenti. Questo **conferma la tesi 3a** della synthesis di coordinamento (applicazione cumulativa).
- Lacuna nota: il **Compendium of Risk-Management Frameworks ENISA** (citato come riferimento per la scelta di metodologia di risk management) non è in wiki. Da considerare in waves future.
- Lacuna nota: **ETSI EN 319 401 V3.1.1** (citato come fonte di mapping per trust service providers) e **CEN/TS 18026:2024** non in wiki. Out-of-scope MVP tool ma rilevante per GRC per chi lavora con trust services.
- Lacuna nota: il **NIST CSF 2.0** è citato come standard di mapping ma non è ancora ingerito — è pendente come prossima sessione di Wave 6.
