# Senior instructor technical audit — 2026-10-09

Publisher: Beacon of the Eagle LLC — Centinell Suite Defense

## Verdict
**NOT SUBMISSION READY.** Current 15 graded questions are mostly one-row CSV lookups. This supports an introductory/medium exercise, not a demonstrated Hard Sherlock. No independent playtest or artifact packaging has been completed.

## Evidence-backed findings
1. Authentication anomaly for svc-backup at 09:02:59Z, failed logon 09:03:12Z, successful logon 09:03:18Z, privilege event 09:05:09Z and new service at 09:08:41Z: suspicious sequence, not proof of malware.
2. Switch learned MAC 02:00:00:00:66:66 on Gi1/0/18 at 09:14:42Z; duplicate gateway claim at 09:14:45Z; WS-17 gateway cache changed at 09:14:51Z. Corroborated network anomaly, not established actor identity.
3. DHCP mapped 10.44.2.66 to that MAC at 09:13:55Z. Unexpected resolver 10.44.2.66 returned 203.0.113.66 for updates.example.org at 09:15:08Z. DNS manipulation hypothesis supported.
4. IoT gateway changed DNS 10.44.4.53 -> 10.44.2.66 at 09:17:01Z, actor 'unknown'. This does not establish who performed it or whether the action was authorized.
5. The IoT action 'disable_telemetry' old=true new=false at 09:18:10Z has ambiguous field semantics. Do not grade it until the logging schema is clarified.
6. Switch port disabled at 09:21:12Z; svc-backup session revoked at 09:35:00Z. These are logged containment actions, not proof that all persistence was eradicated.
7. Restore-validation records show WS-17 forensic image complete, but WS-17 reimage planned, FS-02 backup hash pending, IoT firmware signature pending and SENSOR-07 telemetry test pending. No completed full restoration is demonstrated.

## Instructional design problems
- 15 questions mostly direct value retrieval; minimal multi-artifact reasoning.
- Student-facing answers are obtainable from short files without investigative filtering or competing benign signals.
- Chronology must distinguish correlation from causation. Earlier Windows events cannot be attributed to later ARP/DNS anomalies without a bridging artifact.
- CSV data is illustrative rather than native forensic evidence (EVTX, PCAP, syslog, system images); acquisition provenance and verified SHA-256 manifest are absent.
- Some IPs use documentation ranges appropriately; all scenario infrastructure remains fictional.
- The 50 enterprise cases in /labs are scenario blueprints, not 50 tested executable labs.

## Prioritized acceptance gates
P0: Produce private instructor key with exact evidence row and answer for each graded question; do not publish it in the student repo.
P0: Verify answer uniqueness by an automated parser over final artifacts; independently playtest.
P0: Clarify IoT telemetry action semantics in a separate source-schema document rather than silently altering synthetic evidence.
P1: Add realistic noise and multiple independent evidence sources while preserving answer uniqueness.
P1: Build a real downloadable evidence archive and compute actual SHA-256 checksums of the final bytes.
P1: Add multi-source correlation questions and difficulty calibration from timed blind playtest.
P1: Confirm HTB packaging, originality, intellectual property and current submission rules before upload.

**No acceptance, payout, successful restore, or HTB difficulty classification is asserted.**
