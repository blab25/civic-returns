# Data Dictionary

One row = one data center project. Some large campuses appear as multiple rows (per building or phase) where public records track them separately; a few known duplicate pairs are flagged in notes columns pending consolidation.

## Identification & location

| Column | Definition |
|---|---|
| **Project name** | Public project or facility name. Where no name exists (e.g., permit-level records in Northern Virginia), the street address or permit-holder LLC name is used. |
| **Developer** | Company developing and/or operating the facility. LLC shell names retained where the parent is unconfirmed; parenthetical notes flag known relationships (e.g., "Tallgrass (Project Jade; Crusoe exited Jun 2026)"). |
| **County** | County (or independent city / parish) of the site. |
| **State** | Two-letter USPS code. |
| **Latitude / Longitude** | Decimal degrees (WGS 84). ~96% of rows have coordinates. |

## Status & timeline

| Column | Definition |
|---|---|
| **Status** | One of: `Operational` (energized/serving customers), `Under Construction` (ground physically broken), `Planned` (announced, permitted, or proposed; not yet building), `Cancelled`. Announcement alone does not qualify as Under Construction. |
| **Operating year** | Year the facility came online (Operational) or its publicly stated target year (others). Integer. |

## Scale & investment

| Column | Definition |
|---|---|
| **Power capacity (MW)** | **Confirmed, facility-specific figures only** (numeric). Renewable-energy purchase commitments (PPAs/RECs) are *never* recorded here — those are generation, not facility load. |
| **Est. power capacity (MW)** | Ranges (e.g., "50–100"), campus-wide totals applied to building rows, and design-based inferences (e.g., "~36/bldg" from a confirmed sibling building). Text field. |
| **Power capacity note** | Provenance for the capacity columns: `Confirmed: … (source)`, `Estimate: … (source)`, or `Not disclosed (…)` meaning the figure was researched and no public figure exists. **A blank capacity with a blank note means not yet researched — not zero.** |
| **Building square footage** | Total built or announced square footage for this row's scope. |
| **Land acres** | Site acreage. |
| **CapEx** | Announced capital investment in US dollars (plain integer). Announced/press-release figures; Texas rows may use TDLR construction-cost filings. Campus totals are not duplicated across building rows. |

## Sources

| Column | Definition |
|---|---|
| **Source 1 / 2 / 3** | URLs for the row's core facts (status, scale, investment). |
| **Sources for community benefits** | URLs specifically supporting the community-benefits fields. |

## Community benefits & accountability

| Column | Definition |
|---|---|
| **Key community benefits** | Publicly documented commitments with dollar figures and specifics wherever they exist (grants, funds, infrastructure, water/energy commitments). Entries are tagged by nature: "Discretionary; no formal CBA", "No site-specific community benefits package documented", etc. Distinguishes *delivered/committed* from *pledged-for-the-future*. |
| **Permanent jobs predicted** | Developer/official projection of permanent operational jobs. |
| **Temporary construction jobs predicted** | Peak or total construction jobs projected. |
| **Local hire commitment** | Any documented local-hiring commitment or program. |
| **Workforce programs** | Training/education programs tied to the project (e.g., datacenter academies). |
| **Infrastructure commitments** | Roads, water, grid, or public-facility commitments funded by the developer. |
| **Community opposition** | Documented opposition: lawsuits, petitions, contested hearings, moratorium fights. |
| **Formal CBA?** | Strict `Yes`/`No`. `Yes` requires a signed community benefits agreement meeting **all six criteria**: (1) legally enforceable contract; (2) defined community-side signatory with standing; (3) specific, measurable commitments; (4) governance/reporting/oversight mechanisms; (5) remedies for non-performance; (6) negotiated before approvals were granted. City-signed CBAs qualify; tax abatements, development agreements, MOAs, IRB riders, and voluntary grant programs do not. |

## Audit columns

| Column | Definition |
|---|---|
| **Last audited** | Date (YYYY-MM-DD) the row was last fully verified by the audit process. |
| *(workbook only)* **Change Log sheet** | Every automated fill/correction with date, row, column, old/new values, and source URL. |
