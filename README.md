# HS Offline Loot Forge

Runtime-only target farming tool for **Hero Siege Season 10 offline play**.

> Current release: **v2.6.3 — Gem Split Fix**
> Part of the [Hero Siege Offline Toolkit](https://github.com/falorfrozen-cmd/hero-siege-offline-toolkit).

![HS Offline Loot Forge v2.6.0](docs/obsidian-forge-v2.6.0.png)

## What changed in v2.6.3

- Split the Season 10 Uncut Jewel and Incarnation Gem routes instead of treating both item families as the same drop.
- **Uncut Jewel** now keeps the native Jewel category and its normal Uncut Jewel results.
- **Incarnation Gems** now uses the separate native green Gem of Incarnation branch.
- Added route-extra verification and rollback so a mismatched branch is restored instead of leaving a partial patch active.
- Kept the v2.6.2 dynamic proxy, EAC diagnostics and module-base compatibility fixes.

## Verified Season 10 features

### Rarity and equipment

- Angelic / SS drops and Angelic Focus
- Unholy Focus
- Heroic Focus
- Satanic Items
- Unique Flasks
- Relics

### Cards, keys and currency

- Tarot Cards and native Divine Tarot
- Codex
- Angelic Keys, normal Keys and Dungeon Keys
- Satanic Dice

### Charms and gems

- Normal, Angelic, Unholy and Satanic/Set Charms
- Uncut Jewels (native Jewel category)
- Incarnation Gems (separate green Gem category)
- Boss Gems, including the native Season 10 gem pool

### Materials and crafting

- Ore Materials and Essence of Chaos
- Random Orbs
- Life / Mana Flasks
- Satanic Crystal
- Blacksmith's Mallet
- Destiny Shard
- Gypsy's Prophecy and Prophet's Wisdom
- Runes and Reflection

## Safety model

- **Offline / single-player only.**
- The tool writes only to the running `Hero_Siege.exe` process.
- The game executable on disk is never modified.
- **Restore All**, closing Loot Forge, or restarting the game restores a clean runtime state.
- Only one target route should be used at a time.
- Boss Parts, standalone Set Charm focus and unverified Heroic Charm focus are intentionally absent.

## Download and use

1. Download the latest ZIP from [Releases](https://github.com/falorfrozen-cmd/Hs-Offline-Loot-Forge/releases/latest).
2. Extract the ZIP.
3. Start Hero Siege using **Launch Without EAC**, then enter offline mode.
4. Run `HSOfflineLootForge.exe` and accept the administrator prompt.
5. Click **Attach / Select**, then choose one Quick Farm profile or Boost Vault route.
6. Use **Restore All** before switching to a different farming target.

See [HSOfflineLootForge_INSTRUCTIONS_EN.txt](HSOfflineLootForge_INSTRUCTIONS_EN.txt) for detailed instructions and troubleshooting.

## Build notes

- Target: Windows 64-bit
- Runtime: standalone PyInstaller build
- Source engine version shown in the title: `v2.6.3-s10-gem-split`
- Release binaries are community builds and are not code-signed, so Windows SmartScreen may display a warning.

## Disclaimer

This project is not affiliated with Hero Siege or Panic Art Studios. Use it at your own risk and keep backups of important offline save files.
