# Risk Assessment Methodology & NIST CSF 2.0 Crosswalk — 16 CFR §314.4(b)

[← Back to README](../README.md)

## Requirement

§314.4(b) requires a **written** risk assessment that identifies reasonably foreseeable internal and external risks to the security, confidentiality, and integrity of customer information, and assesses the sufficiency of safeguards in place to control those risks.

## Why NIST CSF 2.0

The Safeguards Rule doesn't mandate a specific framework — but building the assessment on a recognized standard rather than an ad hoc checklist does two things at once: it satisfies the documentation requirement with methodology a Department of Education or accreditor reviewer will recognize, and it gives the whole program a consistent, defensible structure instead of nine disconnected documents.

NIST CSF 2.0's six functions (**Govern, Identify, Protect, Detect, Respond, Recover**) map cleanly onto 314.4's structure:

| 314.4 Element | Requirement | CSF 2.0 Function / Category |
|---|---|---|
| (a) | Designate a Qualified Individual | **GOVERN** — GV.RR (Roles, Responsibilities, Authorities) |
| (b) | Conduct a written risk assessment | **IDENTIFY** — ID.RA (Risk Assessment), ID.AM (Asset Management) |
| (c) | Design & implement safeguards | **PROTECT** — PR.AA, PR.DS, PR.PS, PR.AT |
| (d) | Monitor and test safeguards | **DETECT** — DE.CM (Continuous Monitoring), DE.AE (Adverse Event Analysis) |
| (e) | Train staff | **PROTECT** — PR.AT (Awareness & Training) |
| (f) | Oversee service providers | **GOVERN** — GV.SC (Supply Chain Risk Management) |
| (g) | Evaluate and adjust the program | **GOVERN** — GV.OV (Oversight) |
| (h) | Incident response plan | **RESPOND** — RS.MA, RS.CO; **RECOVER** — RC.RP |
| (i) | QI reports to ownership ≥ annually | **GOVERN** — GV.OV, GV.RM (Risk Management Strategy) |

This crosswalk is the single artifact that answers "how does this map to a recognized framework" in one place, and it's the backbone every other document in this repo cites back to.

> 📸 **Screenshot placeholder:** `images/crosswalk-risk-register/compliance-crosswalk.png`
> A cropped view of the 314.4 → NIST CSF 2.0 compliance crosswalk spreadsheet. No PII risk here — this tab is pure framework mapping — but crop out any tab names/file paths that reference the real institution.

## Risk Analysis & Scoring

Following NIST SP 800-30's risk assessment process (identify threat sources → identify vulnerabilities → determine likelihood → determine impact → calculate risk), each entry in the risk register scores **Likelihood × Impact** against defined criteria rather than gut-feel numbers — Impact is tied to concrete outcomes (number of records potentially exposed, whether a breach-notification trigger under GLBA/FERPA/state law would be tripped, realistic fine exposure) so two different people scoring the same risk land in the same place.

Threat sources considered for each asset include: external attacker, malicious or negligent insider, service-provider failure, and physical loss/theft — evaluated against the vulnerabilities identified for that specific system in the [asset inventory](02-asset-data-inventory.md).

Each risk register entry carries:

- A unique ID (e.g., `R-01`, `R-02`, …) referenced by name throughout the other program documents — [Testing & Monitoring](05-testing-monitoring-plan.md), [Incident Response](06-incident-response-plan.md), and [Service Provider Oversight](07-service-provider-oversight.md) all point findings back into this same register instead of keeping separate tracking
- The 314.4 paragraph and CSF category it maps to
- Likelihood, Impact, and resulting risk score/rating
- Current safeguard status, assigned owner, and target remediation date

> 📸 **Screenshot placeholder:** `images/crosswalk-risk-register/risk-register.png`
> A cropped view of the risk register — 3–5 representative rows. Blur any narrative "Description" or "Notes" cells that describe specific systems, vendors, or internal details; the Likelihood/Impact/Score/Status columns and the scoring legend are safe to show as-is.

## Why this matters

A risk register isn't a compliance artifact you fill out once and file away — it's the shared backlog every other part of the program (safeguards gaps, testing findings, incident post-mortems, service provider issues) feeds into and reads from. Centralizing it is what keeps nine separate 314.4 requirements from turning into nine separate, drifting spreadsheets.

## Related

- [Asset & Data Inventory](02-asset-data-inventory.md)
- [Safeguards Gap Analysis](04-safeguards-gap-analysis.md)
