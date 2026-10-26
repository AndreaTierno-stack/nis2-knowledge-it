---
title: Misure di gestione del rischio cyber
type: concept
scope: grc_personal
tags: [nis2, obblighi, gestione-rischio, art-21, art-24]
sources: ["[[sources/Direttiva (UE) 2022-2555 (NIS2)]]", "[[sources/D.Lgs. 138-2024 (Decreto NIS)]]", "[[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]]", "[[sources/Determinazione ACN termini soggetti 2026 - 2026-04-30]]", "[[sources/Guida lettura specifiche di base]]"]
aliases: [Misure di sicurezza NIS2, Misure ex Art 24, Misure ex Art 21]
---

## Definizione

Insieme di **dieci ambiti minimi** di misure tecniche, operative e organizzative che i [[concepts/Soggetti essenziali e importanti|soggetti essenziali e importanti]] devono adottare per gestire i rischi cyber che incombono sui propri sistemi informatici e di rete e sull'erogazione dei propri servizi.

Disciplinati da:
- **NIS2 — Articolo 21** (direttiva).
- **D.Lgs. 138/2024 — Articolo 24** (Italia).

I dieci ambiti **devono essere proporzionati** all'esposizione al rischio, alla dimensione, alla criticità del soggetto ([[concepts/NIS2|principio di proporzionalità]] codificato in Art. 31 D.Lgs. 138/2024).

## I 10 ambiti minimi (Art. 24 D.Lgs. 138/2024)

1. **Politiche di analisi dei rischi e di sicurezza dei sistemi informatici e di rete**.
2. **Gestione degli incidenti**.
3. **Continuità operativa** — backup, disaster recovery, gestione delle crisi.
4. **Sicurezza della catena di approvvigionamento (supply chain)** — relazione con fornitori e prestatori di servizi.
5. **Sicurezza nell'acquisizione, sviluppo e manutenzione** dei sistemi informatici e di rete, inclusa gestione e divulgazione delle vulnerabilità.
6. **Politiche e procedure per valutare l'efficacia** delle misure di gestione del rischio.
7. **Pratiche di igiene di base** e **formazione in materia di cibersicurezza**.
8. **Politiche e procedure relative all'uso della crittografia** e, se del caso, della cifratura.
9. **Sicurezza delle risorse umane**, **politiche di controllo dell'accesso**, **gestione degli attivi**.
10. **Autenticazione a più fattori (MFA)** o **autenticazione continua**, **soluzioni di comunicazione vocale, video e di testo protette**, **comunicazioni di emergenza protette** all'interno del soggetto.

## Approccio multi-rischio

L'Art. 24 (e l'Art. 21 della direttiva) impone esplicitamente l'**[[concepts/Approccio multi-rischio|approccio multi-rischio]]**: le misure devono coprire **tutti i tipi di rischio** che possono compromettere il sistema, **non solo cyber** in senso stretto. Inclusi: rischi fisici (intrusione, incendio, allagamento), errore umano, atti dolosi, errori sistemici, malfunzionamenti hardware.

## Mappatura art. 24 c.2 → codici misure di sicurezza di base

L'**Appendice A** della [[sources/Guida lettura specifiche di base|guida alla lettura specifiche di base]] è la "stele di Rosetta" tra i 10 elementi astratti dell'art. 24 c.2 e i **codici delle misure di sicurezza di base** ([[concepts/Misure di sicurezza di base|Allegati 1-2]] della det. 379907/2025):

