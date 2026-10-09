# Windows and Linux recovery after aggressive intrusion

**Beacon of the Eagle LLC — Centinell Suite Defense**

1. Declare an incident, identify critical services and business continuity constraints, and isolate confirmed affected hosts via EDR, switch, or firewall controls.
2. Acquire and hash forensic images and volatile artifacts before destructive remediation where feasible. Preserve event logs and account activity.
3. From a clean administrative device, disable or rotate compromised identities, invalidate sessions and tokens, and review privileged group membership.
4. Inspect suspicious services, scheduled tasks, autoruns, SSH authorized_keys, systemd units, startup scripts, and remote management settings; validate each against approved baselines.
5. For high-confidence compromise or unknown persistence, rebuild from verified trusted media rather than relying solely on antivirus scans or ad hoc cleanup.
6. Validate backups offline: integrity, date, clean recovery point, malware screening, and restore testing. Keep untrusted backups out of production.
7. Apply security updates, least privilege, MFA, host firewalls, DNS protections, and network segmentation. Remove unapproved remote access.
8. Rejoin production only after endpoint integrity checks, identity validation, application tests, and owner sign-off.
9. Monitor authentication anomalies, new services, outbound flows, ARP conflicts, and DNS resolver changes during an elevated observation period.
10. Preserve the full case record, restoration approvals, residual risk, and lessons learned.

If ransomware or destructive activity is suspected, protect offline backups and do not reconnect restored systems to an untrusted network.

© 2026 Beacon of the Eagle LLC. All rights reserved.
