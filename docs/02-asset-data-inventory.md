# Asset & Data Inventory — 16 CFR §314.4(b) / NIST CSF ID.AM

[← Back to README](../README.md)

## Requirement

Before you can assess risk, you have to know what you're protecting. §314.4(b) requires the risk assessment to identify and assess reasonably foreseeable risks to customer information — which starts with knowing where that information lives, moves, and rests.

## Approach

Built an inventory of every system that touches student/customer PII, structured around four questions for each one:

| Question | What it captures |
|---|---|
| **What is it?** | System name, vendor, and function (e.g., student information system, financial aid servicing platform, network device) |
| **Where does it live?** | Vendor-hosted / federally hosted / on-premises |
| **What data does it hold or pass through?** | PII category — enrollment records, financial aid data, payment info, etc. |
| **Who's responsible for it?** | Internal owner, or the vendor relationship it falls under |

Systems fall into a few natural buckets:

- **Directly controlled** — on-prem network equipment and staff workstations, where the institution can run its own vulnerability scans and testing directly
- **Vendor-hosted, contracted** — student information system, financial aid servicing/enrollment platforms, loan servicing contact vendors — covered instead under [Service Provider Oversight](07-service-provider-oversight.md)
- **Federally hosted** — U.S. Department of Education systems (e.g., COD, NSLDS, StudentAid.gov / FSA Partner Connect) — out of scope for direct testing, security relies on ED-mandated system requirements
- **State/accreditor-hosted** — state licensing and accreditor portals — same treatment as federally hosted systems

Mapping data flow (where PII *enters*, *moves*, *rests*, and *exits*) on top of this list is what actually feeds the risk analysis — a system holding sensitive data that's also internet-facing and outside the institution's direct control scores very differently than one that's neither.

> 📸 **Screenshot placeholder:** `images/asset-inventory/asset-data-inventory.png`
> A cropped view of the asset/data inventory spreadsheet — 2–3 representative rows with any real vendor/product names and internal system nicknames blurred or replaced with the generic category labels used above (e.g., "Student Information System," "Financial Aid Servicer"). Column headers (System, Hosting, Data Type, Owner) can stay visible.

## Why this matters

This is the "you can't secure what you don't know you have" step, and it's the artifact everything downstream depends on. The risk register (next section) is just this inventory with threats and impact scoring layered on top — skipping or rushing the inventory produces a risk assessment with gaps nobody notices until an incident finds them.

## Related

- [Risk Assessment Methodology](03-risk-assessment-methodology.md)
- [Service Provider Oversight](07-service-provider-oversight.md)
