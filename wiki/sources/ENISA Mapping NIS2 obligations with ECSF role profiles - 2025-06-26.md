---
title: ENISA — Mapping NIS2 obligations with ECSF role profiles
type: source
source_type: article
source_path: raw/articles/Mapping NIS 2 obligations with ECSF role profiles.pdf
url: https://www.enisa.europa.eu/publications/cybersecurity-roles-and-skills-for-nis2-essential-and-important-entities
author: Konstantinos Adamos (University of the Aegean) · Fabio Di Franco (ENISA) · Sozon Leventopoulos (Athens University of Economics and Business)
date_published: 2025-06
date_ingested: 2026-05-19
tags: [enisa, ecsf, nis2, mapping, roles, skills, art-21, art-23, cybersecurity-workforce]
scope: grc_personal
aliases: [Mapping NIS2-ECSF, ENISA NIS2 ECSF mapping, Cybersecurity Roles and Skills for NIS2]
---

## TL;DR

Documento ENISA di giugno 2025 (ISBN 978-92-9204-706-1, DOI 10.2824/8870995, **CC-BY 4.0**, ~32 pp), parte del pacchetto pubblicato il 26/06/2025 insieme alla TIG v1.0 e alla Mapping Table v1.0. Mappa gli **obblighi NIS2 art. 21** (misure di gestione del rischio) **e art. 23** (notifica incidenti) sui **12 profili ECSF** del [[sources/ECSF Role Profiles - 2022-09|framework ECSF]]. Titolo completo: *"Cybersecurity Roles and Skills for NIS2 Essential and Important Entities — Mapping NIS2 obligations to ECSF"*.

Risponde alle domande tipiche di un'organizzazione che deve adempire NIS2: *"Quali ruoli e skill servono per soddisfare gli obblighi? Quale approccio step-by-step può guidarmi nell'organizzazione del workforce, della pianificazione strategica?"* Indirizza sia organizzazioni private sia autorità competenti degli Stati membri che devono tradurre obblighi normativi in policy di capacity building.

Per la wiki, è lo **strumento di workforce planning** allineato a NIS2 a livello UE. Per una transizione da software engineering a GRC, è la fonte autoritativa per **giustificare** la scelta di un profilo professionale specifico: *"ENISA dice che per soddisfare gli obblighi art. 21/23 NIS2 servono ruoli X, Y, Z — io punto al ruolo Z"*.

## Struttura del documento

| Capitolo | Contenuto |
|---|---|
| **1. Introduction** | Purpose, target audience, document structure |
| **2. NIS2 Obligations** | 2.1 Art. 21 (risk-management measures, 10 ambiti) · 2.2 Art. 23 (reporting obligations: pre-notifica 24h, notifica 72h, final report 1 mese) |
| **3. Use cases** | 2 scenari operativi: (3.1) implementazione misure ex art. 21 · (3.2) post-incident response e reporting ex art. 23. Include "Organisational Tasks", "Strategical organisational alignment and Resource allocation", "The Team", "Summary" |
| **4. Detailed mapping of ECSF and NIS2** | Tabella di mapping puntuale obblighi NIS2 ↔ profili ECSF · 4.1 Mapping benefits |
| **Annex I** | Metodologia |

## Use case 1 — Implementazione misure ex art. 21 NIS2

Il documento identifica i ruoli ECSF necessari per implementare le 10 categorie di misure dell'art. 21. Profili coinvolti (preponderanza variabile per misura):

- **CISO** — lead strategico
- **Cybersecurity Risk Manager** — risk assessment + treatment plan
- **Cyber Legal, Policy & Compliance Officer** — interpretazione obblighi, rapporti autorità, documentazione
- **Cybersecurity Architect** — design security-by-design dei sistemi
- **Cybersecurity Implementer** — implementazione tecnica
- **Cybersecurity Educator** — awareness/training ex lett. g) art. 21
- **Cybersecurity Auditor** — verifica efficacia ex lett. f) art. 21
- **Cyber Threat Intelligence Specialist** — input al risk management

