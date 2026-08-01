---
name: maintain-public-profile
description: >-
  Maintain Michael Merimee's public GitHub profile README and LinkedIn drafts.
  Use when updating merimeesoftware/merimeesoftware README, refreshing
  professional positioning, ingesting PORTFOLIO-PUBLIC / LinkedIn PDF / resume,
  or regenerating profile copy with correct voice and FDE directional pull.
---

# Maintain public profile

## Before editing
1. Read `.profile/VOICE.md`, `.profile/SOURCES.md`, and current root `README.md`.
2. Confirm this is a **personal** profile repo — root `README.md` only.
3. Prefer a PR branch over direct `master` pushes.

## Workflow
1. **Ingest** — Read sources in SOURCES.md order. Diff new claims vs current README.
2. **Filter** — Drop internal names, dead client links, overstated titles, lab-metric dumps for GitHub.
3. **Apply voice** — VOICE.md directional pull: DevOps now → FDE/agentic direction; evidence; short.
4. **Edit surfaces**
   - GitHub: root `README.md` (Skills = capabilities; Stack = tools; Elyra featured)
   - LinkedIn drafts: keep under Downloads or `.profile/data/` — don’t dump full resume into GitHub
5. **Verify** — Client URLs still live; no X unless requested; Westfield start May 2024.
6. **Ship** — Commit on a branch / update open PR; summarize what changed for human review.

## Skills section rules
- Lead with **AI & agents**, then platform, then people/communication
- Verb/capability lines, not tool logos
- Every AI claim should be echoable by Elyra or Westfield MCP/agent work

## Automation hooks
- Scheduled or manual agent: ingest Downloads sources → propose README diff → open/update PR
- Never auto-merge to `master`
- Full metric language belongs in PORTFOLIO-PUBLIC / LinkedIn, not forced onto GitHub
