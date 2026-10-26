---
title: ENISA Mapping Table v1.0 — Reg. UE 2024/2690 ↔ standard
type: source
source_type: article
source_path: raw/articles/ENISA_Technical_Implementation_Guidance_Mapping_table_version_1.0.pdf
working_artifact_path: raw/assets/ENISA_Technical_Implementation_Guidance_Mapping_table_version_1.0.xlsx
url: https://www.enisa.europa.eu/sites/default/files/2025-06/ENISA_Technical_Implementation_Guidance_Mapping_table_version_1.0.xlsx
author: ENISA
date_published: 2025-06-26
date_ingested: 2026-05-18
tags: [nis2, enisa, mapping, reg-ue-2024-2690, iso-27001, iso-27002, nist-csf, etsi, cen-ts, framework-nazionali]
scope: grc_personal
aliases: [ENISA Mapping Table, NIS2 Mapping Table, TIG Mapping Table]
---

## TL;DR

Tabella di mappatura ENISA v1.0 di giugno 2025, allegata alla [[sources/ENISA Technical Implementation Guidance v1.0 - 2025-06-26|TIG v1.0]]. Mappa ciascun punto dell'**Allegato del [[sources/Regolamento di esecuzione UE 2024-2690|Reg. UE 2024/2690]]** (13 sezioni, ~60 punti totali) verso 5 famiglie di riferimenti: **ISO/IEC 27001:2022** (clausole + Annex A controls), **NIST Cybersecurity Framework 2.0** (sottocategorie), **ETSI EN 319 401 V3.1.1**, **CEN/TS 18026:2024**, e **framework nazionali NIS2** (per Stato membro che ha contribuito alla consultazione ENISA).

Strumento di **cross-walk operativo**: per un soggetto che già usa ISO 27001 o NIST CSF, la tabella indica quali controlli soddisfano (o sovrappongono) i requisiti del Reg. UE.

## Provenance e politica di citazione

> **Pre-ingest check sul formato (esito Wave 6 Cluster B Sessione 1)**: il file nel batch `raw/articles/ENISA_Technical_Implementation_Guidance_Mapping_table_version_1.0.pdf` è un **PDF v1.7, 33 pagine, con testo selezionabile** (non scansione). L'analisi della struttura del testo estratto rivela tabelle multi-colonna **appiattite** dalla conversione (le celle si sovrappongono in alcuni punti, le righe non sono sempre allineate alle intestazioni). Questo corrisponde allo **Scenario A** del brief Wave 6: il PDF è una **conversione lossy del file Excel ufficiale ENISA**.

### Artefatto ufficiale ENISA (working artifact)

Il **file ufficiale** è in formato `.xlsx`:

> `https://www.enisa.europa.eu/sites/default/files/2025-06/ENISA_Technical_Implementation_Guidance_Mapping_table_version_1.0.xlsx`

Il file Excel è **strutturato per uso operativo** (filtri, celle interattive, ordinamenti). La versione PDF è citabile e referenziabile ma poco utile per consultazione lavorativa.

✅ **Working artifact scaricato (2026-05-18)**: il file `.xlsx` è disponibile in `raw/assets/ENISA_Technical_Implementation_Guidance_Mapping_table_version_1.0.xlsx` (35 KB; autore xlsx: Konstantinos Moulinos, stesso autore della TIG; creato 23/10/2024). Riferimento `working_artifact_path:` nel frontmatter. Il PDF in `raw/articles/` resta la copia citabile.

## Cinque famiglie di riferimenti mappati