## Use case 2 — Post-incident response e reporting ex art. 23 NIS2

Profili coinvolti per la gestione di un incidente significativo:

- **Cyber Incident Responder** — lead operativo del contenimento e analisi
- **Digital Forensics Investigator** — raccolta evidenze
- **Cyber Threat Intelligence Specialist** — contesto threat
- **CISO** — escalation al management body + autorizzazioni
- **Cyber Legal, Policy & Compliance Officer** — interfaccia con CSIRT Italia + ACN + Garante per data breach
- **Cybersecurity Educator** — post-incident review e formazione

**Tempistiche art. 23** richiamate dal documento: 24h pre-notifica, 72h notifica, 1 mese final report. Cfr. [[concepts/Notifica di incidente significativo]].

## Detailed mapping ECSF ↔ NIS2 (cap. 4)

Per ciascuno dei 10 ambiti dell'art. 21 NIS2 + 4 fasi del reporting art. 23, il documento elenca i profili ECSF primari e di supporto. Il valore aggiunto è la **matrice esplicita**:

| Obbligo NIS2 | Profili ECSF primari | Profili di supporto |
|---|---|---|
| Art. 21 lett. a) Risk analysis + N&IS security policy | Risk Manager, CISO, Compliance Officer | Auditor |
| Art. 21 lett. b) Incident handling | Incident Responder, CISO | Forensics, CTI Specialist, Compliance Officer |
| Art. 21 lett. c) Business continuity, backup | CISO, Risk Manager, Architect | Implementer |
| Art. 21 lett. d) Supply chain security | Compliance Officer, Risk Manager, Architect | Auditor |
| Art. 21 lett. e) Security in acquisition/development | Architect, Implementer | Risk Manager |
| Art. 21 lett. f) Policies to assess effectiveness | Auditor, CISO | Risk Manager |
| Art. 21 lett. g) Basic cyber hygiene + training | Educator, CISO | Compliance Officer |
| Art. 21 lett. h) Cryptography | Architect, Implementer | Auditor |
| Art. 21 lett. i) HR security, access control, asset management | CISO, Implementer, Architect | Compliance Officer |
| Art. 21 lett. j) MFA, secure comms | Architect, Implementer | Auditor |
| Art. 23 - Notifica incidenti | Incident Responder, CISO, Compliance Officer | Forensics, CTI |

(Esempio sintetico; il documento contiene matrici più granulari per skills/tasks specifici.)

## Mapping benefits (§ 4.1)

Il documento argomenta esplicitamente perché il mapping è utile:

1. **Per organizzazioni**: workforce planning più efficace, gap analysis su skill, definizione di job descriptions tarate su NIS2.
2. **Per autorità competenti (ACN, ENISA, NIS Cooperation Group)**: capacity building programs, identificare gap di skill a livello nazionale.
3. **Per il sistema educativo (università, formatori, certificatori)**: progettare curricula coerenti con le esigenze di workforce derivate da NIS2.
4. **Per il consulente individuale**: tradurre la propria preparazione in profili ECSF spendibili nel mercato.

## Mapping con il regime NIS2 italiano

Il documento è UE-level. Per il contesto italiano:

- **Art. 21 NIS2 → Det. ACN 379907/2025 / [[concepts/Misure di sicurezza di base]]**: le misure di sicurezza di base codificate dalla det. ACN sono il declinato nazionale degli obblighi art. 21. Il mapping ECSF si applica direttamente.
- **Art. 23 NIS2 → Art. 25 D.Lgs. 138/2024 + Allegati 3-4 det. ACN ([[concepts/Incidenti significativi di base]])**: la notifica al [[entities/CSIRT Italia]] è il declinato nazionale degli obblighi art. 23.
- **Ruoli operativi italiani** ([[entities/Punto di contatto NIS]] + [[entities/Referente CSIRT]] + Rappresentante NIS in Italia): non sono mappati 1-a-1 sui profili ECSF (sono ruoli **amministrativi** di interfaccia con ACN, non profili tecnici di workforce). Tuttavia il punto di contatto NIS è generalmente coperto dal **Cyber Legal/Policy/Compliance Officer**; il referente CSIRT dal **Cyber Incident Responder** o **CISO**.

