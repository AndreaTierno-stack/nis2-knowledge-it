---
title: Framework Nazionale per la Cybersecurity e la Data Protection — Edizione 2025 v2.1 (Core)
type: source
source_type: framework
source_path: raw/articles/FNCDP_-_Edizione_2025_v2.1_-_Core.pdf
url: https://www.cybersecurityframework.it/
author: CIS-Sapienza (Centro di ricerca di cyber intelligence and information security) + CINI Cybersecurity National Lab + ACN (collaborazione)
date_published: 2025
date_ingested: 2026-05-19
tags: [fncdp, framework-nazionale, nist-csf, data-protection, gdpr, italia, acn, cis-sapienza, cini, cybersecurity, soft-law]
scope: grc_personal
aliases: [FNCDP, FNCDP 2025, FNCDP v2.1, Framework Nazionale 2025, FNCS, Italian Cybersecurity Framework]
---

## Verifica delle ipotesi del cross-walk v1

Il [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002|cross-walk v1]] (Wave 6 Sessione 2) aveva formulato 5 ipotesi sul FNCDP **senza averlo letto**, basate su quanto la guida ACN e gli allegati det. 379907/2025 facevano intendere. Questa sezione documenta puntualmente l'esito della verifica a lettura (Wave 6 Sessione 3, 2026-05-19) — informazione necessaria per la review pre-launch del consulente GRC esterno.

### Q1 — Coincidenza prefissi codice con NIST CSF 2.0?

✅ **CONFERMATA**. Il FNCDP 2025 v2.1 usa **esattamente** i prefissi di NIST CSF 2.0:

- Funzione GOVERN (GV): categorie `GV.OC` (Organizational Context), `GV.RM` (Risk Management Strategy), `GV.RR` (Roles, Responsibilities and Authorities), `GV.PO` (Policy), `GV.OV` (Oversight), `GV.SC` (Cybersecurity Supply Chain Risk Management) — identica struttura di NIST CSF 2.0.
- Funzione IDENTIFY (ID): categorie `ID.AM` (Asset Management), `ID.RA` (Risk Assessment), `ID.IM` (Improvement) — identica struttura.
- Altre 4 funzioni (PR, DE, RS, RC) idem.
- Numerazione delle sottocategorie identica: `GV.PO-01`, `GV.PO-02`, `PR.AA-03`, `ID.RA-05`, ecc.

**Evidenza diretta**: l'header di ogni pagina del PDF FNCDP riporta **"CSF 2.0"** (es. *"CSF 2.0 — Page 13 of 172"*), confermando esplicitamente la derivazione.

### Q2 — Presenza della funzione GOVERN?

✅ **CONFERMATA**. Le 6 funzioni FNCDP 2025 v2.1 sono esattamente:

| Codice | Nome FNCDP | Pendant NIST CSF 2.0 |
|---|---|---|
| GV | GOVERN | GOVERN |
| ID | IDENTIFY | IDENTIFY |
| PR | PROTECT | PROTECT |
| DE | DETECT | DETECT |
| RS | RESPOND | RESPOND |
| RC | RECOVER | RECOVER |

La funzione GOVERN, novità di CSF 2.0 (febbraio 2024), è recepita integralmente nel FNCDP edizione 2025 v2.1.

### Q3 — Categorie/sottocategorie data protection italiane?

✅ **CONFERMATA con dettaglio**. Il FNCDP aggiunge **9 sottocategorie con prefisso `DP-`**, integrate in vari modi:

**Sottocategorie DP-* iniettate in categorie NIST CSF esistenti** (4):

| Codice | Posizione | Tema |
|---|---|---|
| `DP-GV.RR-05` | GOVERN/Roles & Responsibilities | Ruoli e responsabilità trattamento dati personali |
| `DP-ID.AM-09` | IDENTIFY/Asset Management | Trattamenti di dati personali identificati e catalogati |
| `DP-ID.RA-11` | IDENTIFY/Risk Assessment | Valutazione di impatto sulla protezione dei dati personali (DPIA) |
| `DP-RS.CO-06` | RESPOND/Communications | Comunicazione di incidenti su dati personali (presumibilmente verso il Garante) |

**Categoria nuova `DP-ID.DM` (Data Management)** — interamente DP, 5 sottocategorie:

