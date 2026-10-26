---
title: Processo gestione incidenti NIS
type: concept
scope: grc_personal
tags: [nis2, italia, gestione-incidenti, nist, linee-guida]
sources: ["[[sources/Linee Guida NIS - Gestione incidenti - 2025-12]]", "[[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]]", "[[sources/D.Lgs. 138-2024 (Decreto NIS)]]"]
aliases: [Processo IR NIS, Modello 5 fasi NIST, Incident response NIS]
---

## Definizione

Processo organizzativo per la gestione degli incidenti di sicurezza informatica adottato dai **soggetti NIS essenziali e importanti** in conformità all'**art. 24** del [[sources/D.Lgs. 138-2024 (Decreto NIS)]] (gestione incidenti come uno dei 10 ambiti minimi delle misure di sicurezza) e all'**art. 25** (notifica al CSIRT).

Il modello di riferimento è quello delle **[[sources/Linee Guida NIS - Gestione incidenti - 2025-12]]**, derivato dal **[[entities/NIST SP 800-61|NIST SP 800-61r3]]**.

## Le 5 fasi

| Fase | Obiettivo | Sotto-fasi |
|---|---|---|
| **1. Preparazione** | Costituire la base per una risposta efficace | Governo (politiche, ruoli/responsabilità); identificazione (inventario sistemi, minacce/vulnerabilità); protezione (misure tecnologiche e organizzative) |
| **2. Rilevamento** | Rilevare tempestivamente l'incidente | — |
| **3. Risposta** | Reagire all'incidente rilevato | Segnalazione; investigazione; contenimento; eradicazione |
| **4. Ripristino** | Riportare i sistemi compromessi allo stato pre-incidente | — |
| **5. Miglioramento** | Lezioni apprese, miglioramenti del processo | Trasversale a tutte le fasi |

## Piano per la gestione degli incidenti

Il processo è generalmente formalizzato in un documento — il **piano per la gestione degli incidenti** — che descrive politiche, ruoli, procedure e flussi operativi.

## Mappatura con le specifiche di base

L'**Appendice B** delle Linee Guida NIS elenca, per ogni fase e sotto-fase, le **misure di sicurezza di base** (cfr. [[concepts/Misure di sicurezza di base]]) della [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]] pertinenti — è il **ponte concreto** tra la specifica regolamentare e il processo operativo.

## Ruoli operativi

- **[[entities/Punto di contatto NIS|Punto di contatto]]**: owner amministrativo (governance e responsabilità).
- **[[entities/Referente CSIRT|Referente CSIRT]] e sostituti**: owner operativo della **fase Risposta — sotto-fase Segnalazione** verso [[entities/CSIRT Italia]]; gestiscono le notifiche scaglionate ex artt. 25 e 26 decreto NIS.
- **Organi di amministrazione e direttivi**: approvano le politiche di gestione incidenti come parte delle [[concepts/Misure di sicurezza di base]].

## Collegamenti

- [[concepts/Notifica di incidente significativo]] — l'output regolatorio della fase Segnalazione
- [[concepts/Incidente significativo]]
- [[concepts/Incidenti significativi di base]] — le soglie operative
- [[concepts/Misure di gestione del rischio cyber]] — la base normativa
- [[entities/NIST SP 800-61]]
- [[entities/CSIRT Italia]]

## Note dell'agente

- *Sintesi dell'agente:* la sotto-fase **Segnalazione** della Risposta è il **punto di intersezione** tra processo interno del soggetto e obblighi normativi: è qui che scatta il timer 24h/72h/1mese delle notifiche al [[entities/CSIRT Italia]].
- La fase **Miglioramento** trasversale è la novità di SP 800-61r3 rispetto a r2, dove il post-incident era solo l'ultima fase: significa che il soggetto deve raccogliere lezioni apprese **continuamente, anche durante l'incidente**, non solo dopo.