| Famiglia | Tipo | Note |
|---|---|---|
| **ISO/IEC 27001:2022** | Standard internazionale ISMS | Clausole (5.2, 5.3, 6.1, ecc.) + Annex A controls (A.5.1, A.5.36, A.8.13, ecc.) |
| **NIST Cybersecurity Framework 2.0** | Framework USA con adozione UE | Sottocategorie (GV.PO-01, PR.AA-05, RS.MA-01, ecc.); il nuovo CSF 2.0 introduce funzione GV (Govern) |
| **ETSI EN 319 401 V3.1.1** | General Policy Requirements for Trust Service Providers | Rilevante per soggetti art. 14 Reg. (trust services) |
| **CEN/TS 18026:2024** | Specifiche tecniche CEN sulla cibersicurezza | Specifica tecnica europea citata cons. 3 Reg. |
| **National frameworks** | Framework cybersecurity nazionali NIS2 | **Esito verificato (2026-05-18) sul `.xlsx` ufficiale**: la colonna contiene **un unico** framework nazionale — *"Cybersecurity Handbook"* (Part A / Part B), citato per la maggior parte dei punti del Reg. Plausibilmente attribuibile a Cipro (CY DSA pubblica un "Cybersecurity Handbook"; non confermato da metadati xlsx). **Il framework italiano [[entities/Framework Nazionale per la Cybersecurity\|FNCDP]] NON è incluso**: l'Italia non ha contribuito al cut-off ENISA, oppure il FNCDP non era nello stato di maturità per essere sottomesso al NIS Cooperation Group work stream on security measures |

## Struttura della tabella

Una **riga per ciascun punto** dell'Allegato Reg. UE 2024/2690 (≈ 60 righe). Colonne:

| Colonna | Contenuto |
|---|---|
| Point No (punto Allegato Reg.) | es. `1.1`, `2.1`, `3.4`, `12.5` |
| Title | es. "Policy on the security of network and information systems" |
| ISO standard 27001:2022 | es. `5.2, A.5.1, A.5.36, A.5.4, 9.3` |
| NIST Cybersecurity Framework v2.0 | es. `PR.AT-02, GV.PO-01, GV.PO-02, GV.OC-03, GV.RM-03` |
| ETSI EN 319 401 | (variabile) |
| CEN/TS 18026:2024 | (variabile) |
| Framework nazionali | (variabile per Stato membro) |

## Esempi di mapping significativi (dal PDF, struttura appiattita)

### Esempio 1 — Policy on N&IS (punto Allegato 1.1)

- **ISO/IEC 27001:2022**: clausola 5.2 (Information security policy), A.5.1 (Policies for information security), A.5.36 (Compliance with policies, rules and standards for information security), A.5.4 (Management responsibilities), clausola 9.3 (Management review).
- **NIST CSF 2.0**: `PR.AT-02`, `GV.PO-01` (Organizational cybersecurity policy), `GV.PO-02` (Cybersecurity policy review), `GV.OC-03` (Legal/regulatory requirements understood), `GV.RM-03` (Cybersecurity risk management activities), `GV.OC-02` (Internal/external stakeholders understood), `ID.IM-01..04` (Improvement).

### Esempio 2 — Risk management framework (punto Allegato 2.1)

- **ISO/IEC 27001:2022**: clausole 6.1, 6.1.2, 6.1.3, 6.2, 8.2, 8.3 + Annex A.5.7, .5.19, .5.20, .5.21.
- **NIST CSF 2.0**: `ID.RA-01..06`, `GV.RM-03`, `ID.RM-01`, `GV.RM-06`, `GV.RR-03`, `ID.IM-01..04`.

### Esempio 3 — Multi-factor authentication (punto Allegato 11.7)

- **ISO/IEC 27001:2022**: A.8.5.
- **NIST CSF 2.0**: `PR.AA-03`.

### Esempio 4 — Asset inventory (punto Allegato 12.4)

- **ISO/IEC 27001:2022**: A.5.9.
- **NIST CSF 2.0**: `ID.AM-01..04`, `ID.AM-07`, `ID.AM-08`, `ID.IM-01..04`.

## Caveat ENISA (citato testuale dalla TIG)

> *"The mapping should not be interpreted as a measure of equivalency among different standards or frameworks. It simply refers to relevant requirements in these standards or frameworks without assessing whether these fully cover the requirements of the regulation."*

> *"Cybersecurity standards or frameworks often address the same cybersecurity concerns but use different language, structures or levels of specificity or detail."*

**Implicazione operativa**: la tabella **non sostituisce** un'analisi di conformità — un soggetto certificato ISO 27001:2022 non è automaticamente conforme al Reg. UE 2024/2690, e viceversa. Lo strumento serve a **ridurre la duplicazione di audit** e a costruire un *crosswalk* ragionato, non a dichiarare equivalenza.