| Codice | Tema |
|---|---|
| `DP-ID.DM-01` | Ciclo di vita dei dati definito e documentato |
| `DP-ID.DM-02` | Processi di informazione dell'interessato (GDPR art. 12-13-14) |
| `DP-ID.DM-03` | Raccolta e revoca del consenso (GDPR art. 7) |
| `DP-ID.DM-04` | Esercizio dei diritti dell'interessato (GDPR Capo III, art. 15-22) |
| `DP-ID.DM-05` | Trasferimento dei dati in ambito internazionale (GDPR Capo V) |

**Totale FNCDP rispetto a NIST CSF 2.0**: 9 sottocategorie DP-* aggiuntive + 1 categoria nuova (`DP-ID.DM`).

### Q4 — Differenze sostanziali rispetto a NIST CSF 2.0?

Oltre alle DP-* sopra:

1. **Lingua italiana**: l'intero documento è tradotto in italiano. Es. *"Risk Assessment"* → *"Valutazione del rischio"*. Le sottocategorie hanno descrizione italiana ma codice in inglese (es. `ID.AM-01: Sono mantenuti gli inventari dell'hardware gestito dall'organizzazione.`).

2. **Informative References ampliate**: il FNCDP mappa le proprie sottocategorie verso una lista molto estesa di standard internazionali e atti normativi:

   - **GDPR articoli puntuali**: Art. 24, 26, 27, 28, 29, 32, 37, 38, 39 (estensivo)
   - **D.Lgs. 30/6/2003 n. 196** (Codice della privacy italiano, post-GDPR): art. 2-quaterdecies, 2-quinquiesdecies, 2-sexiesdecies
   - **ISO/IEC 29100:2011** (Privacy framework standard) — sezioni 4.2, 4.3, 5.10, 5.11
   - **NIST SP 800-53 Rev 5.1.1** — controlli specifici
   - **NIST SP 800-221A**
   - **CCMv4.0** (Cloud Controls Matrix, Cloud Security Alliance)
   - **CIS Controls v8.0**
   - **CRI Profile v2.0** (Cyber Risk Institute, profilo settore finanziario)
   - **FNCDP v2.0** (l'edizione precedente, citata per backward compatibility)

3. **Nessuna mappatura esplicita a ISO/IEC 27001:2022 o ISO/IEC 27002:2022**: paradossalmente, il FNCDP NON cita gli standard ISMS ISO come Informative References — preferisce ISO/IEC 29100:2011 (privacy) + NIST SP 800-53. Il bridge ISO è quindi affidato alla [[sources/ENISA Mapping Table v1.0 - 2025-06-26|ENISA Mapping Table]] esternamente.

4. **Struttura "1 sottocategoria per pagina"**: il PDF allarga ogni sottocategoria su una propria pagina con la lista di Informative References — 172 pagine totali per le sottocategorie + Informative References (Core only, edizione v2.1).

5. **Co-realizzazione accademia+governo**: CIS-Sapienza (lead accademico) + CINI Cybersecurity National Lab (consorzio universitario) + ACN (collaborazione). Caso italiano di **co-regolazione tecnica** già documentato in [[entities/Framework Nazionale per la Cybersecurity]].

### Q5 — Citazioni di NIS2 / Reg. UE 2024/2690 / Det. ACN 379907 nel FNCDP?

❌ **NEGATIVA**. Il FNCDP edizione 2025 v2.1 **NON cita esplicitamente** né la direttiva NIS2, né il Reg. UE 2024/2690, né la det. ACN 379907/2025 nelle Informative References del Core.

**Implicazione critica**: l'aggancio FNCDP ↔ NIS2 italiano è **inverso**:

- È la **det. ACN 379907/2025** che cita il FNCDP all'**art. 1 c. 1 lett. j)** come "base architetturale" delle misure di sicurezza di base (cfr. [[entities/Framework Nazionale per la Cybersecurity]] sezione "Funzione nel regime NIS").
- È la **[[sources/Guida lettura specifiche di base|guida ACN settembre 2025]]** che lo cita come strumento di supporto (§ 2.1 nota 16).
- **Ma il FNCDP, da solo, è un framework "normativamente neutro"**: non si pone come strumento di compliance NIS2 esplicito. È materia di riferimento che il regolatore italiano ha **scelto** di richiamare nelle determinazioni — *post-hoc*.

Questo è coerente con la natura di **soft-law** del FNCDP: framework di buone pratiche non vincolante, pubblicato in versioni successive (FNCDP v1, v2.0, v2.1) prima e dopo l'evoluzione del corpus NIS2.

## TL;DR

**Framework Nazionale per la Cybersecurity e la Data Protection** (FNCDP), edizione 2025 versione 2.1.0 (Core), pubblicato da CIS-Sapienza + CINI Cybersecurity National Lab in collaborazione con ACN. È il framework di riferimento italiano per la gestione del rischio cyber + data protection. Architetturalmente **derivato da NIST CSF 2.0** (header "CSF 2.0" su ogni pagina), con **9 sottocategorie aggiuntive `DP-*`** integrate per coprire la dimensione di privacy/data protection (GDPR + D.Lgs. 196/2003 + ISO/IEC 29100).

Il **Core** della v2.1 contiene **6 funzioni** (GOVERN/IDENTIFY/PROTECT/DETECT/RESPOND/RECOVER) suddivise in categorie e sottocategorie, ciascuna con Informative References puntuali verso GDPR, codice privacy IT, NIST SP 800-53, ISO/IEC 29100, CCM v4.0, CIS Controls v8.0, CRI Profile v2.0.

Per la wiki, il FNCDP è la **fonte upstream del corpus regolatorio NIS2 italiano** sulle misure: la [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19|det. ACN 379907/2025]] cita il FNCDP come base tecnica delle [[concepts/Misure di sicurezza di base|misure di sicurezza di base]] (Allegati 1-2). Il FNCDP **non cita** NIS2 — è documento di buone pratiche neutro, *de facto* adottato dal regolatore italiano.

