# Safeguards Gap Analysis — 16 CFR §314.4(c)(1)–(8)

[← Back to README](../README.md)

## Requirement

§314.4(c) requires the institution to design and implement safeguards to control the risks identified in the assessment, covering eight specific sub-elements. It doesn't require every sub-element to be fully mature on day one — it requires an honest accounting of where each one stands, and a plan to close what's missing.

## Approach

Each of the eight required safeguard categories gets a straightforward status:

| # | Safeguard Category | Status |
|---|---|---|
| 1 | Access controls | Implemented / Partial / Missing |
| 2 | Data inventory & classification | Implemented / Partial / Missing |
| 3 | Encryption (at rest and in transit) | Implemented / Partial / Missing |
| 4 | Secure application development practices | Implemented / Partial / Missing |
| 5 | Multi-factor authentication | Implemented / Partial / Missing |
| 6 | Secure disposal procedures | Implemented / Partial / Missing |
| 7 | Change management | Implemented / Partial / Missing |
| 8 | Logging & monitoring of authorized user activity | Implemented / Partial / Missing |

Anything short of "Implemented" becomes an entry in the [risk register](03-risk-assessment-methodology.md) with an assigned owner and target date — the gap check itself is a status snapshot; the register is where the actual remediation gets tracked to closure.

> 📸 **Screenshot placeholder:** `images/gap-check/safeguards-gap-check.png`
> A cropped view of the 8-category gap-check spreadsheet, showing the category list and status column. Blur any "Notes" or "Evidence" cells that reference specific tools, vendors, or systems by name.

## Why this matters

This is deliberately the most exposing document in the whole program — it's a written admission of exactly which safeguards are missing or incomplete. That's also exactly why regulators require it: a program that only documents what's already working isn't a risk assessment, it's a highlight reel. An honest gap check, paired with a dated remediation plan in the risk register, is what a real Information Security Program actually looks like in progress.

## Related

- [Risk Assessment Methodology](03-risk-assessment-methodology.md)
- [Testing & Monitoring Plan](05-testing-monitoring-plan.md)
