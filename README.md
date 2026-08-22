# Civic Returns: US Data Centers & Community Benefits Dataset

**The first open dataset tracking what US communities actually receive from the data center boom.**

This dataset documents **1,204 US data center projects** across 44 states — their status, power capacity, capital investment, and, uniquely, their **community benefits**: what developers committed to host communities, whether those commitments are enforceable, and where communities fought back.

## Headline findings (August 2026)

- **1,204 projects tracked**: 617 operational, 156 under construction, 407 planned, 24 cancelled
- **$1.40 trillion** in documented capital investment (363 projects with disclosed figures)
- **177.5 GW** of confirmed power capacity across 749 projects. Of the rest: 173 have estimate-only figures, **254 have been researched and have no publicly disclosed capacity at all**, and just 28 remain unresearched — a distinction the explorer lets you filter on
- **1,061 projects** with researched community-benefits documentation
- **Only 4 projects — 0.3% — are covered by a formal, enforceable community benefits agreement**: three data center developments in Lancaster, PA (covered by a single city-negotiated CBA, demonstrating that one municipal agreement can protect multiple projects) and the St. Louis Armory project. Both agreements were signed by city government rather than an independent community coalition
- The dominant model is **discretionary corporate giving**: revocable grant programs, not enforceable commitments

## What counts as a "project" — and why this total differs from industry trackers

**One row = one data center project or campus**, the unit that communities actually negotiate over. Commercial trackers (DatacenterDynamics, datacentermap, DC Byte and similar) generally count **individual buildings, facilities or colocation suites**, so a single campus listed once here may appear five or ten times in their totals. That difference accounts for most of the gap between 1,204 and the larger numbers published elsewhere.

**Included:** hyperscale and campus-scale developments; projects at every stage — operational, under construction, planned and cancelled; any project whose siting, permitting, incentives or community impact are publicly documented.

**Not exhaustively included:** retail colocation suites, enterprise server rooms, small edge and telecom facilities, and individual buildings within a campus that aren't separately documented in public records.

Every row requires a citable public source. This dataset optimises for **community accountability**, not for a complete census of server floorspace: a facility with no public record gives a community nothing to hold anyone to. Where public records do track a campus building-by-building (as in parts of Northern Virginia), those appear as separate rows — see the data dictionary for how granularity is handled.


## What's in this repository

| Path | Contents |
|---|---|
| `data/us_data_centers.csv` | The full dataset (UTF-8 CSV, one row per project/building) |
| `data/us_data_centers.xlsx` | Same data as Excel, including the change-log sheet |
| `index.html` | Interactive explorer (map + charts + filters) — works on GitHub Pages |
| `docs/DATA_DICTIONARY.md` | Definition of every column, including data conventions |
| `docs/METHODOLOGY.md` | Sources, verification process, coverage statistics, limitations |
| `docs/AIRTABLE_INTAKE_FORM.md` | Spec for the community corrections/submissions form |
| `LICENSE.md` | CC BY 4.0 |

## Using the data

The dataset is free to use for any purpose with attribution (CC BY 4.0). Suggested citation:

> Civic Returns, *US Data Centers & Community Benefits Dataset* (2026). https://github.com/[your-username]/civic-returns

Key conventions to understand before analysis (full details in the data dictionary):

- **Power capacity (MW)** contains only confirmed, facility-specific figures. Ranges, campus-wide totals, and inferences live in **Est. power capacity (MW)**, and every researched row carries a **Power capacity note** with its source — including explicit "Not disclosed" notes where a figure was researched and does not publicly exist. Blank ≠ zero; blank means not yet researched.
- **Formal CBA?** applies a strict six-criterion definition (enforceable contract, community-side signatory, specific measurable commitments, governance mechanisms, remedies for non-performance, negotiated before approvals). Tax abatements, development agreements, MOAs, and voluntary grant programs are **No**.
- **CapEx** is announced project investment. Campus-level figures are not repeated across building-level rows of the same campus.

## Updates and corrections

The dataset is updated on a rolling basis (automated daily audit passes; every change is logged with sources in the workbook's Change Log sheet). To submit a correction or report a project or community benefits agreement we missed, use the corrections form (see `docs/AIRTABLE_INTAKE_FORM.md`) or open an issue in this repository.

## Why this exists

Commercial data center trackers serve investors and operators. Nobody was tracking the other side of the ledger: what the communities hosting this trillion-dollar buildout were promised, what they got, and whether any of it is enforceable. This dataset exists to answer that question — for journalists, researchers, advocates, and above all for the local officials and residents negotiating with developers right now, who deserve to know what other communities received.
