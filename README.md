# HS Offline Loot Forge

Runtime-only target farming tool for **Hero Siege Season 10 offline play**.

> Current release: **v2.6.0 — Obsidian Forge**
> Part of the [Hero Siege Offline Toolkit](https://github.com/falorfrozen-cmd/hero-siege-offline-toolkit).

![HS Offline Loot Forge v2.6.0](docs/obsidian-forge-v2.6.0.png)

## What changed in v2.6.0

- Rebuilt the interface as the **Obsidian Forge**.
- Added animated Angelic wings, Unholy spirit claws and Heroic energy wings.
- Grouped verified boosts into Rarity & Focus, Cards & Keys, Charms & Gems, and Materials & Crafting.
- Replaced noisy pre-attach warnings with a restrained `STANDBY` state.
- Added clear symbols and colors for OFF, ON, PARTIAL, STANDBY and MISMATCH states.
- Restored and live-tested the Season 10 native drop engine routes.
- Kept unsafe, freezing or unverified routes out of the release interface.

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
- Uncut Jewels
- Gems
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
3. Start Hero Siege in offline mode.
4. Run `HSOfflineLootForge.exe` as administrator if the game is also elevated.
5. Click **Attach / Select**, then choose one Quick Farm profile or Boost Vault route.
6. Use **Restore All** before switching to a different farming target.

See [HSOfflineLootForge_INSTRUCTIONS_EN.txt](HSOfflineLootForge_INSTRUCTIONS_EN.txt) for detailed instructions and troubleshooting.

## Build notes

- Target: Windows 64-bit
- Runtime: standalone PyInstaller build
- Source engine version shown in the title: `v2.6.0-s10-obsidian-forge`
- Release binaries are community builds and are not code-signed, so Windows SmartScreen may display a warning.

## Disclaimer

This project is not affiliated with Hero Siege or Panic Art Studios. Use it at your own risk and keep backups of important offline save files.
