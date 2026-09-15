# GLBA Safeguards Rule Risk Assessment

![Regulation](https://img.shields.io/badge/regulation-16%20CFR%20314-183A61)
![Framework](https://img.shields.io/badge/framework-NIST%20CSF%202.0-3765A0)
![Sector](https://img.shields.io/badge/sector-Title%20IV%20Higher%20Ed-557C94)
![Status](https://img.shields.io/badge/status-In%20Progress-yellow)

> **A note on what's real here:** the methodology, framework mapping, document structure, and artifacts in this repo come directly from a GLBA Safeguards Rule risk assessment I'm building for the institution I work for. The *institution's identity* doesn't — no institution name, logo, address, or other identifying detail appears anywhere in this repo, and any document screenshots have identifying details and personal names blurred or masked before they go in. The methodology and the work are real; the "who" is deliberately generic.

I handle regulatory compliance for a Title IV institution, and one of my responsibilities is building out our GLBA Safeguards Rule Information Security Program from the ground up — not auditing an existing one, actually building it: the risk assessment, the safeguards, the testing plan, the incident response plan, all of it. I'm packaging the methodology here as I go, both to have a clean public writeup of how a real 314.4 program comes together end to end, and to pair with my [cybersecurity homelab project](https://github.com/HakeemP210/HakeemP210) as hands-on evidence of the practical side of the same skill set.

This is a living project — sections get added and updated as the real assessment progresses.

## Why GLBA + NIST CSF 2.0

The Safeguards Rule (16 CFR §314.4) doesn't mandate a specific framework, but building the program on one anyway makes the whole thing more defensible and more portable: [NIST CSF 2.0](03-risk-assessment-methodology.md)'s six functions (Govern, Identify, Protect, Detect, Respond, Recover) map cleanly onto 314.4's nine sub-elements, so a single crosswalk does double duty — it satisfies the documentation requirement *and* gives the program a structure a reviewer, auditor, or hiring manager will actually recognize.

## Walkthrough

Each 314.4 element gets its own writeup — methodology, how it was approached, and why it matters, with screenshots of the real (sanitized) artifacts as they're finished:

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

*(g) program evaluation/adjustment and (i) board/ownership reporting are ongoing governance activities rather than standalone artifacts — they're referenced throughout the docs above rather than broken out separately.*

## What's Next

- [ ] Finish collecting and reassessing service provider contracts against the safeguards-clause requirement
- [ ] Close out the safeguards gap-check items currently marked Partial/Missing
- [ ] Add the first round of sanitized document screenshots across all sections
- [ ] Draft the annual QI report to ownership once the assessment cycle closes

## Repo Contents

| Path | What it is |
|---|---|
| `README.md` | You're reading it |
| `docs/` | One write-up per 314.4 element — methodology, approach, and why it matters |
| `images/` | Sanitized/blurred screenshots of the real artifacts, organized by topic |

## Disclaimer

This repository documents a real, in-progress compliance methodology for illustrative and portfolio purposes. It is not legal advice, and it is not a template to copy-paste as a substitute for an institution-specific risk assessment. If you're building your own GLBA Safeguards Rule program, consult 16 CFR Part 314 directly and, where needed, qualified legal counsel.
