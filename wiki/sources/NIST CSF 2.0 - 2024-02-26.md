---
title: NIST Cybersecurity Framework (CSF) 2.0
type: source
source_type: paper
source_path: raw/articles/NIST.CSWP.29.pdf
url: https://doi.org/10.6028/NIST.CSWP.29
author: National Institute of Standards and Technology (NIST)
date_published: 2024-02-26
date_ingested: 2026-05-19
tags: [nist, csf, csf-2.0, framework, govern, identify, protect, detect, respond, recover, cybersecurity, dominio-pubblico]
scope: grc_personal
aliases: [NIST CSF 2.0, NIST CSWP 29, Cybersecurity Framework 2.0]
---

## TL;DR

Documento NIST CSWP 29 del 26 febbraio 2024 (40 pp), versione 2.0 del **Cybersecurity Framework** originariamente pubblicato nel 2014. Documento ufficiale **gratuito** e di **pubblico dominio** (NIST.gov). Introduce la sesta funzione **GOVERN** (rispetto al CSF 1.1 che ne aveva 5) e ridefinisce il framework come applicabile a qualunque organizzazione, sezione, settore, livello di maturità — non solo "critical infrastructure" come la dicitura originale.

Cardine architetturale per la wiki: il **[[entities/Framework Nazionale per la Cybersecurity|FNCDP italiano edizione 2025]]** è esplicitamente derivato dal NIST CSF 2.0 ([[sources/Allegato 1 - Misure di sicurezza di base per i soggetti importanti|Allegato 1 det. ACN]] e la [[sources/Guida lettura specifiche di base|guida ACN]] dichiarano l'uso delle 6 funzioni FNCDP/NIST CSF v2.0). Le **misure di sicurezza di base** della det. ACN 379907/2025 sono codificate con prefissi NIST (`GV.PO-01`, `ID.RA-05`, `PR.AA-03`, ecc.) — questa pagina fornisce la fonte upstream per quei codici.

> *Citazione NIST CSF 2.0 (< 15 parole):* *"The CSF is a foundational resource that may be adopted voluntarily and through governmental policies and mandates."* (Trad. agente: *"Il CSF è una risorsa fondazionale, adottabile su base volontaria o tramite politiche e mandati governativi."*)

## Componenti del framework

Il CSF 2.0 è composto da **tre componenti** integrati:

| Componente | Cosa è | Uso |
|---|---|---|
| **CSF Core** | Tassonomia gerarchica di **outcomes** di cibersicurezza in 3 livelli: Functions → Categories → Subcategories | Il "vocabolario" comune del framework — *cosa* deve essere ottenuto |
| **CSF Organizational Profiles** | Descrizione della **postura attuale** e/o **postura target** di un'organizzazione, in termini di outcomes del Core | Lo strumento di **gap analysis** — *dove sono / dove voglio essere* |
| **CSF Tiers** | 4 livelli (Partial / Risk Informed / Repeatable / Adaptive) che caratterizzano il **rigore** delle pratiche di governance e gestione del rischio | Caratterizzazione qualitativa della maturità — *come gestisco il rischio* |

Tre risorse online complementari (NIST CSF website, non incluse nel CSWP 29 stesso): **Informative References**, **Implementation Examples**, **Quick-Start Guides**.

## Le 6 funzioni del CSF Core

Codice di 2 lettere uguale al prefisso delle sottocategorie del FNCDP italiano (cfr. [[concepts/Misure di sicurezza di base]]):

### GOVERN (GV) — *novità del CSF 2.0*

La cibersicurezza è inquadrata nella **enterprise risk management (ERM)** dell'organizzazione. Categorie principali: organizational context, cybersecurity strategy, supply chain risk management, roles/responsibilities/authorities, policy, oversight. La funzione GOVERN è **al centro della ruota** (Fig. 2 CSF 2.0): informa come si implementano le altre 5 funzioni.

*Rilevanza per NIS2*: la GOVERN function è il pendant concettuale dell'**art. 20 NIS2 / art. 23 D.Lgs. 138/2024** (responsabilità degli organi di amministrazione e direttivi). Cfr. [[concepts/Responsabilità degli organi di gestione]].

### IDENTIFY (ID)

Comprensione degli **asset** (dati, hardware, software, sistemi, facility, servizi, persone), dei **fornitori**, e dei **rischi cyber correlati**. Include l'identificazione delle opportunità di miglioramento (Improvement category).

### PROTECT (PR)

**Safeguard** per gestire i rischi: identity management, authentication, access control; awareness/training; data security; platform security; resilience of technology infrastructure.

### DETECT (DE)

**Scoperta tempestiva** di anomalie, indicators of compromise (IoC), eventi avversi. Abilita la successiva risposta e ripristino.

### RESPOND (RS)

Azioni di **contenimento** in caso di incidente rilevato: incident management, analysis, mitigation, reporting, communication.

### RECOVER (RC)

**Ripristino** di asset e operations al normal operating level + comunicazione durante recovery.

### Diagramma logico

Le 6 funzioni sono **concorrenti** (non sequenziali). GOVERN/IDENTIFY/PROTECT/DETECT operano in modo continuo; RESPOND/RECOVER si attivano in caso di incident.

```
                      GOVERN (al centro)
                            │
        ┌───────────────────┼───────────────────┐
        │                                       │
   IDENTIFY ──── PROTECT ──── DETECT ──── RESPOND ──── RECOVER
```

## CSF Organizational Profiles — il workflow di gap analysis

Processo a 5 step (Fig. 3 CSF 2.0):

1. **Scope the Organizational Profile** — definire il perimetro (l'intera org, una BU, un sistema specifico, una specifica minaccia come ransomware).
2. **Gather information** — policy, risk priorities, BIA registers, requirements, practices, work roles.
3. **Create the Profile** — Current Profile + Target Profile, con info per ciascun outcome del Core.
4. **Analyze gaps** — gap analysis Current ↔ Target → action plan prioritizzato.
5. **Implement** — eseguire il plan; aggiornare il Profile periodicamente.

**Community Profiles**: profili condivisi tra organizzazioni con interessi comuni (settore, tipo di minaccia). NIST li pubblica sul proprio sito; un'organizzazione può adottare un Community Profile come baseline per il proprio Target Profile.

## CSF Tiers — 4 livelli di maturità

| Tier | Nome | Caratteristiche sintetiche |
|---|---|---|
| 1 | **Partial** | Risk management ad-hoc, awareness limitata, supply chain non integrata |
| 2 | **Risk Informed** | Risk management approvato dal management, awareness diffusa, supply chain considerata |
| 3 | **Repeatable** | Processi formalizzati e ripetibili, awareness organizationale-wide, supply chain inclusa in modo strutturato |
| 4 | **Adaptive** | Risk management continuamente adattato, awareness culturale, supply chain proattivamente gestita |

I Tier non sono livelli di maturità prescritti (un'organizzazione non deve necessariamente puntare al Tier 4); sono una **scelta strategica** in base al rischio, alle risorse, al contesto.

## Confronto con FNCDP italiano (placeholder — completare in Sessione 3 post-ingest FNCDP)

> **Sezione da completare in Wave 6 Sessione 3** dopo l'ingest del documento `FNCDP_-_Edizione_2025_v2.1_-_Core.pdf`. Punti attesi:
> - Le 6 funzioni FNCDP 2025 coincidono con il NIST CSF 2.0 (stessi prefissi `GV/ID/PR/DE/RS/RC`).
> - Il FNCDP **aggiunge** una dimensione di *data protection* (GDPR + ePrivacy) non presente nel NIST CSF.
> - Il FNCDP è **adattato al contesto italiano** in terminologia (es. "organizzazione" → "soggetto NIS").
> - Una tabella di mapping puntuale categorie/sottocategorie FNCDP ↔ NIST CSF 2.0 sarà costruita post-ingest FNCDP.

## Mapping con il regime NIS2

| Regime | Relazione con NIST CSF 2.0 |
|---|---|
| **[[sources/Direttiva (UE) 2022-2555 (NIS2)\|Direttiva NIS2]]** | Il NIST CSF non è citato esplicitamente, ma la struttura "outcomes-based" è coerente con l'approccio dell'art. 21 NIS2 (10 ambiti minimi di misure) |
| **[[sources/Regolamento di esecuzione UE 2024-2690\|Reg. UE 2024/2690]]** | I 13 punti dell'Allegato del Reg. mappano sulle Funzioni/Categorie/Subcategorie NIST CSF — cfr. [[sources/ENISA Mapping Table v1.0 - 2025-06-26]] |
| **[[sources/ENISA Technical Implementation Guidance v1.0 - 2025-06-26\|ENISA TIG v1.0]]** | Cita esplicitamente il NIST CSF 2.0 come standard di riferimento; ogni requisito del Reg. UE è mappato a sottocategorie NIST CSF (es. punto 1.1 → `PR.AT-02, GV.PO-01, GV.PO-02, GV.OC-03, GV.RM-03`) |
| **[[entities/Framework Nazionale per la Cybersecurity\|FNCDP edizione 2025]]** | Derivato direttamente dal NIST CSF 2.0 — stesse 6 funzioni, stessi prefissi codice |
| **[[sources/Determinazione ACN specifiche di base - 379907-2025-12-19\|Det. ACN 379907/2025]] (Allegati 1-2)** | Le misure di sicurezza di base IT usano codici NIST CSF 2.0 puri (`GV.PO-01`, `PR.AA-03`, `ID.RA-05`, ecc.) |

## Cross-walk con altri standard (Informative References)

Il NIST CSF 2.0 non è uno standard isolato — è **architetturalmente integrato** con altri framework via Informative References pubblicate online:

- **NIST SP 800-53** (Security and Privacy Controls for Federal Information Systems) — il catalogo di controlli di riferimento USA, mappato sulle sottocategorie CSF
- **NIST SP 800-61** ([[entities/NIST SP 800-61|Incident Handling Guide]]) — il modello a 5 fasi adottato anche dalle [[sources/Linee Guida NIS - Gestione incidenti - 2025-12|Linee Guida ACN gestione incidenti]]
- **NIST SP 800-37** (Risk Management Framework)
- **ISO/IEC 27001:2022** + **ISO/IEC 27002:2022** — mapping comune NIS2 ↔ NIST ↔ ISO via [[sources/ENISA Mapping Table v1.0 - 2025-06-26]]
- **COBIT 2019**, **CIS Controls v8**, **PCI DSS 4.0**, **HIPAA Security Rule** — tutti mappati da NIST come Informative References

## Cosa è cambiato dal CSF 1.1 al CSF 2.0

Cambiamenti macroscopici dichiarati nel "Note to Readers" del documento:

1. **Nuova funzione GOVERN** (la 6.a) — la più visibile.
2. **Rimozione del termine "Critical Infrastructure"** dal titolo — il framework è ora esplicitamente universale (era *"Framework for Improving Critical Infrastructure Cybersecurity"*).
3. **Riorganizzazione completa delle Categories** — alcune cat. del 1.1 sono state spostate o assorbite (es. la cat. "Risk Assessment" del 1.1 sotto IDENTIFY è stata in parte spostata sotto GOVERN come "Risk Management Strategy").
4. **Introduzione dei Community Profiles** — risorse condivise per settori/use case.
5. **Online Resources Suite** — NIST sposta una parte sostanziale del contenuto operativo dalle Implementation Examples ai Quick-Start Guides online (web-first).

## Punti chiave per la transizione GRC italiana

1. **Asset di carriera**: il NIST CSF 2.0 è il framework cyber **più citato globalmente**. Conoscenza approfondita = differenziatore in qualsiasi ruolo GRC (auditor, consultant, security officer). La sua coincidenza architetturale con il FNCDP italiano rende particolarmente vantaggioso padroneggiarlo per chi lavora nel mercato italiano.

2. **Linguaggio comune con NIS2**: i codici sottocategoria (`GV.PO-01`, `PR.AA-03`, ecc.) usati dalla det. ACN 379907/2025 sono il vocabolario NIST CSF. Tradurre tra norma e framework è un'attività ricorrente del consulente GRC; partire dalla fonte upstream (questo documento) è efficiente.

3. **Outcome-based vs control-based**: il CSF si distingue da standard come ISO 27001 perché parla di *outcomes* (cosa deve essere ottenuto) anziché di *controls* (cosa deve essere fatto). Per ISO 27001 LA prep, è utile esercitarsi a tradurre: outcome CSF → control ISO 27002.

4. **GOVERN come ponte verso il board**: la nuova funzione GOVERN è la più "executive-friendly" del framework. Per costruire reporting agli organi di amministrazione (richiesto da art. 23 D.Lgs. 138/2024), il linguaggio GOVERN è più immediato della clausola normativa.

5. **Tiers come strumento di stage diagnosi**: non confondere Tier (rigore della governance) con maturità tecnica. Un'organizzazione può essere Tier 3 con misure tecniche modeste, e Tier 1 con tooling sofisticato ma processi ad-hoc.

## Entità menzionate

- [[entities/NIST SP 800-61|NIST Special Publications]] — famiglia complementare al CSF (esiste già il nodo per SP 800-61 per IR)
- ISO/IEC — fonte degli standard 27001/27002 mappati come Informative References

## Concetti collegati

- [[concepts/Misure di sicurezza di base]] — utilizzano la struttura NIST CSF v2.0 (6 funzioni, codici puntuali)
- [[concepts/Misure di gestione del rischio cyber]] — art. 21 NIS2 mappato a NIST CSF via ENISA TIG
- [[concepts/Responsabilità degli organi di gestione]] — pendant della funzione GOVERN
- [[concepts/Processo gestione incidenti NIS]] — collegato alle funzioni RESPOND/RECOVER
- [[concepts/Approccio multi-rischio]] — coerente con la scopo del CSF di applicarsi a tutti i tipi di rischio

## Synthesis collegate

- [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] — synthesis dedicata al cross-walk (creata in questa sessione)
- [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]] — la TIG cita esplicitamente il NIST CSF come standard di mapping

## Note dell'agente

- *Sintesi dell'agente:* il NIST CSF 2.0 è **il singolo documento più ad alta leva** per la transizione GRC italiana nel contesto NIS2: pubblico, gratuito, breve (40 pp), e architetturalmente coincidente con il FNCDP italiano. La sua padronanza vale come *quick win* nei primi mesi di carriera GRC.
- *Sintesi dell'agente:* la novità della funzione **GOVERN** è strategicamente significativa per NIS2: arriva nello stesso periodo in cui l'art. 20 NIS2 introduce la responsabilità del board. I due cambiamenti convergono: il framework tecnico-operativo e la norma giuridica spingono entrambi sul "*chi governa il rischio cyber, lo gestisce*". Questo allineamento accidentale è un punto narrativo utile per articoli LinkedIn / contributi pubblici sulla materia.
- Lacuna nota: il **Profile Templates** ENISA pubblicato online (separato da questo CSWP 29) include esempi di Organizational Profile pre-compilati. Non in wiki; outlook futuro.
- Lacuna nota: il **mapping completo CSF 2.0 → Informative References** (NIST SP 800-53, ISO 27002, ecc.) è pubblicato online da NIST come matrice separata. Non ingerito in wiki — out-of-scope di questa sessione. La [[sources/ENISA Mapping Table v1.0 - 2025-06-26|ENISA Mapping Table]] fornisce un mapping parziale via NIS2.
