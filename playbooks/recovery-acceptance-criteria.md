# Recovery acceptance criteria — Windows, Linux, IoT

**Beacon of the Eagle LLC | Centinell Suite Defense**

Recovery is complete only after authorized operators verify:

| Control | Evidence required | Pass condition |
|---|---|---|
| Backup provenance | Backup job record, timestamp, immutable/offline status | Source predates confirmed compromise or is independently proven clean |
| Backup integrity | SHA-256 manifest and isolated restore logs | All applicable hashes and checks pass |
| Endpoint integrity | Trusted reimage record, patch level, secure configuration | Known-good baseline met |
| Identity | Credential rotation, session revocation, MFA validation | Compromised access cannot be reused |
| Network | ARP gateway baseline, approved DNS resolver, switch policy | No unauthorized gateway/resolver mappings |
| IoT safety | Vendor-approved firmware, config backup, functional tests | Signed firmware verified where supported; critical functions normal |
| Data completeness | File counts, application checksums, transaction reconciliation | Within approved recovery point objective; discrepancies documented |
| Monitoring | SOC alert tests and post-recovery observations | Telemetry restored and anomaly detection operational |

**Do not promise zero data loss.** If a trusted restore point cannot be verified, preserve the original media and escalate before destructive action. No live recovery tests are claimed in this repository.

© 2026 Beacon of the Eagle LLC. All rights reserved.
