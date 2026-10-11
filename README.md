# CENTINELL — THE INVISIBLE INTRUDER

**BEACON OF THE EAGLE LLC** · **CENTINELL SUITE DEFENSE**  
Cybersecurity · Digital Forensics · Incident Response  
© 2026 Beacon of the Eagle LLC. All rights reserved.

> **Academic-style DFIR training collection · 50 fictional case blueprints · In development**
>
> This repository is **not** an approved HTB Sherlock, a validated collection of 50 playable labs, or a deployed endpoint protection product.

## Start here

| Reader | Where to go | Time |
| --- | --- | --- |
| HTB reviewer / content evaluator | [Submission candidate](htb-ready/README.md) | 2 min |
| Training coordinator | [50-case catalog](CATALOG.md) | 3 min |
| Student / analyst | [Main incident brief](scenario/incident-brief.md) and [evidence](artifacts/) | Self-paced |
| Instructor / QA | [Validation status](htb-ready/validation-report.md) and [audit](htb-ready/instructor-audit.md) | 5 min |

## What problem does it address?

Analysts learn to find suspicious activity that may not trigger a conventional antivirus alert, reconstruct events using independent sources, preserve evidence, contain only verified scope, and plan safe recovery. The training focuses on **analysis and judgment**, not automatic attacker blocking, remote power control, or production security enforcement.

## One fictional enterprise, one continuing story

The core synthetic incident includes unusual service-account activity, a new Windows service, conflicting gateway ARP observations, an unexpected DNS responder, and an IoT gateway configuration change. Students must separate observed facts from assumptions: the artifacts do **not** independently prove attacker identity, exfiltration, a single causal chain, or completed restoration.

## Academic progression

| Level | Focus | Case allocation |
| --- | --- | --- |
| 100 — Foundations | Evidence, timestamps, identity and baseline analysis | See catalog |
| 200 — Applied investigations | Windows, Linux, email and networks | See catalog |
| 300 — Advanced DFIR | Correlation, lateral movement and persistence | See catalog |
| 400 — Enterprise specialties | Cloud, IoT, web and perimeter | See catalog |
| 500 — Expert response | Multistage investigation, recovery and resilience | See catalog |

**Levels are curriculum tags, not verified HTB difficulty ratings.** Cases can be cross-listed by learning objective without moving or duplicating files.

## Lightweight structure

- `CATALOG.md`: concise index of the ten areas and 50 case outlines.
- `labs/`: existing case blueprints, organized by topic; no duplicate level folders.
- `scenario/`, `artifacts/`, `questions/`: current synthetic incident and student evidence.
- `htb-ready/`: focused candidate and transparent quality gates.
- `playbooks/`: authorized defensive investigation and recovery guidance.

## Current state and next quality gates

**Completed:** repository structure, 50 documented scenario outlines, core synthetic logs, focused candidate questions, instructor audit and recovery guidance.

**Not completed/verified:** 50 independent playable evidence packages; unique-answer checks for each case; private instructor walkthrough; final artifact checksums; independent blind playtests; HTB approval or payment.

We will strengthen the **existing** candidate first, then promote additional cases only when evidence, questions, answers and playtesting meet the same standard. Keep instructor answers private.

## Rights and ethics

All companies, people, accounts and incident events inside the training scenario are fictional. Authorized defensive analysis only. [Publisher and ownership statement](BEACON-OWNERSHIP.md). Any external submission or licensing must follow the recipient's current terms.

**Repository:** https://github.com/Centinell2025/CENTINELL-THE-INVISIBLE-INTRUDER


---
**Ethical and educational use / Uso ético y educativo:** This is a fictional or simulated defensive cybersecurity training exercise. Test only systems you own or are explicitly authorized to assess. / Ejercicio de ciberseguridad defensiva ficticio o simulado. Realice pruebas solo en sistemas propios o con autorización expresa. See / Consulte [Educational Purpose Notice](EDUCATIONAL_PURPOSE_NOTICE.md).
