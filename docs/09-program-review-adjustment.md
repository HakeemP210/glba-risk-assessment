# Program Review & Adjustment — 16 CFR §314.4(g)

[← Back to README](../README.md)

## Requirement

§314.4(g) requires the institution to evaluate and adjust its Information Security Program in light of testing/monitoring results, material changes to operations or business arrangements, new risk assessment findings, or any other circumstance that may have a material impact on the program. It's the requirement that turns everything else in this repo from a set of documents produced once into a program that's actually maintained.

## Approach

The program gets reviewed on two tracks:

- **Scheduled** — a full review of every document in this repo at least annually, timed to precede the board report (see [Board Reporting](10-board-reporting.md))
- **Triggered** — an immediate review of the affected document(s) whenever a specific event occurs: a testing/monitoring result, a security incident, a material operational or vendor change, a new or re-scored risk finding, or any other circumstance the Qualified Individual has reason to know may matter

Every review — scheduled or triggered — gets logged in a running **Program Change Log**: date, trigger, what changed, which documents were affected. The point of the log isn't bureaucratic box-checking — it's what lets anyone (an auditor, a reviewer, a future version of me) verify that "the program gets reviewed and adjusted" is an actual practice and not just a sentence in a policy document.

> 📸 **Screenshot placeholder:** `images/program-review/change-log.png`
> A cropped view of the Program Change Log spreadsheet — the Date, Trigger Category, and Documents Affected columns are safe to show as-is; blur the "What Changed" narrative cells if they reference anything institution-specific beyond what's already described generically in this repo.

### This isn't theoretical — see the incident response writeup

The clearest example of a triggered review in this program is documented in detail in [Incident Response Plan](06-incident-response-plan.md#its-been-tested-once-for-real): a real security incident, surfaced partway through a scheduled annual review, resulted in a new risk register entry, two existing risk ratings raised to reflect confirmed real-world precedent, a correction to that year's board report, and a confirmed update to the plan's external reporting contact — all in the same review cycle, all logged.

## Why this matters

A risk assessment that gets written once and never revisited is a snapshot, not a program — and it ages out of relevance the moment anything changes, which for a real institution is constantly (new vendors, new systems, staff turnover, an actual incident). Naming the specific triggers in advance, rather than leaving "review the program periodically" as a vague aspiration, is what makes this requirement checkable: either a real event happened and the log shows a corresponding review, or it didn't.

## Related

- [Risk Assessment Methodology](03-risk-assessment-methodology.md)
- [Incident Response Plan](06-incident-response-plan.md)
- [Board Reporting](10-board-reporting.md)
