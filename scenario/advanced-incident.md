# Advanced incident: aggressive adversary and network poisoning

**Beacon of the Eagle LLC | Centinell Suite Defense**

This **fictional** extension adds an attacker-controlled Kali Linux machine on an isolated training network. The adversary is suspected of ARP spoofing and DNS poisoning, credential misuse, and destructive changes affecting Windows, Linux, and IoT devices. Kali is an analyst attribution hypothesis, not a verified fact merely because tools resemble Kali utilities.

## Scope
- Workstation WS-17 (10.44.2.17)
- File server FS-02 (10.44.2.32)
- Linux jump host LINUX-JUMP-01 (10.44.3.11)
- IoT gateway IOT-GW-01 (10.44.4.1)
- IoT sensor SENSOR-07 (10.44.4.27)
- Suspected rogue device 10.44.2.66 (fictional)

## Objectives
Identify poisoning indicators, establish an evidence-backed timeline, scope compromised systems, preserve volatile evidence, and execute safe staged recovery. No offensive payloads, credential theft, or active attack instructions are included.

## Key uncertainty
ARP/DNS anomalies alone do not establish the identity, operating system, or intent of an adversary. Validate against switch telemetry, DHCP leases, endpoint evidence, and device configuration baselines.

© 2026 Beacon of the Eagle LLC. All rights reserved.
