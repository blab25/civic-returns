# Civic Returns: US Data Centers & Community Benefits Dataset

**The first open dataset tracking what US communities actually receive from the data center boom.**

This dataset documents **1,185 US data center projects** across 44 states — their status, power capacity, capital investment, and, uniquely, their **community benefits**: what developers committed to host communities, whether those commitments are enforceable, and where communities fought back.

## Headline findings (July 2026)

- **1,185 projects tracked**: 596 operational, 97 under construction, 486 planned, 6 cancelled
- **$1.04 trillion** in documented capital investment (284 projects with disclosed figures)
- **169.8 GW** of confirmed power capacity (681 projects with confirmed figures; estimates and verified "not disclosed" status tracked separately)
- **641 projects** with researched community-benefits documentation
- **Only 4 projects — 0.3% — have a formal, enforceable community benefits agreement** (CoreWeave/Lancaster PA ×3 and the St. Louis Armory project), and none was negotiated with an independent community-side signatory
- The dominant model is **discretionary corporate giving**: revocable grant programs, not enforceable commitments

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

> Civic Returns, *US Data Centers & Community Benefits Dataset* (2026). https://github.com/[blab25]/civic-returns

Key conventions to understand before analysis (full details in the data dictionary):

- **Power capacity (MW)** contains only confirmed, facility-specific figures. Ranges, campus-wide totals, and inferences live in **Est. power capacity (MW)**, and every researched row carries a **Power capacity note** with its source — including explicit "Not disclosed" notes where a figure was researched and does not publicly exist. Blank ≠ zero; blank means not yet researched.
- **Formal CBA?** applies a strict six-criterion definition (enforceable contract, community-side signatory, specific measurable commitments, governance mechanisms, remedies for non-performance, negotiated before approvals). Tax abatements, development agreements, MOAs, and voluntary grant programs are **No**.
- **CapEx** is announced project investment. Campus-level figures are not repeated across building-level rows of the same campus.

## Updates and corrections

The dataset is updated on a rolling basis (automated daily audit passes; every change is logged with sources in the workbook's Change Log sheet). To submit a correction or report a project or community benefits agreement we missed, use the corrections form (see `docs/AIRTABLE_INTAKE_FORM.md`) or open an issue in this repository.

## Why this exists

Commercial data center trackers serve investors and operators. Nobody was tracking the other side of the ledger: what the communities hosting this trillion-dollar buildout were promised, what they got, and whether any of it is enforceable. This dataset exists to answer that question — for journalists, researchers, advocates, and above all for the local officials and residents negotiating with developers right now, who deserve to know what other communities received.
