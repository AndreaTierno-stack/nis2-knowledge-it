---
title: Evidenze documentali NIS
type: concept
scope: grc_personal
tags: [nis2, italia, specifiche-di-base, compliance, documentazione, audit, grc]
sources: ["[[sources/Guida lettura specifiche di base]]", "[[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]]", "[[sources/Allegato 1 - Misure di sicurezza di base per i soggetti importanti]]", "[[sources/Allegato 2 - Misure di sicurezza di base per i soggetti essenziali]]"]
aliases: [Documentazione NIS, Documenti NIS, Deliverable di compliance NIS, Evidenze NIS]
---

## Definizione

Insieme dei **documenti** che un soggetto NIS deve **possedere o produrre** per dimostrare l'attuazione delle [[concepts/Misure di sicurezza di base|misure di sicurezza di base]]. Sono il **layer di compliance** del regime: ogni audit, ispezione o verifica ACN si svolge a partire da questi documenti.

Tipizzazione e elenco autoritativo: § 2.5 della [[sources/Guida lettura specifiche di base|guida alla lettura]] (per i raggruppamenti) e **Appendice C** (per i documenti soggetti ad approvazione degli organi di amministrazione e direttivi).

## Le 6 tipologie

| Tipologia | Esempi | Riferimento misure |
|---|---|---|
| **Elenchi** | personale dell'organizzazione di sicurezza informatica · configurazioni di riferimento · sistemi accessibili da remoto | `GV.RR-02` · `PR.PS-01` · `PR.AA-05` |
| **Inventari** | apparati fisici · servizi · sistemi e applicazioni software · *flussi di rete*¹ · servizi erogati dai fornitori · fornitori | `ID.AM-01..04` · `GV.SC-04` |
| **Piani** | valutazione dei rischi · continuità operativa · ripristino in caso di disastro · trattamento dei rischi · gestione delle vulnerabilità · adeguamento · valutazione efficacia · formazione · risposta agli incidenti | `ID.RA-05` · `ID.IM-04` · `ID.RA-06` · `ID.RA-08` · `ID.IM-01` · `PR.AT-01` · `RS.MA-01` |
| **Politiche di sicurezza informatica** | sui **16 ambiti** elencati in Tabella 1 degli allegati (gestione rischio, ruoli, HR, audit, supply-chain, asset, vulnerabilità, BC/DR, IAM, sicurezza fisica, formazione, dati, dev/config/dismissione, reti, monitoraggio, risposta incidenti) | `GV.PO-01` |
| **Procedure** | sui requisiti specifici che le richiedono (es. notifica incidenti, dismissione HW, comunicazione ripristino) | vari |
| **Registri** | esiti del riesame delle politiche · attività di formazione del personale · manutenzioni hardware effettuate | `GV.PO-02` · `PR.AT-01` · `PR.PS-03` |

¹ *Solo essenziali (`ID.AM-03`).*

I documenti possono essere **cartacei o digitali**, purché facilmente fruibili da chi ha necessità di consultarli. Il soggetto può **raggruppare o distribuire** i contenuti tra più documenti secondo il proprio contesto organizzativo.

## Appendice C — 11 documenti che richiedono approvazione del board

Lista esatta dei documenti che devono essere **approvati dagli organi di amministrazione e direttivi**, con il requisito che ne richiede l'approvazione:

| # | Documento | Requisito |
|---|---|---|
| 1 | Organizzazione per la sicurezza informatica | `GV.RR-02` p.1 |
| 2 | Politiche di sicurezza informatica | `GV.PO-01` p.3 |
| 3 | Valutazione del rischio posto alla sicurezza dei sistemi informativi e di rete | `ID.RA-05` p.3 |
| 4 | Piano di trattamento del rischio | `ID.RA-06` p.3 |
| 5 | Piano di gestione delle vulnerabilità | `ID.RA-08` p.4 |
| 6 | Piano di adeguamento | `ID.IM-01` p.1 |
| 7 | Piano di continuità operativa | `ID.IM-04` p.4 |
| 8 | Piano di ripristino in caso di disastro | `ID.IM-04` p.4 |
| 9 | Piano di gestione delle crisi | `ID.IM-04` p.4 |
| 10 | Piano di formazione | `PR.AT-01` p.2 |
| 11 | Piano per la gestione degli incidenti di sicurezza informatica | `RS.MA-01` p.2 |

Queste 11 deliberazioni sono la **traduzione operativa** della responsabilità degli organi di amministrazione e direttivi ex **art. 23 decreto NIS** (cfr. [[concepts/Responsabilità degli organi di gestione]]): non basta delegare al CISO, l'organo apicale deve approvare formalmente i documenti elencati.

## Riesami obbligatori (cadenza)

| Documento | Cadenza | Trigger ad-hoc |
|---|---|---|
| Politiche di sicurezza informatica | annuale (`GV.PO-02`) | evoluzioni normative, incidenti significativi, riorganizzazioni, mutamenti di esposizione |
| Organizzazione per la sicurezza informatica (`GV.RR-02`) | biennale | id. |
| Valutazione del rischio (`ID.RA-05`) | biennale | id. |
| Piani BC / DR / crisi (`ID.IM-04`) | biennale | id. |
| Piano risposta incidenti (`RS.MA-01`) | biennale (con integrazione lessons learned) | incidenti significativi, mutamenti minacce |

## Differenza importanti vs essenziali

L'elenco generale è lo stesso, ma per gli **essenziali** la guida segnala in corsivo documenti aggiuntivi o piani arricchiti (es. inventari di flussi di rete via `ID.AM-03`, piano formazione specializzata via `PR.AT-02`, configurazioni di riferimento hardened via `PR.PS-01`, registri di manutenzioni HW via `PR.PS-03`, procedure di comunicazione ripristino via `RC.CO-03`).

## Collegamenti

- [[concepts/Responsabilità degli organi di gestione]] — gli 11 documenti di Appendice C concretizzano l'art. 23 decreto NIS
- [[concepts/Misure di sicurezza di base]] — i documenti sono evidenze delle misure
- [[concepts/Clausole basate sul rischio]] — il piano di trattamento del rischio (doc #4) documenta le deroghe ex C3
- [[concepts/Sistemi informativi e di rete rilevanti]] — l'elenco dei rilevanti (`GV.OC-04`) è un'evidenza richiesta
- [[concepts/Specifiche tecniche di base]]
- [[concepts/Notifica di incidente significativo]] — il piano gestione incidenti (doc #11) governa il processo

## Note dell'agente

- *Sintesi dell'agente:* questa pagina è il **deliverable layer** della compliance NIS. È letteralmente la check-list che un audit di prima istanza utilizza: documento N → richiesto da requisito X → presente / approvato dal board sì o no.
- *Implicazione per la transizione GRC:* per l'autore (una transizione da software engineering a GRC), gli 11 documenti dell'Appendice C sono **il punto di ingresso operativo del mercato della compliance NIS italiana**. La possibilità di costruire **template open-source** dei piani — con frontmatter strutturati, mapping ai requisiti, sezioni di riesame — è un'opportunità di posizionamento concreta (asset GitHub-spendibile).
- I documenti dell'Appendice C **non sono produzione "carta per carta"**: il soggetto può raggruppare o distribuire i contenuti — è la **struttura logica** (con i contenuti minimi richiesti dalle misure citate) che conta, non la forma.