## Versioning

**Importante**: nel pre-ingest check di Wave 6 Sessione 1, il file PDF è stato identificato come "PDF v1.7". Il fix M1 di Wave 6 Sessione 2 (2026-05-19) chiarisce che **"v1.7" si riferisce alla specifica del formato PDF (ISO 32000-1:2008, PDF 1.7)** — è una caratteristica del file binario, non della versione del documento ENISA.

**Versione del documento ENISA**: **v1.0** (giugno 2025), coerente sia per la TIG sia per la Mapping Table. Le due artefatti ENISA sono pubblicate insieme e con stessa numerazione di versione (1.0):

| Artefatto ENISA | Versione documento ENISA | Versione formato file |
|---|---|---|
| Technical Implementation Guidance (TIG) | v1.0 (giugno 2025) | PDF 1.7 |
| Mapping Table | v1.0 (giugno 2025) | PDF 1.7 (PDF in batch) · xlsx (file ufficiale) |

Nessuna rinomina del nodo necessaria (filename `ENISA Mapping Table v1.0 - 2025-06-26.md` è corretto).

**Esito M1**: chiarito; il nodo resta con il nome originale.

## Politica di citazione

- **Citabile** per riferimento operativo (ID di punto + standard + clausola).
- **Non riprodurre tabelle intere** in altri nodi della wiki o in deliverable downstream — citare per ID puntuali.
- **Working artifact preferito**: file `.xlsx` ufficiale ENISA (vedi sopra), per filtraggio operativo.

## Entità menzionate

- [[entities/ENISA]] — autore
- ISO/IEC — fonte degli standard 27001/27002
- NIST — fonte del CSF 2.0
- ETSI — fonte di EN 319 401
- CEN — fonte di CEN/TS 18026
- Stati membri UE — fonti dei national frameworks

## Concetti collegati

- [[concepts/Misure di gestione del rischio cyber]] — art. 21 NIS2 di cui il Reg. è esecutivo; la mapping table copre tutti i requisiti tecnici
- [[concepts/Misure di sicurezza di base]] — il regime IT ha la propria mappatura (Allegato A guida ACN per art. 24 c.2 → codici misure); la Mapping Table ENISA è il pendant UE su standard internazionali
- [[entities/Framework Nazionale per la Cybersecurity]] — pending ingest; sarà confrontato con la presenza/assenza del FNCDP nella mapping table

## Synthesis collegate

- [[synthesis/Risposta TIG ENISA alle Q1-Q4 della coordinamento UE-IT]] — usa la mapping table come uno dei riferimenti
- [[synthesis/Coordinamento Reg UE 2024-2690 e Det ACN 379907-2025]]

## Note dell'agente

- *Sintesi dell'agente:* la mapping table è uno **strumento di carriera GRC ad alto valore**: chi padroneggia la sua lettura può proporre crosswalk Reg. UE 2024/2690 ↔ ISO 27001 ↔ NIST CSF a clienti che già hanno una certificazione e devono dimostrare compliance al Reg. UE senza duplicare gli audit.
- *Implicazione operativa per il NIS2 Tool — pilot Cloud*: il tool non usa la mapping table direttamente nel verdetto, ma può citarla come **risorsa post-verdetto** che il consulente userà per impostare la gap analysis.
- ✅ **xlsx ufficiale scaricato** (2026-05-18, `raw/assets/`).
- **Lacuna verificata (2026-05-18)**: il **FNCDP italiano NON è incluso** nella colonna "National frameworks" del xlsx ufficiale. L'unico framework nazionale presente è il "Cybersecurity Handbook" (Part A/B; plausibilmente CY). *Opportunità GRC italiana*: contribuire al prossimo round di consultazione ENISA per far riconoscere il FNCDP come framework di compliance equivalente al Reg. UE 2024/2690. Per una transizione da software engineering a GRC, è un'opportunità di posizionamento (proporre l'attività ad ACN o al CIS-Sapienza è una mossa networking-friendly).
