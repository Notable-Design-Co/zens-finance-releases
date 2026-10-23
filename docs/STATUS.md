# Status

Snapshot of 2026-10-22 (America/Los_Angeles). Rewrite it when things change; don't append.

## What publishes here

The release workflow of the private source repository `zens-finance` (`.github/workflows/release.yml`), once for
each `vX.Y.Z` tag. Nothing else should write here.

## Latest version

- GitHub identifies **v1.1.0** as the latest published release, published 2026-09-29 at 01:10:46 UTC (checked
  2026-10-22 Pacific / 2026-10-23 UTC): <https://github.com/Notable-Design-Co/zens-finance-releases/releases/tag/v1.1.0>.
- Its eight assets are the Windows installer, universal macOS DMG and zip, their three blockmaps, `latest.yml`
  and `latest-mac.yml`. No artifacts or update manifests were changed during this documentation correction.
- Installed versions are unknown. Publication does not establish which computers have updated.

## Update compatibility

Version 1.1.0 names `Notable-Design-Co/zens-finance-releases` and allows release links under both owners. Older
versions use the old owner's feed address and rely on GitHub's redirect. Macs running 1.0.x need to download 1.1.0
manually once; the old macOS link issue is fixed in 1.1.0.

## Next action

No release action here. Source changes do not update published installers; a future release requires separate
permission and follows `zens-finance` `docs/RELEASING.md`. Never delete a published release.
