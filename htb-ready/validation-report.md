# Submission validation report

**Beacon of the Eagle LLC | Centinell Suite Defense**

## Improvements made
- Reduced the graded challenge to 15 exact-answer questions rather than grading speculative conclusions.
- Linked each question to an existing synthetic evidence source.
- Kept enterprise training blueprints separate from the proposed HTB submission.
- Kept instructor answers out of the student package.

## Known evidence limitations
- The dataset is small and CSV-based; realistic EVTX, PCAP, syslog, firmware snapshots and consistent acquisition metadata are still needed for a strong Hard claim.
- No tested restoration or independent student playtest has been performed.
- The operating system used by the suspected adversary is not established.
- The chain of custody template contains empty hashes, not verified hashes.
- The original IoT event named disable_telemetry has ambiguous boolean semantics; it should not be graded until clarified.

## Submission gate
- [ ] Independent verification of each of the 15 exact answers
- [ ] Private instructor walkthrough and answer proofs
- [ ] Clean, portable downloadable student artifact archive
- [ ] Hash manifest calculated from final package bytes
- [ ] Independent timed playtest and difficulty assessment
- [ ] Platform-specific packaging and licensing check

**Decision:** NOT YET READY FOR HTB SUBMISSION.

© 2026 Beacon of the Eagle LLC. All rights reserved.
