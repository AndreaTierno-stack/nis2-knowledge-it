---
title: Approccio multi-rischio
type: concept
scope: grc_personal
tags: [nis2, gestione-rischio, multi-risk, all-hazards]
sources: ["[[sources/Direttiva (UE) 2022-2555 (NIS2)]]", "[[sources/D.Lgs. 138-2024 (Decreto NIS)]]", "[[sources/Guida lettura specifiche di base]]"]
aliases: [All-hazards approach, Multi-rischio, Approccio basato su tutti i pericoli]
---

## Definizione

Principio interpretativo introdotto da NIS2 in materia di [[concepts/Misure di gestione del rischio cyber|misure di gestione del rischio]]. Le misure ex Art. 21 NIS2 / Art. 24 D.Lgs. 138/2024 devono **coprire tutti i tipi di rischio** che possono compromettere i sistemi informatici e di rete e l'erogazione dei servizi, **non solo le minacce di natura strettamente "cyber"**.

In senso anglosassone equivale all'**all-hazards approach** della disciplina sulle infrastrutture critiche.

## Sviluppo

- **NIS1**: focus prevalente su minacce di natura cyber (malware, attacchi mirati, vulnerabilità software).
- **NIS2 (Considerando + Art. 21)**: codifica dell'approccio multi-rischio per riflettere la realtà che la **continuità del servizio** è esposta a fattori eterogenei: cyber, fisici, ambientali, errori umani, atti dolosi non cyber.
- **D.Lgs. 138/2024 Art. 24** recepisce direttamente.

## Tipologie di rischio coperte

- **Cyber in senso stretto**: malware, ransomware, intrusioni, exfiltration, DoS.
- **Vulnerabilità tecniche**: bug, configurazioni errate, dipendenze obsolete.
- **Catena di approvvigionamento**: compromissione di fornitori, MSP, MSSP, software supplier.
- **Rischi fisici**: intrusioni fisiche, furti di hardware, incendi, allagamenti, blackout.
- **Rischi ambientali**: eventi naturali (terremoti, alluvioni), guasti infrastrutturali (rete elettrica, connettività).
- **Rischi umani**: errore, negligenza, social engineering, dolo dipendenti.
- **Rischi geopolitici**: sanzioni, embarghi, interruzione fornitori internazionali.

## Conferma sul perimetro degli incidenti notificabili

La [[sources/Guida lettura specifiche di base|guida alla lettura specifiche di base]] (§ 3.1) chiarisce che, **in considerazione dell'approccio multi-rischio** e della definizione di incidente all'art. 2 c.2 lett. t) decreto NIS, **gli incidenti oggetto di notifica ricomprendono anche quelli accidentali** — fault, malfunzionamento dei sistemi (anche da errore umano) — **non solo intenzionali**. Esempio canonico: un fault che impatta la disponibilità del sistema e rompe il livello di servizio atteso (`DE.CM-01`) è IS-3 a tutti gli effetti.

## Collegamento con la BCM/DR

L'approccio multi-rischio fa convergere la cybersicurezza con la **Business Continuity Management** e il **Disaster Recovery**: le misure di **continuità operativa** (ambito 3 dei 10 dell'Art. 24) sono il punto di intersezione naturale.

## Collegamenti

- [[concepts/Misure di gestione del rischio cyber]] — l'approccio multi-rischio è il paradigma sotto cui leggere i 10 ambiti
- [[concepts/Specifiche tecniche di base]] — declinano in dettaglio le misure
- [[concepts/Notifica di incidente significativo]] — la notifica copre incidenti di qualunque origine
