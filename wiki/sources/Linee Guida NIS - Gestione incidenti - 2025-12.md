---
title: Linee Guida NIS — Gestione incidenti — 2025-12
type: source
scope: grc_personal
source_type: article
source_path: raw/articles/definizione-del-processo-di-gestione-degli-incidenti-di-sicurezza-informatica.pdf
url: https://www.acn.gov.it/portale/nis/normativa
author: Agenzia per la Cybersicurezza Nazionale
date_published: 2025-12
date_ingested: 2026-04-29
tags: [NIS2, ACN, gestione incidenti, NIST, specifiche di base, linee guida]
---

## TL;DR

Linee Guida NIS dell'[[entities/ACN]] (v1.0 dic 2025, v1.1 apr 2026) che definiscono il **processo di gestione degli incidenti di sicurezza informatica** per i soggetti NIS essenziali e importanti, in attuazione degli articoli 24 e 25 del [[sources/D.Lgs. 138-2024 (Decreto NIS)]]. Il modello è derivato dal **NIST SP 800-61r3** e articolato in cinque fasi (preparazione, rilevamento, risposta, ripristino, miglioramento). Le appendici A e B mappano le specifiche di base della [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]] sulle fasi del processo.

## Punti chiave

- **Versioni**: v1.0 dic 2025 (prima pubblicazione); v1.1 apr 2026 (aggiunge i riferimenti alla Determinazione 127434/2026 sui termini per i soggetti 2026 e l'aggiornamento della Determinazione piattaforma e procedure).
- **Destinatari**: soggetti NIS **essenziali e importanti** (definiti in art. 6 decreto NIS).
- **Norme di riferimento**: [[sources/D.Lgs. 138-2024 (Decreto NIS)]]; Determinazione obblighi di base (n. 379907 del 19/12/2025); Determinazione soggetti 2026; Determinazione piattaforma e procedure.
- **Documenti di riferimento**: [[entities/NIST SP 800-61]] (r2 e r3, Computer Security Incident Handling Guide / Incident Response Recommendations).
- **Modello a 5 fasi** (derivato da NIST SP 800-61r3):
  1. **Preparazione** — precede l'incidente; sotto-fasi: governo (politiche, ruoli/responsabilità), identificazione (inventario sistemi, minacce/vulnerabilità), protezione (misure tecnologiche e organizzative).
  2. **Rilevamento** — rilevazione tempestiva del verificarsi di un incidente.
  3. **Risposta** — sotto-fasi: segnalazione, investigazione, contenimento, eradicazione.
  4. **Ripristino** — riportare i sistemi compromessi allo stato pre-incidente.
  5. **Miglioramento** — lezioni apprese; **trasversale a tutte le fasi**.
- **Piano per la gestione degli incidenti**: documento organizzativo che descrive il processo (citato in §2 del documento).
- **Mappatura misure di sicurezza di base**: l'Appendice B elenca, per ciascuna fase/sotto-fase, le misure pertinenti tratte dalle specifiche di base — è il **ponte concreto** tra l'obbligo astratto (art. 24) e l'implementazione operativa.
- **Definizioni chiave**: "punto di contatto" (persona designata dal soggetto NIS ex art. 7 c. 1 lett. c)) e "referente CSIRT" (designato dal punto di contatto per interloquire con [[entities/CSIRT Italia]] ed effettuare le notifiche ex artt. 25 e 26 decreto NIS).

## Citazioni rilevanti

> "La gestione degli incidenti è ricompresa tra le misure in materia di gestione dei rischi che i soggetti NIS essenziali e importanti devono adottare secondo quanto previsto dall'articolo 24 del decreto. Inoltre, ai sensi dell'articolo 25 […], i soggetti NIS devono notificare al CSIRT Italia ogni incidente che ha un impatto significativo sulla fornitura dei loro servizi." — §1.1 Premessa.

> "Il modello di processo qui presentato è definito sulla base di quello riportato nel documento del NIST Incident Response Recommendations and Considerations for Cybersecurity Risk Management SP 800-61r3." — nota 4 a §2.

## Entità menzionate

- [[entities/ACN]] — autore
- [[entities/CSIRT Italia]] — destinatario delle notifiche, referente operativo
- [[entities/NIST SP 800-61]] — base metodologica del modello

## Concetti collegati

- [[concepts/Notifica di incidente significativo]]
- [[concepts/Incidente significativo]]
- [[concepts/Misure di gestione del rischio cyber]]
- [[concepts/Specifiche tecniche di base]]
- Processo gestione incidenti (5 fasi NIST)

## Note dell'agente

- Il documento è **operativo, non normativo**: serve come "guida alla lettura" delle specifiche di base. Non sostituisce gli allegati 1-4 della det. 379907/2025; li **strutturano lungo il processo NIST**.
- *Sintesi dell'agente:* la scelta di NIST SP 800-61r3 come base è significativa — r3 è recentissimo (2024) e introduce il framework "incident response in the context of cybersecurity risk management", più ampio e moderno di r2. ACN si allinea così alle pratiche internazionali più aggiornate.
- L'aggiornamento v1.1 (apr 2026) è marginale ma testimonia che i documenti di linee guida vengono **manutenuti dinamicamente** in funzione dell'evoluzione del corpus regolatorio (det. 127434/2026 sui termini soggetti 2026 + nuova det. piattaforma e procedure 2026).
