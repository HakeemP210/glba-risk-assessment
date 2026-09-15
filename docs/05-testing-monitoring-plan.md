# Testing & Monitoring Plan — 16 CFR §314.4(d)

[← Back to README](../README.md)

## Requirement

§314.4(d) requires the institution to regularly monitor and test the effectiveness of its safeguards. The rule gives two paths: continuous monitoring, or — if continuous monitoring isn't in place — annual penetration testing plus vulnerability assessments at least every six months. Whichever path is chosen has to be documented, not just practiced informally.

## Approach

Without continuous monitoring infrastructure in place yet (tracked as its own entry in the risk register), the institution documented the regulatory-floor path as its current approach:

- **Annual penetration testing**
- **Vulnerability assessments** at least every six months

This is written down explicitly as a deliberate choice with a reevaluation trigger, not a default — as logging/monitoring capabilities mature, moving toward continuous monitoring is the documented next step.

### Scope

Testing scope is split by who actually controls the system:

- **In-scope for direct testing** — infrastructure the institution owns and controls outright (network devices, staff workstations). These get scanned and tested directly.
- **Out of scope for direct testing** — vendor-hosted, federally hosted, or state/accreditor-hosted systems. The institution has no authorization to scan or pen-test systems it doesn't own; their security is instead evidenced through vendor assurance documentation, contractual safeguards clauses, or the hosting platform's own mandated security requirements, and tracked in the [asset inventory](02-asset-data-inventory.md) and [service provider oversight](07-service-provider-oversight.md) documentation instead.

This scope split matters enough to call out on its own: running a scanner against a system you don't have authorization to test isn't due diligence, it's a separate problem. Documenting *why* something is out of scope is as important as documenting what's in scope.

> 📸 **Screenshot placeholder:** `images/testing-monitoring/testing-cadence-table.png`
> A cropped screenshot of the testing cadence table (activity / frequency / performed-by / scope columns) from the plan. This section is framework-only, no PII — safe to show close to as-is, just crop out the header/footer with the real institution's contact info.

### Cadence & responsibilities

| Activity | Frequency | Scope |
|---|---|---|
| Vulnerability assessment | At least every 6 months | In-scope network and workstations |
| Penetration test | Annually | In-scope network and workstations |
| Triggered assessment | As needed, on material change | Any system materially changed or affected |

All findings — from the internal testing above — feed back into the [risk register](03-risk-assessment-methodology.md) with an owner, target date, and status, the same as every other finding across the program.

## Why this matters

"We ran a scan once" isn't a testing program — a defined cadence with named responsibility is what turns testing from a one-time event into an ongoing control. Documenting the scope boundary (what's tested directly vs. relied on vendor/federal assurance for) also heads off the most common audit finding in this area: institutions either not testing anything, or testing systems they never had authorization to touch.

## Related

- [Safeguards Gap Analysis](04-safeguards-gap-analysis.md)
- [Service Provider Oversight](07-service-provider-oversight.md)
