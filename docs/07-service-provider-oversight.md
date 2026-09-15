# Service Provider Oversight — 16 CFR §314.4(f)

[← Back to README](../README.md)

## Requirement

§314.4(f) requires the institution to oversee any third-party service provider that receives, maintains, processes, or otherwise accesses customer information on its behalf — by (1) taking reasonable steps to select and retain providers capable of maintaining appropriate safeguards, (2) requiring those safeguards by contract, and (3) periodically reassessing providers based on the risk they present.

## Approach

### Scope

The institution's service provider category applies to any contracted third party that handles customer information on its behalf — for this program that means the student information system vendor, the enrollment/lead-processing servicer, and the loan servicing contact vendor. A regulator, an accreditor, and a mass-market consumer product with no negotiable service agreement are each explicitly called out as *out of scope* for this plan (they're addressed elsewhere — regulators/accreditors aren't "acting on the institution's behalf," and the consumer product is tracked as its own item in the risk register pending a planned migration to a managed business-grade plan). Being explicit about what's *not* in scope, and why, is as important as the list of what is.

> 📸 **Screenshot placeholder:** `images/service-provider-oversight/scope-table.png`
> A cropped view of the service provider scope table — replace real vendor names with generic role labels ("Student Information System," "Enrollment Servicer," "Loan Contact Servicer") before screenshotting, or blur the Vendor column entirely and leave only the Role column visible.

### Selecting & retaining providers

Before engaging a new provider, the institution documents a review of available security documentation (e.g., a SOC 2 report or equivalent, where one exists), confirms data handling practices align with applicable federal/state requirements, and considers the provider's known security incident history. For providers already in use before this process existed, that same review is done retroactively as part of the first annual reassessment rather than skipped.

### Requiring safeguards by contract

Each in-scope provider's contract is tracked for whether it contains an adequate safeguards clause, with status logged directly against risk register entries — "not yet confirmed" is a legitimate, honestly-documented status while contracts are being collected and reviewed, same as any other gap in the program.

> 📸 **Screenshot placeholder:** `images/service-provider-oversight/contract-status-table.png`
> A cropped view of the contract safeguards-clause status table. Blur the Vendor column; the Contract Safeguards Clause status and Risk Register ID columns are safe to show.

### Periodic reassessment

Every in-scope provider is reassessed **annually on a fixed calendar schedule**, independent of individual contract renewal dates — deliberately decoupled so reassessment doesn't silently slip because a contract auto-renewed. Each reassessment considers whether safeguards remain adequate for the risk the provider presents, any incidents since the last review, and whether the contractual safeguards clause is still current. Findings go into the risk register with an owner, target date, and status, same as everywhere else.

## Why this matters

A service provider that handles customer information on the institution's behalf is effectively an extension of the institution's own attack surface — GLBA holds the institution accountable for that provider's safeguards, not just its own. A fixed reassessment schedule and an explicit "not yet confirmed" status (instead of silence) are what keep this from becoming a check-the-box exercise done once at contract signing and never revisited.

## Related

- [Asset & Data Inventory](02-asset-data-inventory.md)
- [Testing & Monitoring Plan](05-testing-monitoring-plan.md)
