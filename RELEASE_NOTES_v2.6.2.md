# HS Offline Loot Forge v2.6.2 — Dynamic Proxy Update

This maintenance release restores compatibility with the current Hero Siege Season 10 executable, including Hero Siege 7.0.2.

## Fixes

- Replaced executable-tail padding with a private runtime proxy page, so normal executable code growth no longer consumes Loot Forge's proxy storage.
- Added PEB-based image-base discovery as a fallback for unavailable module snapshots.
- Added specific EAC/access-denied diagnostics instead of the generic `module base not found` message.
- Updated Boss Gems and Boss Parts signature validation for the current executable layout.
- Added an administrator manifest to the packaged application.

## Safety and verification

- Offline/single-player use only. Launch Hero Siege without EAC.
- `Hero_Siege.exe` on disk is never modified.
- Proxy redirects are restored before the private runtime page is released.
- If a future build no longer matches a verified signature, Loot Forge stops safely instead of writing blindly.
- Static compatibility tests passed for Hero Siege 7.0.0 and 7.0.2.
- Dynamic allocation, write, restore and release were verified in a live Windows process.

## Upgrade

Close older Loot Forge versions, extract `HSOfflineLootForge-v2.6.2.zip` into a fresh folder, launch Hero Siege without EAC, then run the new executable.
