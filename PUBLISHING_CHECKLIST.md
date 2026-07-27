# Publishing Checklist

## 1. Put it on GitHub (~20 min)

1. Create a free account at github.com (if needed), then click **New repository**.
2. Name it `civic-returns` (or similar). Public. Don't initialize with a README.
3. On the new repo page, choose **"uploading an existing file"** and drag in the entire contents of this `civic-returns-publish` folder (README.md at the top level, plus `data/`, `docs/`, `index.html`, `LICENSE.md`).
4. Commit. Your dataset is now published, versioned, and citable.
5. Edit README.md on GitHub to replace `[your-username]` in the citation line.

## 2. Turn on the live explorer (~5 min)

1. In the repo: **Settings → Pages → Source: Deploy from a branch → main → / (root)** → Save.
2. In 1–2 minutes the explorer is live at `https://<username>.github.io/civic-returns/`.
3. Optional later: buy a domain (e.g., civicreturns.org) and add it under Settings → Pages → Custom domain.

## 3. Set up the corrections form (~10 min)

Follow `docs/AIRTABLE_INTAKE_FORM.md`, then paste the form URL into the README, the explorer footer, and your launch post.

## 4. Optional: citable archive

Create a free account at zenodo.org → New upload → attach `data/us_data_centers.csv` + README → publish. You get a DOI; add it to the README citation. Repeat for major versions only.

## 5. Launch post (the part that makes it spread)

Lead with the finding, not the dataset. Suggested angle:

> **America is building $1 trillion of data centers. Communities have enforceable agreements for 0.3% of them.**
> Of 1,185 tracked US data center projects, exactly 4 have a formal community benefits agreement — and none was negotiated with an independent community coalition at the table. The rest of the "community benefits" are discretionary corporate giving, revocable at any time. Explore the map, download the data.

Include: 3–4 headline stats, one map screenshot, the explorer link, the repo link, the corrections form link.

## 6. Send it to the people already working this beat

- **Sabin Center for Climate Change Law** (Columbia) — they maintain the CBA database and wrote the definitive data-center CBA analysis; your dataset extends their work nationally.
- Reporters who covered the specific fights in the data: Cardinal News (VA), Tucson Sentinel/AZ Luminaria (Project Blue), Memphis outlets (xAI), Lancaster Online (PA CBA), Racine County Eye (WI), BG Independent (OH).
- Data Center Dynamics / Data Center Frontier tips lines — "first open dataset of data center community benefits" is a story for them.
- Advocacy orgs: local coalitions named in your opposition column are your most motivated users and contributors.

## 7. Keep it fresh

- The daily audit task keeps improving the workbook. Every week or two: re-export the CSV, regenerate `index.html` (ask Claude — "refresh the publish package from the latest workbook"), and drag the updated files into GitHub.
- Watch the corrections queue; credit contributors.