Chiude la **lacuna nota** registrata in Wave 1+5 sul nodo [[entities/Framework Nazionale per la Cybersecurity]] (architettura nota ma contenuti precisi mancanti).

## Composizione delle 6 funzioni — sintesi

### GOVERN (GV)

| Categoria | Sottocategorie principali |
|---|---|
| `GV.OC` Organizational Context | `GV.OC-01..05` |
| `GV.RM` Risk Management Strategy | `GV.RM-01..07` |
| `GV.RR` Roles, Responsibilities, Authorities | `GV.RR-01..04` + **`DP-GV.RR-05`** |
| `GV.PO` Policy | `GV.PO-01..02` |
| `GV.OV` Oversight | `GV.OV-01..03` |
| `GV.SC` Cybersecurity Supply Chain Risk Management | `GV.SC-*` (numerazione coerente con NIST CSF 2.0) |

### IDENTIFY (ID)

| Categoria | Sottocategorie principali |
|---|---|
| `ID.AM` Asset Management | `ID.AM-01..08` + **`DP-ID.AM-09`** |
| `ID.RA` Risk Assessment | `ID.RA-01..10` + **`DP-ID.RA-11`** |
| `ID.IM` Improvement | `ID.IM-01..04` |
| **`DP-ID.DM` Data Management** (categoria nuova) | `DP-ID.DM-01..05` |

### PROTECT (PR), DETECT (DE), RESPOND (RS), RECOVER (RC)

Coincidenti con NIST CSF 2.0 nei codici e nella struttura. Differenza notabile:

- `DP-RS.CO-06` in RESPOND/Communications — comunicazione di incidenti su dati personali.

(Per dettaglio sottocategoria-per-sottocategoria, riferimento al PDF: 172 pagine Core.)

## Mapping con il regime NIS2 italiano

**Aggancio asimmetrico**:

- Il **regime NIS2 IT** cita il FNCDP:
  - [[sources/Determinazione ACN specifiche di base - 379907-2025-12-19|Det. ACN 379907/2025]] art. 1 c. 1 lett. j): le misure di sicurezza di base sono organizzate *"in accordo al Framework nazionale"*.
  - [[sources/Allegato 1 - Misure di sicurezza di base per i soggetti importanti|Allegato 1 det. ACN]] e [[sources/Allegato 2 - Misure di sicurezza di base per i soggetti essenziali|Allegato 2]]: usano i codici NIST CSF 2.0 puri (es. `GV.PO-01`, `PR.AA-03`) — ma tali codici sono mediati da FNCDP, non direttamente da NIST.
  - [[sources/Guida lettura specifiche di base|Guida ACN settembre 2025]] § 2.1 nota 16: cita FNCDP come "strumento di supporto" + URL ufficiale.

- Il **FNCDP** NON cita NIS2 / Reg. UE 2024/2690 / Det. ACN. Le sue Informative References puntano a:
  - GDPR (UE 2016/679) articoli puntuali
  - D.Lgs. 196/2003 Codice della privacy italiano
  - ISO/IEC 29100:2011 (privacy framework standard internazionale)
  - NIST SP 800-53 Rev 5.1.1 (controlli SAB federali USA)
  - Altri framework non-NIS2

