# Profile maintenance automation (design)

Goal: keep GitHub + LinkedIn copy aligned with professional data without manual rewrite every time — while preserving voice, honesty, and human merge control.

```text
Sources (Downloads / exports)
        │
        ▼
   Ingest + normalize     ← skill: .profile/SKILL.md
        │
        ▼
   Voice filter           ← .profile/VOICE.md
        │
        ├─► README.md patch (GitHub)
        └─► LinkedIn draft md (optional)
        │
        ▼
   Open / update PR       ← never auto-merge master
        │
        ▼
   You review client list + claims → merge
```

## Layers

| Layer | What | Where |
|---|---|---|
| **Voice & rules** | Tone, directional pull, don’ts | `.profile/VOICE.md` |
| **Sources** | What files/URLs to read | `.profile/SOURCES.md` |
| **Skill** | Agent procedure for edits | `.profile/SKILL.md` |
| **Examples** | Patterns from other profiles | `.profile/EXAMPLES.md` |
| **Cursor Automation** (optional next) | Schedule or “when PORTFOLIO-PUBLIC changes” → run skill → PR | Cursor Automations editor |
| **GitHub Action** (optional later) | Link check client URLs weekly; fail PR if dead | `.github/workflows/` |

## Recommended v1 (low risk)
1. Keep brag sheet + LinkedIn PDF in known paths (SOURCES.md).
2. Trigger: you say “refresh profile” *or* a monthly Cursor Automation.
3. Agent runs `.profile/SKILL.md`, opens/updates PR on `cursor/profile-*` branch.
4. You merge after client-site pass.

## Recommended v2
- Copy latest `PORTFOLIO-PUBLIC.md` into `.profile/data/PORTFOLIO-PUBLIC.md` (versioned).
- Automation watches that file on push → regenerate README sections marked with HTML comment anchors.
- Separate job: `lychee` or curl link-check on client URLs.

## Scraping note
LinkedIn blocks anonymous scrape (auth wall / HTTP 999). Prefer **manual PDF export** or data download — don’t fight LinkedIn login in CI. GitHub API is fine for repo/README. Client sites: allowlist + link check only.

## Not automated
- Claiming new titles
- Adding client sites without your allowlist edit
- Pushing straight to `master`
