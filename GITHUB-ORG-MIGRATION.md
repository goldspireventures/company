# GitHub org migration — goldspireventures

Move active repos under **https://github.com/goldspireventures**.

## 1. Create the org

1. GitHub → **Settings** → **Organizations** → **New organization**
2. Name: `goldspireventures`
3. Plan: Free is fine until you need private collaborators at scale

## 2. Push order (highest leverage first)

| Priority | Local path | Target repo |
|----------|------------|-------------|
| 1 | `goldspire-corporate` | `corporate` |
| 2 | `goldspire-launch-stack` | `launch-stack` |
| 3 | `apps/Livia` | `livia` |
| 4 | `secure-text` | `veil` |
| 5 | `the3companies` | `triforge` |
| 6 | `SIMI` | `simi` |
| 7 | `Valrolly-Events` | `valrolly-events` |
| 8 | Others per `REPO-REGISTRY.yaml` | … |

### Per-repo commands (example: corporate)

```powershell
cd "c:\Users\eamon\Personal Projects\goldspire-corporate"
git init
git add .
git commit -m "Initial commit: Goldspire Ventures corporate site"
gh repo create goldspireventures/corporate --private --source=. --remote=origin --push
```

Repeat with `--private` or `--public` per repo sensitivity. Corporate + marketing sites are often public; `launch-stack` and `livia` usually private.

## 3. Update local remotes (existing repos)

```powershell
git remote set-url origin https://github.com/goldspireventures/REPO_NAME.git
git push -u origin main
```

## 4. Post-migration cleanup

- [ ] Point Vercel `goldspireventures.com` at `goldspireventures/corporate`
- [ ] Remove `apps/Livia/artifacts/goldspire-corporate` after deploy cutover
- [ ] Update Cursor workspace files with new clone paths
- [ ] Update Console Lab venture rows with `repoUrl` → new GitHub URLs
- [ ] Add org README linking to goldspireventures.com

## 5. Naming conventions

- Repo names: lowercase, hyphenated (`launch-stack`, `valrolly-events`)
- Product code names can differ (`secure-text` → repo `veil`)
- One repo per deployable product or factory; no Personal Projects mega-repo