| Elemento art. 24 c.2 | Codici misure di sicurezza di base |
|---|---|
| a) Politiche analisi rischi + sicurezza sistemi | `GV.OC-04`, `GV.RM-03`, `GV.RR-02`, `GV.PO-01`, `GV.PO-02`, `ID.RA-05`, `ID.RA-06` |
| b) Gestione incidenti (incl. notifiche art. 25-26) | `PR.PS-04`, `DE.CM-01`, `DE.CM-09`, `RS.MA-01`, `RS.CO-02`, `RC.RP-01`, `RC.CO-03` |
| c) Continuità operativa (backup, DR, crisi) | `ID.IM-04`, `PR.DS-11` |
| d) Sicurezza catena di approvvigionamento | `GV.SC-01`, `GV.SC-02`, `GV.SC-04`, `GV.SC-05`, `GV.SC-07` |
| e) Sicurezza acquisizione/sviluppo/manutenzione + vulnerabilità | `GV.SC-05`, `ID.RA-01`, `ID.RA-08`, `PR.PS-01`, `PR.PS-02`, `PR.PS-03`, `PR.PS-06` |
| f) Politiche valutazione efficacia misure | `ID.IM-01` |
| g) Pratiche di igiene base + formazione | `PR.AT-01`, `PR.AT-02` |
| h) Crittografia + cifratura | `PR.DS-01`, `PR.DS-02` |
| i) Sicurezza/affidabilità HR + controllo accessi + asset | `GV.RR-04`, `ID.AM-01`, `ID.AM-02`, `ID.AM-03`, `ID.AM-04`, `PR.AA-01`, `PR.AA-03`, `PR.AA-05`, `PR.AA-06`, `PR.IR-01` |
| l) MFA / autenticazione continua / comunicazioni protette / emergenza | `PR.AA-03`, `PR.DS-02`, `PR.IR-03` |

> *Note redazionali:* (1) la lettera **i)** della tabella di art. 24 c.2 raggruppa HR + controllo accessi + asset; nella numerazione del decreto le lettere sono a-l (senza j-k che sono usate solo nella numerazione alternativa). (2) Le misure marcate con codici "solo essenziali" (`ID.AM-03`, `PR.AT-02`, `PR.PS-01`, `PR.PS-03`, `PR.IR-03`, `RC.CO-03`) si applicano solo all'Allegato 2.

## Specifiche tecniche

L'Art. 27 D.Lgs. 138/2024 affida alle **[[concepts/Specifiche tecniche di base|determinazioni del Direttore generale ACN]]** il compito di **dettagliare** ciascun ambito con specifiche tecniche concrete. Le linee guida ENISA forniscono ulteriore standard di riferimento UE.

La concretizzazione operativa è la **[[sources/Determinazione ACN specifiche di base - 379907-2025-12-19|determinazione ACN n. 379907 del 19/12/2025]]**, che individua le **[[concepts/Misure di sicurezza di base|misure di sicurezza di base]]** (Allegato 1 per soggetti importanti, Allegato 2 per soggetti essenziali). Termini di adozione:
- **Coorte 2025**: 18 mesi dall'entrata in vigore della determinazione.
- **Coorte 2026**: entro il **31 luglio 2027** ([[sources/Determinazione ACN termini soggetti 2026 - 2026-04-30]]).

## Responsabilità degli organi di gestione

L'Art. 23 D.Lgs. 138/2024 (Art. 20 NIS2) attribuisce agli **organi di amministrazione e direttivi** la responsabilità di **approvare** le misure, **vigilare** sull'attuazione, **rispondere** delle violazioni e seguire **formazione periodica**.

## Collegamenti

- [[concepts/Approccio multi-rischio]]
- [[concepts/Specifiche tecniche di base]]
- [[concepts/Misure di sicurezza di base]] — Allegati 1-2 della det. 379907/2025
- [[concepts/Clausole basate sul rischio]] — le 4 clausole che modulano i requisiti delle misure
- [[concepts/Sistemi informativi e di rete rilevanti]] — scoping primario
- [[concepts/Evidenze documentali NIS]] — layer documentale di compliance
- [[concepts/Processo gestione incidenti NIS]] — declinazione operativa dell'ambito 2 (gestione incidenti)
- [[concepts/Notifica di incidente significativo]] — obbligo speculare reattivo
- [[concepts/Sanzioni NIS2]] — sanzioni in caso di violazione
- [[entities/ACN]]