## Citazione (entro vincolo <15 parole)

> *"Which roles and skills are needed to meet these requirements?"* (ENISA NIS2-ECSF p. 6 — 9 parole)

## Punti chiave per la transizione GRC italiana

1. **Documento autorevole di posizionamento**: per giustificare a un recruiter / cliente "perché il tuo profilo ECSF X è quello che mi serve per NIS2", questo documento è la **fonte UE-binding** da citare. Asset di carriera diretto.

2. **Mapping bidirezionale**: il documento può essere letto sia "obbligo → ruolo" (workforce planning) sia "ruolo → obblighi che soddisfa" (positioning). L'autore può estrarre il subset di obblighi NIS2 coperti dal profilo Cyber Legal/Policy/Compliance Officer e usarlo come *value proposition*.

3. **Coerenza con TIG / Mapping Table**: il documento è parte del **pacchetto integrato ENISA del 26/06/2025**, insieme a TIG v1.0 + Mapping Table v1.0. Padroneggiare il pacchetto completo = padroneggiare lo stato dell'arte UE-level su NIS2.

4. **Use cases operativi**: i 2 use case (implementazione misure + post-incident response) sono **storie applicate** da usare per esempi concreti in contesti di colloquio o di vendita servizi. Più potenti di descrizioni astratte di ruolo.

5. **Caveat**: il documento è **soft-law** (come la TIG). Non vincolante. Le organizzazioni italiane sono libere di organizzare il proprio workforce diversamente — ma se lo fanno, devono comunque dimostrare che ciascun obbligo NIS2 è coperto da qualcuno con le skill appropriate.

## Entità menzionate

- [[entities/ENISA]] — pubblicatore
- Konstantinos Adamos (University of the Aegean) — autore lead
- Fabio Di Franco (ENISA) — co-autore (anche lead dell'ECSF 2022)
- Sozon Leventopoulos (Athens University of Economics and Business) — co-autore

## Concetti collegati

- [[concepts/Misure di gestione del rischio cyber]] — art. 21 NIS2 di cui il mapping copre i 10 ambiti
- [[concepts/Notifica di incidente significativo]] — art. 23 NIS2 di cui il mapping copre le 4 fasi
- [[concepts/Responsabilità degli organi di gestione]] — il CISO è il referente operativo del management body
- [[concepts/Evidenze documentali NIS]] — i deliverable ECSF (Strategy, Policy, Risk Assessment) coincidono con la documentazione richiesta

## Synthesis collegate

- [[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]] — synthesis dedicata (creata in questa sessione)
- [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] — complementare: il cross-walk dice *cosa* fare, l'ECSF dice *chi* lo fa

## Note dell'agente

- *Sintesi dell'agente:* questo documento è il **trait d'union** tra la dimensione tecnica (misure NIS2 / NIST CSF / FNCDP / ISO 27002) e la dimensione workforce/skill. Per il consulente GRC che vende un servizio, presentare in un'unica offerta "mapping tecnico + workforce plan" è una proposta di valore completa.
- *Sintesi dell'agente:* il documento **non risponde** alla domanda "quale sia il *miglior* profilo per NIS2": tutti i 12 profili sono necessari in un'organizzazione matura. Ma per il **consulente esterno** che si vende come "lead per la compliance NIS2 di una PMI", i profili più *spendibili* in singolo sono Cyber Legal/Policy/Compliance Officer + Risk Manager + Auditor (in combinazione).
- **Lacuna nota**: il documento è UE-generico. Non descrive le specificità italiane (ruoli amministrativi del decreto NIS, interazione con Garante per data breach, ecc.). La synthesis [[synthesis/Profili ECSF per il consulente GRC NIS2 italiano]] colma parzialmente questo gap per l'autore.
