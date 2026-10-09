# Forensic investigation playbook

**Beacon of the Eagle LLC — Centinell Suite Defense**

1. Obtain written scope and open a case with a unique ID.
2. Preserve original log exports and record SHA-256 hashes, acquisition times, handlers, and storage locations.
3. Capture volatile state when safe: current sessions, network connections, ARP cache, DNS cache, running services, and switch port information. Avoid altering live systems unnecessarily.
4. Correlate switch ARP observations, endpoint cache changes, resolver changes, authentication, and firewall events.
5. Examine Windows event 4624/4625/4672/7045, Linux SSH records, and IoT configuration audits.
6. Distinguish observation from hypothesis. Do not assert Kali use, exfiltration, or attacker identity without corroboration.
7. Build a UTC timeline and identify affected assets, recovery dependencies, and missing evidence.
8. Document each finding with artifact path, original row, analyst, confidence, and alternative explanations.

**Evidence integrity:** maintain a chain-of-custody register and preserve originals. Synthetic artifacts in this repository are not live forensic evidence.

© 2026 Beacon of the Eagle LLC. All rights reserved.
