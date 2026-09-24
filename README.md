# zens-finance-releases

Public download and update channel for the Zen's Finance desktop app: its installers and update manifests for Windows and macOS.

**Status:** maintained · **Owner:** Alec

## What it is and is not

- Each GitHub Release here is one version of Zen's Finance: the Windows installer (NSIS `.exe`), the macOS universal
  DMG and zip, their `.blockmap` files, and the update manifests `latest.yml` and `latest-mac.yml`.
- The app's updater reads this repository. The app's update settings (`electron-builder.yml`, `publish`, in the
  source repository) point at `Notable-Developers/zens-finance-releases`. This repository now lives at
  `Notable-Design-Co/zens-finance-releases`, and GitHub redirects the old address (checked on 2026-09-24 for the
  `latest.yml` download).
- Only the versioned installers and update manifests that the release workflow builds belong here. Never client
  data, statements, reports, logs, tokens or source code. This repository is public.
- The source code is not here. It is in the private repository `zens-finance`.

## Run and test

Nothing to run or test here. The source repository builds each installer, installs it and runs its tests before
anything is uploaded.

## Release and rollback

- **How a release arrives:** a `vX.Y.Z` tag in `zens-finance` starts its release workflow
  (`.github/workflows/release.yml`). The workflow creates a draft release here, uploads exactly the expected files,
  and then publishes the draft as the latest release. The apps never see drafts.
- **Rollback:** never delete a published release, because Windows apps may already have downloaded it. The fix is
  released as the next patch from `zens-finance` (its `docs/RELEASING.md`).
- **Which computers run which version:** Unknown, needs Alec.

## Docs

- [docs/STATUS.md](docs/STATUS.md): what publishes here and the latest version
