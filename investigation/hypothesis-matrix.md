# Forensic hypothesis matrix

**Beacon of the Eagle LLC | Centinell Suite Defense**

| Hypothesis | Supporting artifact | Alternative explanation | Additional test |
|---|---|---|---|
| Gateway impersonation | network/arp-observations.csv | Duplicate address/misconfiguration | Verify switch port ownership and approved gateway MAC |
| DNS manipulation | network/dns-poisoning-observations.csv | Approved temporary resolver | Compare DHCP policy, DNS logs and change tickets |
| Credential misuse | windows/security-events.csv; identity/account-audit.csv | Authorized service activity | Confirm scheduled jobs and service account owner |
| IoT configuration tampering | iot/gateway-audit.csv | Approved maintenance | Check signed change record and configuration backup |
| Possible data transfer | firewall/traffic.csv | Legitimate application telemetry | Inspect authorized proxy logs and application records |

Do not equate suspicious with proven malicious. A Kali Linux operating system is not established by these logs.

© 2026 Beacon of the Eagle LLC. All rights reserved.
