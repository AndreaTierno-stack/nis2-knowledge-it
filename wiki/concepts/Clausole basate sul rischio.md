---
title: Clausole basate sul rischio
type: concept
scope: grc_personal
tags: [nis2, italia, specifiche-di-base, approccio-rischio, art-31, id-ra-05, id-ra-06]
sources: ["[[sources/Guida lettura specifiche di base]]", "[[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]]", "[[sources/Allegato 1 - Misure di sicurezza di base per i soggetti importanti]]", "[[sources/Allegato 2 - Misure di sicurezza di base per i soggetti essenziali]]"]
aliases: [Approccio basato sul rischio NIS, Clausole modulanti, Risk-based clauses NIS]
---

## Definizione

Insieme delle **4 clausole linguistiche standardizzate** che ricorrono nei requisiti delle [[concepts/Misure di sicurezza di base|misure di sicurezza di base]] (Allegati 1 e 2 della [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19|det. 379907/2025]]) e che **modulano** l'ambito o la modalità di applicazione del requisito in funzione del rischio specifico del soggetto.

Sono la **traduzione testuale** dell'art. 31 del decreto NIS — che impone di tener conto, nello stabilire gli obblighi, del *grado di esposizione dei soggetti ai rischi, delle dimensioni e della probabilità che si verifichino incidenti*. Documentate sistematicamente in **Appendice B** della [[sources/Guida lettura specifiche di base|guida alla lettura]].

## Le 4 clausole

| Clausola | Effetto | Req. SI | Req. SE |
|---|---|---|---|
| **C1.** `per almeno i sistemi informativi e di rete rilevanti` | restringe l'**ambito** ai sistemi rilevanti ex `GV.OC-04` | 13 | 22 |
| **C2.** `in accordo agli esiti della valutazione del rischio di cui alla misura ID.RA-05` | definisce **modalità e ambito** in funzione del risk assessment | 6 | 10 |
| **C3.** `fatte salve motivate e documentate ragioni normative o tecniche` | consente **deroga** con motivazione documentata + misure compensative ex `ID.RA-06` p.2 | 8 | 10 |
| **C4.** `forniture con potenziali impatti sulla sicurezza dei sistemi informativi e di rete` | restringe l'ambito alle **forniture rilevanti** ex definizione art. 2 c.1 lett. q) decreto NIS | 3 | 3 |

> **Applicazione in cascata.** Quando un requisito presenta più clausole, queste si applicano in cascata. Esempio: `PR.AA-03` p.2 (MFA) ha C1 + C2 → MFA almeno sui rilevanti, eventualmente esclusi quelli per cui la valutazione del rischio mostra rischio trascurabile.

## C1 — "per almeno i sistemi informativi e di rete rilevanti"

Restringe l'ambito di applicazione del requisito ai soli [[concepts/Sistemi informativi e di rete rilevanti|sistemi rilevanti]]. La pagina dedicata copre il dettaglio.

Esempio canonico: `PR.DS-11` p.4 (test di ripristino backup) — solo sui rilevanti.

## C2 — "in accordo agli esiti della valutazione del rischio di cui alla misura ID.RA-05"

Definisce **modalità** (come si applica il requisito) e/o **ambito** (dove si applica) in funzione della valutazione del rischio fatta ex misura **`ID.RA-05`**.

- **Esempio modalità**: `PR.AA-01` p.2 (credenziali utenze robuste e aggiornate) — frequenza/complessità maggiori per utenze admin (alto rischio).
- **Esempio ambito**: `PR.AA-03` p.2 (MFA) — su quali sistemi rilevanti applicarla; esclusione possibile per sistema standalone con accesso fisico controllato.

Distinzione con C1 (cfr. guida § 2.3.2, nota 25): C1 definisce l'ambito **sui rilevanti**, C2 definisce l'ambito **sul rischio**; possono combinarsi.

## C3 — "fatte salve motivate e documentate ragioni normative o tecniche"

Consente al soggetto di **derogare** dall'applicazione del requisito quando:

