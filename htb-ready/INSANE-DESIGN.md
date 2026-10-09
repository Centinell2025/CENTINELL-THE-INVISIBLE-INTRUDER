# INSANE target — design specification (not a verified difficulty)

**Beacon of the Eagle LLC | Centinell Suite Defense**

## Objective
Evolve the current focused Sherlock candidate into a defensible, multi-source, high-complexity blue-team investigation. **Insane is a target, not an approved difficulty or payout guarantee.** The existing 15 questions are simple lookups and do not meet this target.

## Fictional case narrative
An experienced intruder may have abused a service account on FS-02 while a second cluster of network anomalies appears around a gateway MAC conflict, rogue DNS reply and IoT configuration change. The analyst must test whether these observations share an actor or are unrelated. **Do not pre-decide causality.**

## Investigation phases
1. **Evidence trust and provenance:** determine clock skew, missing intervals, sensor reliability, integrity and event normalization. Build an acquisition ledger.
2. **Identity and endpoint:** correlate service-account authentication, service creation, process lineage, scheduled tasks and credential activity. Compare with documented maintenance.
3. **Network deception:** reconstruct ARP/MAC changes, switch learning, DHCP, DNS response timing, gateway reachability and possible MITM without assuming payload compromise.
4. **IoT and cloud dependencies:** trace approved vs unapproved configuration changes; interpret vendor-specific telemetry states only after schema verification.
5. **Impact and recovery:** distinguish observed effects from suspected exfiltration; test backup provenance, integrity and restore validation.
6. **Decision under uncertainty:** propose least-disruptive containment with explicit safety, availability and chain-of-custody tradeoffs.

## Evidence expansion plan (synthetic and reproducible)
- Native-format Windows event export (EVTX or documented JSONL substitute) and Sysmon-like process tree with benign admin baseline.
- Linux auth, journal and command history with provenance and redaction.
- PCAP/PCAPNG with benign background traffic and adversarial hypotheses; full packet capture is generated offline, never from real victims.
- DHCP, DNS, switch CAM/ARP, firewall, NAC and netflow telemetry with independently cross-checkable time windows.
- IoT configuration snapshots, schema, vendor baseline and signed firmware metadata.
- Backup catalog, SHA-256 manifests, restore-test evidence and explicit unknowns.
- Document synthetic generation method, random seed, timestamp model, file hashes and chain-of-custody notes.

## Proposed advanced graded tasks (do not publish answers until evidence exists)
1. Reconstruct the earliest **corroborated** deviation after correcting sensor clock offsets.
2. Identify which successful login cannot be explained by approved maintenance using two sources.
3. Link a suspicious service to a process tree and its parent identity.
4. Determine the exact time interval of gateway MAC takeover using independent switch and endpoint logs.
5. Distinguish the legitimate DHCP source from rogue network activity using lease and packet evidence.
6. Correlate poisoned DNS replies to client resolution and subsequent network traffic; separate attempted from successful redirection.
7. Reconstruct a possible lateral movement chain and mark each link confirmed, probable or unproven.
8. Identify the IoT configuration change and prove which account or API principal made it, if supported.
9. Calculate an evidence-backed incident scope and enumerate unaffected controls.
10. Determine whether claimed exfiltration is supported by payload/flow evidence; avoid inference from a single connection.
11. Identify the earliest trustworthy clean restore point and validate its hash.
12. Demonstrate that post-restoration telemetry and application data pass explicit acceptance tests.
13. Reconcile contradictory artifacts and explain the decisive independent source.
14. Identify the minimal authorized containment sequence preserving critical business services.
15. Construct the final UTC timeline with precise proof references and unresolved uncertainties.

**All proposed tasks above are design prompts, not currently answerable graded questions.** Convert them into exact-answer or bounded multiple-choice questions only after generating evidence and verifying uniqueness.

## Insane quality gates
- [ ] All advanced tasks supported by generated case-specific evidence
- [ ] Native or clearly documented portable artifact formats
- [ ] At least two independent sources per major inference
- [ ] No unsupported attacker attribution or guaranteed zero data loss
- [ ] Instructor-only full solution with exact proof references
- [ ] Automated uniqueness and answer regression checks
- [ ] Independent blind playtest; difficulty and solve time assessed
- [ ] Portable package, checksums and submission rules verified

**Current decision:** Development only. Do not label as completed Insane or submit as such yet.

© 2026 Beacon of the Eagle LLC. All rights reserved.
