# Profile maintenance automation (design)

```text
Work PC / Grok capture
        → michaels-mind Inbox/ (from-work, from-grok)
        → second-brain-ingest (Cursor desk or Cloud)  [librarian]
        → Life/Career canon + wiki
        → maintain-public-profile (Cursor)            [publisher]
        → merimeesoftware README PR (you merge)
```

## Who runs what

| Job | Need it? | Where |
|-----|----------|--------|
| Capture (notes/todos) | Yes | **Grok** + phone/Obsidian + work-PC dump |
| Queue paths only | Optional | GitHub Action already (`queue-inbox.yml`) — no LLM |
| Librarian / wiki compile | **Yes** | **Cursor** (desk session or Cloud Agent) with `second-brain-ingest` |
| Profile publish | Yes | **Cursor** with `.profile/SKILL.md` → PR |
| LLM inside Actions | **No** | Keep out (vault policy) |

Grok is best for **capture** and life-ops todos. Cursor is best for **compile + publish** (repo tools, PRs, skills). Don’t put the librarian primarily in Grok-while-driving or in GitHub Actions.

## Layers

| Layer | Where |
|---|---|
| Voice + brag + allowlist | `michaels-mind` `Life/Career/` |
| Librarian skill | `~/.cursor/skills/second-brain-ingest` |
| Publish skill | `merimeesoftware/.profile/SKILL.md` |
| Profile mirror of voice/sources | `.profile/VOICE.md`, `SOURCES.md` |

## Not automated
- Claiming new titles
- Adding clients off-allowlist
- Pushing straight to `master`
