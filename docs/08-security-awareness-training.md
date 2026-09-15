# Security Awareness & Training — 16 CFR §314.4(e)

[← Back to README](../README.md)

## Requirement

§314.4(e) requires the institution to ensure personnel can actually carry out the Information Security Program, through four sub-elements: (1) general staff security awareness training, (2) qualified information security personnel, (3) ongoing security training for that personnel, and (4) verification that key security personnel maintain current threat knowledge.

## Approach

### General staff training — 314.4(e)(1)

- **Audience:** all personnel with access to student or customer PII
- **Delivery:** a written training handout, with a signed acknowledgment confirming it was read and understood
- **Frequency:** annually, plus at time of hire for any new personnel granted access to student/customer information
- **Content:** drawn directly from risks identified in the [risk register](03-risk-assessment-methodology.md) — training content changes as risks are identified or resolved, instead of being a generic annual slideshow disconnected from what's actually been found

> 📸 **Screenshot placeholder:** `images/training/handout-cover-topics.png`
> A cropped screenshot of the training handout — the cover/topic-list page works well since it shows structure without any completed acknowledgment data. Do not screenshot any signed acknowledgment log — those contain real staff names/signatures.

### Qualified information security personnel — 314.4(e)(2)

For an institution of this size, a single Qualified Individual serving as the dedicated information security personnel is documented as a deliberate, sized-to-fit decision — backed by a recognized industry certification (CompTIA Security+) and ongoing hands-on skill development (see the companion [cybersecurity homelab project](https://github.com/HakeemP210/HakeemP210)) rather than left as an unstated assumption.

### Ongoing training & current threat knowledge — 314.4(e)(3)–(4)

Maintained through a combination of:

- Continuing education tied to the Security+ certification
- Monitoring relevant security advisories (e.g., CISA alerts, vendor security bulletins for systems in the [asset inventory](02-asset-data-inventory.md))
- Independent, hands-on cybersecurity study and lab work

This is documented explicitly as an ongoing activity with sources named, not a one-time certification treated as permanently sufficient.

## Why this matters

A written Information Security Program is only as good as the people executing it day to day. Tying general staff training content directly to the actual risk register — instead of a generic annual compliance video — means training changes as real risks change, and connecting the QI's own certification and hands-on practice to this requirement (rather than treating it as a separate resume line) is what makes 314.4(e)(2)–(4) a documented, defensible answer instead of an assumption.

## Related

- [Risk Assessment Methodology](03-risk-assessment-methodology.md)
- [Incident Response Plan](06-incident-response-plan.md)
