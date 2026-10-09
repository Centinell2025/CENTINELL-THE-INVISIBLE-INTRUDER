# Student investigation questions

For every answer cite the exact artifact and log row. UTC timestamps must use ISO 8601 when available.

1. Which workstation IP first appears as the source of the suspicious file-server authentication sequence?
2. What service account has both a failed and successful network logon in close succession?
3. Give the UTC timestamp of the successful network logon to the file server.
4. Which event ID records special privileges being assigned on the file server?
5. Which new service name should investigators review as possible persistence?
6. Which internal source IP initiated the successful SSH authentication to the Linux jump host?
7. Which SSH authentication method succeeded?
8. At what UTC time did the first connection to the external documentation-range endpoint occur?
9. Which destination port was used for that external connection?
10. What DNS hostname resolved to the external endpoint?
11. Identify the two outbound firewall rows of interest and compute their combined bytes_out.
12. What evidence supports lateral movement, and which claims remain unproven without additional telemetry?

**Important:** These records are deliberately limited; an outbound connection alone does not prove exfiltration and a new service alone does not prove malicious persistence.
