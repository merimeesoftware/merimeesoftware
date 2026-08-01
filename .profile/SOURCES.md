# Professional data sources (ingest order)

Canonical inputs for regenerating GitHub README and LinkedIn drafts. Prefer freshest + most defensible.

| Priority | Source | Path / URL | Use for |
|---|---|---|---|
| 1 | Portfolio brag sheet | `C:\Users\micha\Downloads\PORTFOLIO-PUBLIC.md` (or copy into `.profile/data/` when updated) | Westfield results, competencies, LinkedIn About |
| 2 | LinkedIn export PDF | `C:\Users\micha\Downloads\Profile.pdf` | Current public LinkedIn state / gaps |
| 3 | Resume | `C:\Users\micha\Downloads\Michael_Merimee_Resume.docx` | Pre-Westfield career, education |
| 4 | FDE resume draft | `C:\Users\micha\Downloads\Michael_Merimee_Resume_FDE.md` | Targeted bullets |
| 5 | LinkedIn update pack | `C:\Users\micha\Downloads\Michael_Merimee_LinkedIn_Westfield_Update.md` | Paste-ready LinkedIn |
| 6 | Live GitHub profile README | `README.md` (this repo) | Current public GitHub |
| 7 | Client sites (manual allowlist) | Listed in README “Client delivery” | Only links that still represent the work |

## Facts locked
- Westfield start: **May 2024**
- Account type: **personal** (`merimeesoftware/merimeesoftware`, root `README.md` only)
- Contact: LinkedIn + GitHub (no X unless re-added)

## Ingest rules
1. Never invent metrics; only use claims present in PORTFOLIO-PUBLIC or verified by user.
2. Soften lab metrics for GitHub; keep full metrics for LinkedIn/resume.
3. Drop client links that are dead or no longer look like the shipped work.
4. After ingest, open a PR — do not push straight to `master` without review.
