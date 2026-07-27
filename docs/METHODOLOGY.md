# Methodology

## Scope

US data center projects — operational, under construction, planned, and cancelled — with an emphasis on hyperscale and campus-scale development and on the **community dimension**: benefits, agreements, opposition, and enforceability. Retail colocation is included but not exhaustively; the dataset does not attempt to enumerate every small colocation suite in every metro.

## Sources

Row-level facts are compiled and cross-checked from:

- **Trade press**: Data Center Dynamics, Data Center Frontier, Data Center Knowledge, and regional business press
- **Tracker databases**: datacentermap.com, baxtel.com, cleanview.co, dcbyte.com, interconnection.fyi, Aterio, Epoch AI
- **Primary/official sources**: company press releases and data center community pages (Meta, Google, Microsoft, AWS local-community sites), state and local government announcements, economic development authorities, Texas TDLR construction filings, SEC filings, county permit records
- **Local journalism**, which is frequently the only source for community benefits, opposition, and agreement details

Source URLs are recorded per row (Source 1–3 and a dedicated community-benefits source column).

## Verification process

The dataset has undergone systematic verification passes (most recently July 2026):

1. **Status audit** — every project marked Planned/Under Construction with a stated operating year at or before the current year was individually re-verified against news and tracker sources; 88 status corrections were applied in the July 2026 pass, including 2 cancellations discovered (Kingsboro NC; DPO Wisconsin Rapids) and a developer exit (Crusoe leaving Wyoming's Project Jade).
2. **Capacity audit** — confirmed figures separated from estimates and from verified "not disclosed" cases (see Data conventions). Renewable-energy commitments were systematically excluded from capacity fields.
3. **Community benefits research** — all hyperscale operators' projects were researched for documented benefits; entries record dollar figures and cite sources, and explicitly distinguish discretionary corporate giving from enforceable agreements. Absence claims ("no package documented") reflect actual research, not missing research.
4. **Formal CBA classification** — every claimed "community benefits agreement" was tested against a strict six-criterion definition (enforceable contract; community-side signatory; specific measurable commitments; governance mechanisms; remedies; negotiated pre-approval). Several widely reported "CBAs" (development agreements, MOAs, IRB riders) were classified No with reasons documented.
5. **Ongoing automated audit** — a daily process re-verifies ~10 rows across all columns, stamps a "Last audited" date, and appends every change with its source to a Change Log sheet.

## Coverage statistics (July 2026)

| Field | Coverage |
|---|---|
| Project name, status, state | 100% |
| Coordinates | 96% |
| Building square footage | ~82% |
| Power capacity — confirmed figure | 57% |
| Power capacity — confirmed + estimate or verified "not disclosed" | 75% |
| Land acres | ~60% |
| Community benefits researched | 54% (100% of hyperscale operators) |
| Operating year | 39% |
| CapEx | 24% |

**Blank cells mean "not yet researched," never "zero" or "none."** Researched absences are recorded explicitly ("Not disclosed", "No site-specific package documented").

## Known limitations

- **Building vs. campus granularity is inconsistent** across sources; some campuses appear as one row, others as several. A few known duplicate pairs are flagged pending consolidation.
- **Operating year and CapEx** skew toward large, newsworthy projects; the colocation long tail is underdocumented (the daily audit is progressively filling it).
- **Community benefits are only as visible as local journalism makes them**; absence of documentation is evidence of non-disclosure, not proof of absence.
- **Capacity estimates** (the Est. column) inherit tracker-site methodology differences; the note column records which source each came from.
- Figures reflect their citation date; the buildout moves fast. The Change Log records when each cell was last touched.

## Corrections

Corrections and additions are welcome — especially from residents and local officials who know their community's agreements firsthand. Submit via the corrections form or a repository issue. Claims require a citable source (news article, government document, or agreement text).