- **Vincoli normativi** (leggi/regolamenti che vietano o modificano l'implementazione);
- **Vincoli tecnici** (limiti tecnologici/funzionali).

In caso di deroga il soggetto deve:

1. **Motivare e documentare** il vincolo.
2. **Adottare misure di mitigazione compensative**, ove applicabile (ex `ID.RA-06` p.2).
3. **Inserire nel piano di trattamento del rischio** la descrizione delle misure compensative e dell'eventuale rischio residuo.

**Caveat**: la possibilità di deroga **non si estende** ai **requisiti non derogabili** elencati in **Tabella 2** degli allegati (cfr. [[concepts/Misure di sicurezza di base]] § Tabella 2). Per quei requisiti, anche in presenza di vincoli, l'applicazione è dovuta — ma le misure compensative restano necessarie.

Esempio: `DE.CM-09` p.1 (EDR endpoint) — può essere derogata su endpoint come dispositivi medici dove l'installazione invaliderebbe la certificazione del dispositivo.

## C4 — "forniture con potenziali impatti sulla sicurezza"

Restringe l'ambito ai contratti di fornitura la cui compromissione potrebbe avere effetti sulla sicurezza dei sistemi informativi e di rete del soggetto (= sulla loro capacità di resistere agli eventi che ne minano CIA, in coerenza con la definizione di "sicurezza" all'art. 2 c.1 lett. q) decreto NIS).

Presente in soli 3 requisiti (entrambi gli allegati): `GV.SC-01` p.1, `GV.SC-04` p.1, `GV.SC-05` p.1 (catena di approvvigionamento).

## Mappatura sintetica requisiti → clausole

### Soggetti importanti

| Clausola | Requisiti |
|---|---|
| C1 | `GV.RR-04` p.1 · `ID.IM-04` p.1-3 · `PR.AA-01` p.3 · `PR.AA-03` p.2 · `PR.AA-06` p.1 · `PR.DS-01` p.1 · `PR.DS-02` p.1 · `PR.DS-11` p.1 · `PR.PS-04` p.2 · `PR.IR-01` p.1 · `DE.CM-01` p.1 |
| C2 | `PR.AA-01` p.1-2 · `PR.AA-03` p.2 · `PR.DS-01` p.1 · `PR.DS-02` p.1 · `PR.PS-02` p.1 |
| C3 | `GV.SC-05` p.1 · `PR.AA-01` p.1 · `PR.DS-01` p.1-2 · `PR.DS-02` p.1 · `PR.PS-02` p.1-2 · `DE.CM-09` p.1 |
| C4 | `GV.SC-01` p.1 · `GV.SC-04` p.1 · `GV.SC-05` p.1 |

### Soggetti essenziali (super-set + delta)

| Clausola | Requisiti aggiuntivi rispetto agli importanti |
|---|---|
| C1 | + `ID.RA-01` p.2 · `PR.DS-11` p.3-4 · `PR.PS-01` p.1 · `PR.PS-03` p.1-2 · `DE.CM-01` p.4-6 |
| C2 | + `GV.RR-04` p.4 · `PR.DS-11` p.4 · `PR.PS-02` p.4 · `PR.IR-03` p.1 |
| C3 | + `ID.RA-01` p.2 · `PR.PS-02` p.4 |
| C4 | (identici agli importanti) |

Riferimento autoritativo: **Appendice B** della [[sources/Guida lettura specifiche di base|guida alla lettura]].

## Collegamenti

- [[concepts/Sistemi informativi e di rete rilevanti]] — concetto-figlio della clausola C1
- [[concepts/Misure di sicurezza di base]] — i requisiti che fanno uso delle 4 clausole
- [[concepts/Specifiche tecniche di base]]
- [[concepts/Approccio multi-rischio]] — principio normativo di rango superiore (art. 21 NIS2)
- [[concepts/NIS2]] — principio di proporzionalità ex art. 31

## Note dell'agente

- *Sintesi dell'agente:* le 4 clausole sono il **vocabolario operativo dell'approccio risk-based** delle specifiche di base. Senza padroneggiarle, un requisito letto in isolamento sembra rigido; con le clausole, lo stesso requisito diventa modulabile — ed è qui che il regime smette di essere "checklist" e inizia ad essere "risk management".
- *Implicazione per la transizione GRC:* la mappatura clausole → requisiti è il **piano di lavoro** di un'audit NIS pragmatico. Per ogni requisito si chiede: quali clausole modulano il requisito? Il soggetto ha la documentazione che giustifica come le ha applicate (elenco rilevanti, esiti `ID.RA-05`, motivazione deroghe, perimetro forniture)?
