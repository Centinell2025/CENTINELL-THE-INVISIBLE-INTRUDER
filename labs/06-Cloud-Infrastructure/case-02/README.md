# Case 02 — Excessive IAM privilege

**BEACON OF THE EAGLE LLC | CENTINELL SUITE DEFENSE**

**Fictional enterprise scenario | Training blueprint | Not yet independently validated**

## Investigation objective
A security analyst at the same fictional enterprise must determine whether **excessive iam privilege** occurred, distinguish legitimate activity from suspicious activity, establish affected assets and provide a defensible containment and recovery plan.

## Required evidence to construct
Primary: **IAM policy change history**. Add an independent corroborating source, a benign comparison baseline, synchronized UTC timestamps, acquisition notes and a real SHA-256 manifest after packaging. **These case-specific artifacts have not yet been generated.**

## Five student investigation tasks
1. Identify the earliest suspicious UTC event and its exact artifact row.
2. Identify the relevant identity, source and destination or affected asset using the primary artifact.
3. Correlate the event with an independent source; explain one plausible benign alternative.
4. Determine what the evidence proves, what it does not prove, and the minimum safe containment action.
5. Define restoration acceptance checks, data-integrity validation and residual risk before reopening access.

## Instructor design criteria
Prepare five objectively gradable questions with unique evidence-backed values after the artifacts are built. Keep the private instructor answer key and walkthrough **outside** student-facing material. Conduct a timed blind playtest. Do not invent results or claim successful recovery.

## Containment and recovery safeguards
Obtain incident commander and system owner approval; preserve volatile evidence where safe; isolate only the confirmed scope; revoke affected credentials or sessions as justified; preserve immutable/offline backups; verify clean restore points in isolation; compare checksums and application transaction counts; document RPO/RTO and any data loss. For operational devices use vendor-approved procedures and safety checks.

© 2026 Beacon of the Eagle LLC. All rights reserved.
