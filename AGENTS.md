# zens-finance-releases: rules for AI agents

## Read first

- `docs/STATUS.md`
- `README.md`
- In the private source repository `zens-finance`: `docs/RELEASING.md` and `.github/workflows/release.yml`.

## Commands

None. There is no code, build or test here. To see what is published:

```bash
gh release list --repo Notable-Design-Co/zens-finance-releases
```

## Rules

- This repository is public. Nothing private goes in: no client data, statements, reports, logs, tokens, keys or
  source code. (zens-finance `docs/RELEASING.md`)
- Don't rename or move this repository. Installed apps find their updates through its name
  (zens-finance `electron-builder.yml`, `publish`). It already moved once, from `Notable-Developers` to
  `Notable-Design-Co`, and the apps now depend on GitHub's redirect.
- Releases come from the zens-finance release workflow (`.github/workflows/release.yml`, on a `vX.Y.Z` tag). A release
  holds only the installer, the DMG, the zip, their blockmaps, `latest.yml` and `latest-mac.yml`. Any manual step,
  such as deleting a failed draft, follows zens-finance `docs/RELEASING.md`.
- Never delete a published release. Release the next patch instead. (zens-finance `docs/RELEASING.md`)

## Repository conventions

- Start by reading docs/STATUS.md. Before you stop, update it: rewrite what changed, don't append.
- Don't create handoff, brief, plan, report or dated files. State goes in docs/STATUS.md,
  decisions in docs/decisions/, lasting reference in one docs/<TOPIC>.md per topic.
- docs/archive/ is history. Never act on it.
- One change per branch, through a pull request with CI green. Delete the branch after merge.
- No secrets, prices or client personal data in the repository.
- Full standard: notable-site-ops/standards/engineering.md
