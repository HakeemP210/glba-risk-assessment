# GLBA Safeguards Rule Risk Assessment Program

![Regulation](https://img.shields.io/badge/regulation-16%20CFR%20314-183A61)
![Framework](https://img.shields.io/badge/framework-NIST%20CSF%202.0-3765A0)
![Sector](https://img.shields.io/badge/sector-Title%20IV%20Higher%20Ed-557C94)
![Status](https://img.shields.io/badge/status-Risk%20Assessment%20Complete-2E7D4F)

> **A note on what's real here:** the procedure, framework mapping, document structure, and artifacts in this repo come directly from a GLBA Safeguards Rule risk assessment I built for the institution I work for. The *institution's identity* does not appear anywhere in this repo, and any document screenshots have identifying details and personal names blurred or masked before they go in. The procedures and the work are real, the "who" is deliberately generic.

I handle regulatory compliance for a Title IV institution, and one of my responsibilities was building out our GLBA Safeguards Rule Information Security Program from the ground up. Not auditing an existing one, actually building it including the risk assessment, the safeguards, the testing plan, the incident response plan, all of it. The written risk assessment required under 314.4(b) has been completed and includes an asset inventory, threat/vulnerability analysis, a scored 18-item risk register, and a full compliance crosswalk. I'm packaging the procedures here to have a clean public writeup of how a real 314.4 program comes together end to end.

This is a living project meaning the risk assessment itself is done, but safeguards implementation, service provider remediation, and future review cycles will keep this updated going forward.

## Why GLBA + NIST CSF 2.0

TThe Safeguards Rule under 16 CFR § 314.4 does not mandate the use of a specific cybersecurity framework. However, structuring the information security program around an established framework makes the program more defensible, consistent, and adaptable. [NIST CSF 2.0](03-risk-assessment-methodology.md)'s six functions (Govern, Identify, Protect, Detect, Respond, Recover) map cleanly onto 314.4's nine sub-elements, so a single crosswalk can therefore serve two purposes.It demonstrates how the institution addresses the Safeguards Rule requirements. It also gives the information security program a recognized structure that can be easily understood by reviewers, auditors, and cybersecurity professionals.

## Walkthrough

Each element of 16 CFR § 314.4 has its own dedicated write-up that documents the step-by-step process, explains how the requirement was addressed, and outlines why it is important. Each section also includes screenshots of the actual, sanitized artifacts created during the implementation process.

| 314.4 | Element | Doc |
|---|---|---|
| (a) | Governance & Qualified Individual designation | [`01-governance-qi-designation.md`](docs/01-governance-qi-designation.md) |
| (b) | Asset & data inventory | [`02-asset-data-inventory.md`](docs/02-asset-data-inventory.md) |
| (b) | Risk assessment methodology & NIST CSF 2.0 crosswalk | [`03-risk-assessment-methodology.md`](docs/03-risk-assessment-methodology.md) |
| (c) | Safeguards gap analysis (8 required categories) | [`04-safeguards-gap-analysis.md`](docs/04-safeguards-gap-analysis.md) |
| (d) | Testing & monitoring plan | [`05-testing-monitoring-plan.md`](docs/05-testing-monitoring-plan.md) |
| (h) | Incident response plan | [`06-incident-response-plan.md`](docs/06-incident-response-plan.md) |
| (f) | Service provider oversight | [`07-service-provider-oversight.md`](docs/07-service-provider-oversight.md) |
| (e) | Security awareness & training | [`08-security-awareness-training.md`](docs/08-security-awareness-training.md) |
| (g) | Program review & adjustment | [`09-program-review-adjustment.md`](docs/09-program-review-adjustment.md) |
| (i) | Board / ownership reporting | [`10-board-reporting.md`](docs/10-board-reporting.md) |

## What's Next

- [ ] Close out the safeguards gap-check items currently marked Partial/Missing — tracked as an ongoing 314.4(c) implementation workstream, separate from the completed risk assessment

## Repo Contents

| Path | What it is |
|---|---|
| `README.md` | You're reading it |
| `docs/` | One write-up per 314.4 element: procedures, approach, and why it matters |
| `images/` | Sanitized/blurred screenshots of the real artifacts, organized by topic |

## Disclaimer

This repository documents a real, in-progress compliance methodology for illustrative and portfolio purposes. It is not legal advice, and it is not a template to copy-paste as a substitute for an institution-specific risk assessment. If you're building your own GLBA Safeguards Rule program, consult 16 CFR Part 314 directly and, where needed, qualified legal counsel.
