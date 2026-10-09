# Evidence crosswalk — student-facing artifact map

Publisher: Beacon of the Eagle LLC — Centinell Suite Defense

| Student question | Artifact | Evidence field / event |
|---|---|---|
| 1–2 | artifacts/windows/security-events.csv | FS-02, event 4624, svc-backup, source_ip |
| 3–4 | artifacts/windows/security-events.csv | FS-02, event 7045, detail and timestamp_utc |
| 5–6 | artifacts/network/arp-observations.csv | baseline and conflicting mapping for 10.44.2.1 |
| 7 | artifacts/network/switch-port-events.csv | duplicate-gateway-claim |
| 8 | artifacts/network/arp-observations.csv | WS-17 gateway cache changed |
| 9–10 | artifacts/network/dns-poisoning-observations.csv | unexpected resolver and answer |
| 11–13 | artifacts/iot/gateway-audit.csv | change_dns event |
| 14 | artifacts/identity/account-audit.csv | authentication-anomaly |
| 15 | artifacts/network/switch-port-events.csv | port-disabled-by-analyst |

## Evidence interpretation warnings
- A Windows service creation record is not sufficient to establish malicious persistence.
- ARP and DNS anomalies support a poisoning hypothesis but do not establish attacker identity or the tool/OS used.
- A revoked session or disabled port does not demonstrate full eradication.
- Pending restore checks must remain explicitly pending.

The mapping above intentionally names evidence sources but does not reveal the answers.
