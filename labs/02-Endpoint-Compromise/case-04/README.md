# Case 04: Persistence via scheduled task

**Beacon of the Eagle LLC — Centinell Suite Defense**  
**Scenario:** synthetic enterprise DFIR exercise  
**Attack surface:** Internal activity or lateral movement within enterprise  
**Status:** investigation blueprint (not a completed validated lab)

## Situation
Security monitoring flags indicators consistent with **persistence via scheduled task** in the continuing fictional enterprise. The analyst must determine whether an attack occurred, what assets are affected, and whether the event is a false positive. No adversary behavior is assumed proven.

## Evidence to collect (authorized and read-only where possible)
1. UTC logs from relevant endpoints, identity systems, network controls and applications.
2. Asset inventory, baseline configurations, change tickets and account ownership records.
3. Current connections and volatile state when safe, followed by verified forensic copies with SHA-256 hashes.
4. Backup catalog, restore point timestamps, immutable/offline copy status and application consistency checks.

## Investigation questions
1. What is the earliest corroborated suspicious event and which artifact proves it?
2. What entry point and trust boundary are implicated?
3. Which users, hosts, applications and data sets might be affected?
4. What benign explanation could produce similar indicators?
5. What additional evidence would confirm or refute compromise?

## Defensive containment
- Coordinate incident commander, system owner, SOC and operations; record approval and change window.
- Preserve evidence before destructive actions, except where immediate safety demands containment.
- Isolate affected sessions, hosts, network segments or access paths using approved controls while preserving unaffected business services.
- Protect backups and stop replication of suspected corruption; avoid indiscriminate shutdowns or deletion.

## Eradication and recovery
1. Identify and close the confirmed root cause (patch, configuration, access, or trusted rebuild).
2. Revoke compromised sessions and credentials from a clean administration device where applicable.
3. Validate offline/immutable backups and perform an isolated test restore; choose a clean recovery point aligned with the RPO.
4. Rebuild or restore affected assets using trusted vendor media and approved procedures.
5. Verify file hashes, record counts, application transactions, permissions, device safety and normal telemetry before reconnecting.
6. Restore service in stages with owner sign-off and heightened monitoring; document any irrecoverable gap honestly.

## Data preservation gate
**Never promise zero data loss without verified backup coverage.** If no trusted copy exists, halt destructive remediation, preserve current media, and escalate to specialist recovery. Define RPO/RTO and compare recovered datasets against known-good baselines.

## Student deliverable
Produce a UTC timeline, evidence table with hashes, reasoned findings, containment decision log, restoration checklist and residual-risk statement. Instructor grading and solutions remain private.

© 2026 Beacon of the Eagle LLC. All rights reserved.
