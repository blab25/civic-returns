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
4. **Formal CBA classification** — every claimed "community benefits agreement" was tested against a strict six-criterion definition (enforceable contract; community-side signatory; specific measurable commitments; governance mechanisms; remedies; negotiated pre-approval). Several widely reported "CBAs" (development agreements, MOAs, IRB riders) were classified No with reasons documented. **Counting convention:** the `Formal CBA?` flag is applied per project, consistent with the dataset's unit of analysis (one row = one project). The four `Yes` projects derive from two agreement documents: the City of Lancaster, PA CBA covers three data center developments across two campuses, and the St. Louis Armory CBA covers one. Headline figures therefore report **4 covered projects**; anyone counting distinct agreement documents should report 2. Both readings are supported by the source column, which links the underlying agreement for each row.
5. **Ongoing automated audit** — a daily process re-verifies ~20 rows across all columns, stamps a "Last audited" date, and appends every change with its source to a Change Log sheet. As of this publish (Aug 7, 2026), the audit has processed 241 of 1,187 rows since the workbook's "Last audited" column was introduced.

## Coverage statistics (August 2026, n = 1,187 projects)

| Field | Coverage |
|---|---|
| Project name, status, state | 100% |
| Coordinates | 96% |
| Building square footage | ~82% |
| Power capacity — confirmed figure | 60% (714 projects) |
| Power capacity — estimate only | 10% (121) |
| Power capacity — researched, **not published by operator** | 18% (215) |
| Power capacity — not yet researched | 12% (137) |
| Land acres | ~61% |
| Community benefits researched | 63% (100% of hyperscale operators) |
| Operating year | 43% |
| CapEx | 25% |

**Capacity disclosure is itself a finding.** Of the 473 projects without a confirmed megawatt figure, 215 have been researched and simply have no publicly disclosed capacity — the operator has never published one — and 121 have only a range or campus-level figure. The explorer lets users filter on these four states directly.

**Blank cells mean "not yet researched," never "zero" or "none."** Researched absences are recorded explicitly ("Not disclosed", "No site-specific package documented").

## Known limitations

- **Building vs. campus granularity is inconsistent** across sources; some campuses appear as one row, others as several. A few known duplicate pairs are flagged pending consolidation.
- **Operating year and CapEx** skew toward large, newsworthy projects; the colocation long tail is underdocumented (the daily audit is progressively filling it).
- **Community benefits are only as visible as local journalism makes them**; absence of documentation is evidence of non-disclosure, not proof of absence.
- **Capacity estimates** (the Est. column) inherit tracker-site methodology differences; the note column records which source each came from.
- Figures reflect their citation date; the buildout moves fast. The Change Log records when each cell was last touched.

## Corrections

Corrections and additions are welcome — especially from residents and local officials who know their community's agreements firsthand. Submit via the corrections form or a repository issue. Claims require a citable source (news article, government document, or agreement text).
