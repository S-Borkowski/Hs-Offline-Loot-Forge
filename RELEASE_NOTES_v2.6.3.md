# HS Offline Loot Forge v2.6.3 — Gem Split Fix

This release corrects the Season 10 Uncut Jewel and Incarnation Gem farming routes.

## Fixes

- Uncut Jewel now keeps the game's native Jewel category and produces normal Uncut Jewels.
- Incarnation Gems now uses the separate native green Gem of Incarnation branch.
- The two routes no longer share the same result path.
- Added route-extra byte verification and rollback. If the current executable does not match the verified layout, Loot Forge restores the attempted changes and reports a mismatch instead of leaving a partial route active.

## Included compatibility work

- Runtime proxy memory is privately allocated instead of using executable padding.
- PEB-based module discovery remains available when normal module enumeration fails.
- EAC/access-denied failures use specific diagnostics.
- The packaged application requests administrator privileges.

## Safety

- Offline/single-player use only. Launch Hero Siege without EAC.
- The game executable on disk is never modified.
- Use Restore All before changing between unrelated farming routes.
- A future unsupported game build is rejected instead of being patched blindly.

## Upgrade

Close older Loot Forge versions, extract `HSOfflineLootForge-v2.6.3.zip` into a fresh folder, launch Hero Siege without EAC, then run the new executable.
