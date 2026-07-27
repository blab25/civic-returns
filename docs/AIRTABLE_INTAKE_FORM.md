# Community Corrections & Submissions Form (Airtable spec)

Purpose: a friendly front door for non-technical contributors — residents, local officials, journalists — to submit corrections, missing projects, and community benefits agreements. Airtable is used **only as an intake queue**; the canonical dataset lives in this repository. (~10 minutes to set up; free tier is fine for intake volume.)

## Base structure

One base, one table: **Submissions**.

| Field | Type | Options / notes |
|---|---|---|
| Submission type | Single select | `Correction to existing entry` / `Missing data center` / `Community benefits info` / `Community benefits agreement (CBA)` / `Opposition or dispute` / `Other` |
| Project name | Single line text | As it appears in the dataset, if known |
| County & State | Single line text | |
| What should change / be added | Long text | The substance of the submission |
| Source link | URL | **Required** — news article, government document, or agreement text |
| Second source (optional) | URL | |
| Your relationship to this project | Single select | `Resident` / `Local official` / `Journalist` / `Researcher` / `Industry` / `Other` — context, not gatekeeping |
| Contact email (optional) | Email | Only if they want follow-up |
| Status | Single select | `New` / `Reviewing` / `Accepted` / `Rejected` / `Needs source` — **not on the form**; internal triage field |
| Reviewer notes | Long text | Internal |
| Date received | Created time | Automatic |

## Form settings

- Share → Form view; include all fields except Status, Reviewer notes, Date received.
- Required: Submission type, What should change, Source link.
- Form title: **"Improve the Civic Returns data center dataset"**
- Description: *"Spotted an error? Know about a data center or a community benefits agreement we missed? Submissions with a citable source (news article, government document, or agreement text) are reviewed and, if verified, added with credit. Community members and local officials especially welcome."*

## Triage workflow

1. New submissions arrive as `New`; review weekly (or whenever notified — enable Airtable email notifications on form submission).
2. Verify against the source provided. No source → mark `Needs source` and reply if contact given.
3. Accepted items: apply to the workbook (or hand to the daily audit task), log in the Change Log sheet with the submitted source, mark `Accepted`.
4. Periodically thank/credit contributors (with permission) in release notes.

## Link placement

Put the form URL in three places: the repository README ("Submit a correction"), the explorer footer, and any launch post.
