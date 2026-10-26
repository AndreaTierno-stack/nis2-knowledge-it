---
title: Sistemi informativi e di rete rilevanti
type: concept
scope: grc_personal
tags: [nis2, italia, specifiche-di-base, ambito-applicazione, scoping, gv-oc-04]
sources: ["[[sources/Guida lettura specifiche di base]]", "[[sources/Determinazione ACN specifiche di base - 379907-2025-12-19]]", "[[sources/Allegato 1 - Misure di sicurezza di base per i soggetti importanti]]", "[[sources/Allegato 2 - Misure di sicurezza di base per i soggetti essenziali]]"]
aliases: [Sistemi rilevanti, Sistemi informativi rilevanti, Relevant network and information systems, Sistemi NIS rilevanti]
---

## Definizione

Sotto-insieme dei sistemi informativi e di rete di un soggetto NIS sul quale si applicano in modo **ristretto** alcuni requisiti delle [[concepts/Misure di sicurezza di base|misure di sicurezza di base]]. Definito all'**art. 1** della [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19|determinazione obblighi di base]] come:

> *"sistemi informativi e di rete la cui compromissione comporterebbe un **impatto significativo** sulla **riservatezza, integrità e disponibilità** delle attività e dei servizi per i quali il soggetto rientra nell'ambito di applicazione del decreto NIS"*.

È lo **strumento di scoping** primario delle misure: un soggetto NIS non è obbligato a "blindare tutto" ma può circoscrivere il perimetro tecnico ai sistemi che effettivamente sostengono i servizi rilevanti per la classificazione NIS.

## Processo di individuazione — 3 step

Secondo la [[sources/Guida lettura specifiche di base|guida alla lettura]] (§ 2.3.1):

1. **Identifica attività e servizi NIS** = quelli per i quali il soggetto rientra nell'ambito di applicazione del decreto.
2. **Valuta impatto CIA** di una compromissione dei sistemi che li sostengono, in termini di riservatezza, integrità e disponibilità. **Nessuna metodologia obbligatoria** — ogni soggetto sceglie quella adatta al proprio contesto.
3. **Individua come rilevanti** i sistemi per i quali la valutazione produce un **impatto significativo**.

## Misura GV.OC-04 — l'elenco dei rilevanti

L'elenco aggiornato dei sistemi rilevanti è un'**evidenza documentale** richiesta dalla misura **`GV.OC-04`** (entrambi gli allegati). Senza questo elenco, l'applicazione delle clausole basate sui rilevanti non è dimostrabile.

## Funzione regolatoria — la clausola "per almeno i sistemi informativi e di rete rilevanti"

Il concetto opera tramite la **prima delle 4 [[concepts/Clausole basate sul rischio|clausole basate sul rischio]]**:

> *"... per almeno i sistemi informativi e di rete rilevanti ..."*

presente in **13 requisiti** delle misure per soggetti importanti e **22 requisiti** per soggetti essenziali (cfr. Appendice B della [[sources/Guida lettura specifiche di base|guida]]).

Quando un requisito porta questa clausola, il soggetto può limitarne l'applicazione ai soli sistemi rilevanti. Esempio canonico: il test di ripristino dei backup (`PR.DS-11` punto 4 — solo essenziali) si applica almeno ai rilevanti, non necessariamente a tutti i backup.

## Requisiti con la clausola (sintesi)

### Soggetti importanti (13 requisiti)

`GV.RR-04` p.1 · `ID.IM-04` p.1-3 · `PR.AA-01` p.3 · `PR.AA-03` p.2 · `PR.AA-06` p.1 · `PR.DS-01` p.1 · `PR.DS-02` p.1 · `PR.DS-11` p.1 · `PR.PS-04` p.2 · `PR.IR-01` p.1 · `DE.CM-01` p.1.

### Soggetti essenziali (22 requisiti — super-set)

Tutti i precedenti + `ID.RA-01` p.2 (VA/PT obbligatori) · `PR.DS-11` p.3-4 (backup cifrati + test ripristino) · `PR.PS-01` p.1 (hardening) · `PR.PS-03` p.1-2 (dismissione HW) · `DE.CM-01` p.4-6 (filtraggio traffico, parametri quali-quantitativi).

## Applicazione in cascata con altre clausole

Quando un requisito combina questa clausola con `in accordo agli esiti della valutazione del rischio di cui alla misura ID.RA-05`, **si applicano in cascata**: il requisito vale almeno sui sistemi rilevanti *per i quali la valutazione del rischio ne richiede l'attuazione*. Esempio: `PR.AA-03` p.2 (MFA) — almeno sui rilevanti, ma il soggetto può escludere quelli per cui il rischio è trascurabile (es. sistema standalone con accesso fisico controllato).

## Distinzione operativa rispetto ad altri concetti

- **Ambito NIS** (`AMB.SI/NO.*`) → settori e tipologie di soggetto (es. trasporto aereo, sanità, fornitori cloud). Risponde a "**sono nel perimetro NIS**?".
- **Sistemi rilevanti** → risponde a "**quali sistemi del soggetto devo proteggere con il massimo rigore**?". È il **secondo filtro**, applicato all'interno del soggetto già rientrante nell'ambito.
- **Categoria di rilevanza** ([[concepts/Categorie di rilevanza|minimo→alto]]) → classifica il **soggetto** nel suo complesso, non i suoi sistemi. Determina le **misure aggiuntive** (lungo termine), non lo scoping delle misure di base.

## Collegamenti

- [[concepts/Clausole basate sul rischio]] — concetto-parente: le 4 clausole standardizzate
- [[concepts/Misure di sicurezza di base]] — i requisiti che fanno uso della clausola
- [[concepts/Incidenti significativi di base]] — il modello tridimensionale degli incidenti è valutato proprio sui sistemi rilevanti
- [[concepts/Notifica di incidente significativo]] — IS-1..4 si manifestano (tipicamente) sui rilevanti
- [[concepts/Specifiche tecniche di base]]

## Note dell'agente

- *Sintesi dell'agente:* il concetto sposta sul soggetto l'onere di **definire il proprio perimetro tecnico**. È la traduzione operativa del **principio di proporzionalità** ex art. 31 decreto NIS sul piano dell'**ambito** (non delle modalità).
- *Implicazione per la transizione GRC:* l'elenco `GV.OC-04` dei sistemi rilevanti è il **primo deliverable** richiesto in un audit NIS — senza di esso non è possibile verificare l'applicazione di 22 requisiti per gli essenziali / 13 per gli importanti.