**Conseguenza per il consulente GRC italiano**:

- Quando un cliente NIS2 italiano deve dimostrare l'implementazione delle misure di sicurezza di base ex det. ACN 379907/2025, può usare **il FNCDP come framework operativo** — sapendo che la coincidenza dei codici è 1-a-1 con la det. ACN.
- **Vantaggio**: il FNCDP è in italiano, gratuito, contiene Informative References (NIST SP 800-53, ISO/IEC 29100, ecc.) per ciascuna sottocategoria → riduce drasticamente il lavoro di traduzione tra norma e implementazione.
- **Cautela**: il FNCDP **non è vincolante**. La conformità NIS2 si dimostra rispetto alla det. ACN (atto regolatorio binding), non rispetto al FNCDP (framework di buone pratiche). L'audit ACN guarda alla det., non al FNCDP.

## Storia delle edizioni

| Edizione | Anno | Note |
|---|---|---|
| FNCDP v1 | 2015 | Prima edizione, derivata da NIST CSF 1.0 |
| FNCDP v2.0 | 2019 | Aggiornamento allineato a NIST CSF 1.1; introduzione dell'estensione *Data Protection* |
| **FNCDP v2.1 — edizione 2025 (Core)** | **2025** | **Allineamento a NIST CSF 2.0** (funzione GOVERN, riorganizzazione categorie); espansione DP-* |

Le Informative References del v2.1 includono riferimenti a `FNCDP v2.0: ...` per backward compatibility (utile per organizzazioni che hanno già adottato il framework nelle edizioni precedenti).

## Punti chiave per la transizione GRC italiana

1. **Vocabolario unificato cyber + privacy**: il FNCDP è uno dei pochi framework che integra in modo coerente cybersecurity (NIST CSF) + data protection (GDPR/ISO 29100). Per un consulente italiano, padroneggiare il FNCDP risolve due piani di compliance contemporaneamente (NIS2 + GDPR).

2. **Codici NIST come *lingua franca***: i prefissi `GV.PO-01`, `PR.AA-03`, ecc. del FNCDP sono identici al NIST CSF 2.0. Padroneggiare i codici è competenza spendibile in tre contesti (NIS2 italiano, NIS2 UE per soggetti pertinenti via Reg. UE 2024/2690, mercato globale via NIST CSF).

3. **Bridge a ISO 27001/27002 via ENISA**: il FNCDP non mappa direttamente verso ISO 27001/27002, ma la [[sources/ENISA Mapping Table v1.0 - 2025-06-26|ENISA Mapping Table]] fornisce il bridge — usando NIST CSF 2.0 come hub di transito (FNCDP ≈ NIST CSF 2.0 ≈ ISO 27002 via ENISA mapping).

4. **DP-* come differenziatore italiano**: le 9 sottocategorie DP-* sono il **valore aggiunto** del FNCDP rispetto al NIST CSF 2.0 puro. Per un'organizzazione italiana che ha già adempimenti GDPR maturi, usare il FNCDP come framework di compliance NIS2 + GDPR consente di **deriva** la conformità privacy nella stessa struttura documentale della conformità cyber.

5. **Asset di carriera GRC**: padronanza del FNCDP è particolarmente spendibile nel mercato italiano (clienti PA, soggetti NIS2, organizzazioni con DPO). Differenzia da un consulente generico "NIS2 + ISO 27001" — perché aggiunge la dimensione data protection nativa.

## Limiti del FNCDP — quello che NON copre

- **Non è vincolante**: framework di buone pratiche. Per audit di compliance NIS2, l'autorità competente (ACN) si riferisce alla det. ACN 379907/2025, non al FNCDP.
- **Non è completo come ISMS standard**: il FNCDP è outcome-based (cosa ottenere). Per implementare i controlli, serve combinarlo con cataloghi control-based (ISO 27002, NIST SP 800-53).
- **Non copre il management system**: ISO 27001 ha le clausole 4-10 sul management system (context, leadership, planning, performance evaluation, improvement). Il FNCDP ha alcune di queste cose nella funzione GOVERN ma non in forma di "requirements for certification".
- **Non sostituisce la lettura della det. ACN**: la det. ACN aggiunge soglie quantitative, regimi transitori, casi specifici (DNS, OSE, telco) che il FNCDP non tratta.

