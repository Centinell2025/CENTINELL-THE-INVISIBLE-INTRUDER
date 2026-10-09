# Evidence-backed incident timeline (UTC)

**Beacon of the Eagle LLC | Centinell Suite Defense**

| Time | Observation | Evidence |
|---|---|---|
| 09:02:59 | Service account authentication anomaly | artifacts/identity/account-audit.csv |
| 09:03:18 | Network logon to file server | artifacts/windows/security-events.csv |
| 09:14:45 | Conflicting gateway MAC observed | artifacts/network/arp-observations.csv |
| 09:15:08 | Unexpected DNS resolver and answer | artifacts/network/dns-poisoning-observations.csv |
| 09:16:11 | Successful SSH public-key authentication | artifacts/linux/auth.log (date lacks year; inferred from scenario context) |
| 09:17:01 | IoT gateway DNS changed | artifacts/iot/gateway-audit.csv |
| 09:21:12 | Suspicious switch port disabled | artifacts/network/switch-port-events.csv |
| 09:27:04 | Outbound TLS connection observed | artifacts/firewall/traffic.csv |

**Analyst caution:** This is a chronology, not a proven causal chain. Preserve evidence and investigate whether events share a common actor.

© 2026 Beacon of the Eagle LLC. All rights reserved.
