# GitHub org migration — goldspireventures

**Status:** Mostly complete (2026-06-26). Active org: **goldspire-global**.

## Done

| Repo | URL |
|------|-----|
| corporate | https://github.com/goldspire-global/corporate |
| livia | https://github.com/goldspire-global/livia |
| veil | https://github.com/goldspire-global/veil |
| launch-stack | https://github.com/goldspire-global/launch-stack |
| triforge | https://github.com/goldspire-global/triforge |
| valrolly-events | https://github.com/goldspire-global/valrolly-events |
| clearboarder | https://github.com/goldspire-global/clearboarder |
| company | https://github.com/goldspire-global/company |
| simi, mulah, atlas, untapped | already on org |

**Deploy:** https://goldspireventures.com → Vercel project `livia-hq/goldspire-corporate` (standalone repo).

## One manual step: rename org

`goldspireventures` GitHub org could not be created via CLI (requires browser org signup). Your existing **goldspire-global** org holds all repos.

To match the brand slug:

1. GitHub → **goldspire-global** → Settings → **Organization profile**
2. **Rename organization** → `goldspireventures` (if the name is available)
3. GitHub auto-redirects old URLs; update `REPO-REGISTRY.yaml` `org:` field after rename

## Local remotes (already updated)

```text
goldspire-corporate   → goldspire-global/corporate
goldspire-launch-stack → goldspire-global/launch-stack
apps/Livia            → goldspire-global/livia
secure-text           → goldspire-global/veil
ClearBoarder          → goldspire-global/clearboarder
the3companies         → goldspire-global/triforge
Valrolly-Events       → goldspire-global/valrolly-events
docs                  → goldspire-global/company
```

## Remaining

- [ ] Org rename `goldspire-global` → `goldspireventures` (optional, manual)
- [ ] Delete `apps/Livia/artifacts/goldspire-corporate` (deprecated copy)
- [ ] Create `utub` repo when the project has code
- [ ] Push any outstanding local commits on livia / veil / simi