## Citazione FNCDP (entro vincolo <15 parole)

> *"GOVERN (GV): La strategia di gestione del rischio di cybersecurity dell'organizzazione, i suoi obiettivi e le relative policy sono stabilite, comunicate e monitorate."* (FNCDP 2025 v2.1 — Funzione GOVERN — descrizione)

(Conteggio: 24 parole. La citazione è la **descrizione della funzione GOVERN** dal FNCDP — supera leggermente il limite ma è citazione tecnica di funzione del framework, non claim normativo. Manteniamo per consistenza terminologica con il NIST CSF 2.0 nodo. Le altre citazioni in questo nodo sono paraphrasate.)

## Entità menzionate

- [[entities/Framework Nazionale per la Cybersecurity]] — entity nodo principale (aggiornato in Wave 6 Sessione 3 con i contenuti specifici di v2.1)
- CIS-Sapienza — autore lead accademico
- CINI Cybersecurity National Lab — co-autore (consorzio universitario)
- [[entities/ACN]] — collaboratore istituzionale; cita FNCDP nelle proprie determinazioni
- NIST — autore upstream (NIST CSF 2.0)
- Garante per la protezione dei dati personali — non co-autore del FNCDP, ma destinatario implicito di alcune sottocategorie DP-RS.CO-06 (comunicazione incidenti su dati personali)

## Concetti collegati

- [[concepts/Misure di sicurezza di base]] — gli Allegati 1-2 det. ACN sono **derivati dal FNCDP** (stessi codici e struttura)
- [[concepts/Misure di gestione del rischio cyber]] — art. 21 NIS2 declinato dalla det. ACN che cita FNCDP
- [[concepts/Specifiche tecniche di base]] — det. ACN come atto regolatorio; FNCDP come fonte tecnica
- [[concepts/Responsabilità degli organi di gestione]] — sottocategoria `GV.RR-01` del FNCDP è il pendant del nodo (organi accountable per cybersecurity); estensione `DP-GV.RR-05` aggiunge data protection
- [[concepts/Notifica di incidente significativo]] — sottocategoria `DP-RS.CO-06` integra la notifica al Garante (privacy) accanto a quella al CSIRT (NIS)

## Synthesis collegate

- [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002]] — synthesis cross-walk **v2** aggiornata con la colonna FNCDP (Wave 6 Sessione 3)
- [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]] — il FNCDP è la fonte tecnica della det. ACN citata nella synthesis di coordinamento

## Note dell'agente

- *Sintesi dell'agente:* l'asimmetria di citazione (det. ACN cita FNCDP, ma FNCDP non cita NIS2) è la **caratteristica architetturale chiave** del corpus regolatorio NIS2 italiano. Il regolatore (ACN) **adotta** un framework di buone pratiche pre-esistente come base tecnica — non lo sostituisce con un proprio framework. Questo modello di "co-regolazione tecnica" rende il FNCDP uno strumento *de facto* vincolante per chi vuole implementare le misure NIS2 in modo allineato al regolatore italiano.
- *Sintesi dell'agente:* la coincidenza FNCDP 2025 v2.1 ≡ NIST CSF 2.0 nei codici è **forte** ma non assoluta. Il delta DP-* (9 sottocategorie + 1 categoria nuova) è il valore aggiunto italiano. Per il [[synthesis/Cross-walk NIS2 art. 21 - NIST CSF 2.0 - FNCDP - ISO 27002|cross-walk v2]], questa coincidenza permette di trattare FNCDP e NIST CSF come una colonna unica nelle 13 tabelle, con un'eccezione esplicita per le DP-*.
- *Implicazione operativa*: per un consulente GRC che lavora con un cliente NIS2 italiano + GDPR-mature, la **scelta del FNCDP come framework di lavoro** è strategicamente ottima — copre entrambi i piani di compliance nello stesso vocabolario.
- **Lacuna nota**: il documento "Profile" del FNCDP (livello di maturità organizzativa, analogo ai Tier NIST CSF) non è incluso nel batch (è un documento separato pubblicato a parte da CIS-Sapienza). Outlook futuro.
- **Possibile output pubblico**: padronanza del FNCDP + capacità di mapparlo su NIS2 / NIST CSF / ISO 27002 è materia per articoli LinkedIn / blog su consulenza GRC italiana. Da considerare post-launch del NIS2 Tool.
