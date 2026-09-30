# KobeTools fork of Finetune

Upstream: https://github.com/ronitsingh10/FineTune (branch `main`). Built from source with no auto-update. Re-check every row after each upstream sync.

## Fork changes

| Change | Where |
|---|---|
| Sparkle is never started | FineTune/Utilities/UpdateManager.swift (no `updater.start()`) |
| Upstream update feed and signing key removed | FineTune/Info.plist |
| Source build script (ad-hoc, no hardened runtime) | scripts/build-install-local.sh |

## Syncing

Sync to upstream **release tags**, not the tip of `main`. From mactools run `scripts/audit-upstream.sh finetune`, merge only after review, then check every row above.
