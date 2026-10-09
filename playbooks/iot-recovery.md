# IoT recovery after suspected poisoning

**Defensive recovery only | Beacon of the Eagle LLC — Centinell Suite Defense**

1. Identify the IoT device owner, safety criticality, maintenance window, and approved recovery procedure. Never power-cycle safety-critical equipment without operational approval.
2. Segment affected IoT VLANs and restrict untrusted routes while preserving required safety and monitoring paths.
3. Preserve device logs, configuration snapshots, firmware versions, and gateway network settings. Hash exported files.
4. Compare DNS, gateway, NTP, certificates, firmware signatures, and configuration against a trusted baseline.
5. Replace altered settings using a verified offline backup or vendor-approved secure reprovisioning; do not trust backups made after suspected compromise without validation.
6. Rotate device and management credentials, revoke affected tokens/certificates, and disable unknown management accounts from a trusted administrative workstation.
7. Update to vendor-signed firmware if appropriate; validate device identity, secure boot where supported, and communications to known endpoints.
8. Restore one device or segment at a time; test telemetry, time sync, network isolation, alarms, and normal operations.
9. Monitor for recurrence of ARP conflicts, rogue DNS answers, and unexpected management activity.
10. Keep the segment isolated and escalate to the vendor if device integrity cannot be established.

Do not assume factory reset guarantees removal of persistent compromise. Preserve safety and vendor support requirements.

© 2026 Beacon of the Eagle LLC. All rights reserved.
