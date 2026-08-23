# HS Offline Loot Forge v2.6.0 — Obsidian Forge

This is the Season 10 rebuild of HS Offline Loot Forge.

## Highlights

- New Obsidian Forge interface with a process console, animated Quick Farm showcase, categorized Boost Vault and runtime journal.
- Animated Angelic wings, Unholy spirit claws and Heroic energy wings.
- Verified Season 10 native routes for rarity items, flasks, cards, codex, keys, charms, gems, materials, crafting items, runes and boss gems.
- Native Divine Tarot route restored.
- Boss Gems now use the native Season 10 gem pool rather than a single fixed gem.
- Clear STANDBY/OFF/ON/PARTIAL/MISMATCH feedback and safer one-route-at-a-time workflow.

## Stability and safety

- Runtime-only: `Hero_Siege.exe` on disk is never modified.
- Restore All and app close restore active runtime changes.
- Routes that froze the game, produced no normal-monster drops or remain unverified are absent from the release interface.
- Python bytecode compilation, static Season 10 route tests, packaged callback/state tests and a standalone EXE startup test passed.
- Microsoft Defender custom scan reported no threats for the packaged EXE.

## Upgrade notes

- This is a major upgrade from v1.1.2 and is intended for the current Season 10 build.
- Extract the new ZIP into a fresh folder; do not overwrite a running older version.
- The binary is not code-signed, so Windows SmartScreen may display a warning.
