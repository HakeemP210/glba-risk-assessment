# Incident Response Plan — 16 CFR §314.4(h)

[← Back to README](../README.md)

## Requirement

§314.4(h) requires a written incident response plan covering seven specific elements: goals, an internal response process, defined roles/responsibilities/decision-making authority, an internal and external communications plan, remediation of identified weaknesses, documentation and reporting, and post-incident evaluation and revision of the plan itself.

## Approach

### Five-phase internal response process

```
1. Detect & Report → 2. Assess & Contain → 3. Eradicate → 4. Recover → 5. Post-Incident Review
```

Every phase has a named owner and a plain description of what actually happens in it — not just a diagram. Staff are trained (see [Security Awareness Training](08-security-awareness-training.md)) to report anything suspicious immediately rather than attempt to resolve it themselves; the Qualified Individual leads assessment, containment, and eradication with standing authority to take immediate technical action (disabling accounts, isolating devices) without needing prior sign-off when it's needed to limit harm.

### Roles & decision authority

| Role | Responsibility |
|---|---|
| All staff | Report any suspected event immediately — not expected to resolve anything on their own |
| Qualified Individual | Leads response: assesses severity, directs containment/eradication, has standing authority for immediate technical action |
| Ownership/Director | Notified of any confirmed event; makes decisions requiring executive authority — external communications, legal counsel, law enforcement, material financial/operational decisions |

### Communications

Internal: the QI notifies ownership as soon as a suspected event is confirmed as an incident, with status updates through resolution.

External notification obligations are genuinely layered for a Title IV institution and worth documenting explicitly rather than leaving implicit:

- **State breach notification law** — triggered if sensitive personal information is compromised, with a "without unreasonable delay" standard and a hard deadline (and Attorney General notification) once the number of affected state residents crosses a statutory threshold
- **U.S. Department of Education** — Title IV participants are required to report cybersecurity incidents affecting Title IV data through Federal Student Aid's incident reporting channel
- **Affected service providers** — if the incident involves systems or data they hold on the institution's behalf
- **Law enforcement** — if criminal activity is suspected

> These obligations under GLBA, FERPA, state law, and Title IV can overlap in ways that genuinely need legal counsel before external notification — the plan says so explicitly rather than pretending it's a solved problem. The current FSA incident-reporting procedure and contact are confirmed and kept on file *before* an incident, not looked up during one.

> 📸 **Screenshot placeholder:** `images/incident-response/five-phase-diagram.png`
> The five-phase response process diagram/table and the roles & responsibilities table. No PII in this section — safe to show close to as-is, crop out header/footer institution contact info.

### Remediation, documentation, and revision

Every control weakness identified during or after an incident gets logged into the same [risk register](03-risk-assessment-methodology.md) used everywhere else in the program, with an owner, target date, and status — no separate incident-only tracking system. A blank incident log template (date/time discovered, reported by, description, systems affected, containment actions, root cause, parties notified, resolution, risk register entry created) is attached to the plan so any staff member reporting an event fills in the same structured fields every time.

The plan itself gets reviewed within 15 business days of any incident's resolution, and at least annually independent of whether an incident occurred.

> 📸 **Screenshot placeholder:** `images/incident-response/incident-log-template.png`
> The blank incident log template — this is safe to show in full since it's an empty form with no real incident data in it.

## Why this matters

A plan that only exists on paper fails the first time it's actually needed. Naming who has authority to act *before* an incident (not during one), pre-confirming the actual reporting channels and deadlines, and routing every finding back into the same risk register the rest of the program uses is what makes an incident response plan operational instead of decorative.

## Related

- [Risk Assessment Methodology](03-risk-assessment-methodology.md)
- [Security Awareness Training](08-security-awareness-training.md)
