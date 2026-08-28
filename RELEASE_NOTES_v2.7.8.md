# HS Offline Loot Forge v2.7.8 — Maledict & Mythic Jewels

Season 10 changed the game's internals, and several jewel features stopped doing what
their names said. This release fixes them and adds two new jewel options.

## New

**Maledict Uncut Jewel**
Farm Uncut Jewels that actually roll the **Maledict** prefix.

Before, this route asked the game for the wrong prefix. You got tier S jewels, but almost
never a Maledict one. It now asks for the right prefix, so Maledict jewels really drop.

A second problem is fixed with it: only the **name and tier** used to become Maledict while
the stats still came from the wrong prefix — which is why the jewel did not grant its skill.
The stats now come from Maledict too.

**Uncut Jewel → Mythic (purple)**
Makes Uncut Jewels drop **purple (Mythic)** instead of blue.

This is not just a colour change. The jewel's real rarity is changed, so its name and its
stat roll change with it.

**Suffix Tier → S**
Every suffix rolls the top tier (Tier S) instead of a random one.

**Jewel routes now switch purple on for you**
Turn on *Uncut Jewels* or *Maledict Uncut Jewel* and the Mythic (purple) option comes on
automatically. Turn the route off and it goes back off. No second button to remember.

## Fixes

- **"MISMATCH" on the Mythic button is gone.** Once you switched the option on, Loot Forge
  could no longer find that spot in the game and showed a red MISMATCH, even though nothing
  was wrong. It now recognises the option in both states.
- **Works across more Hero Siege builds.** Loot Forge searches the running game for the
  places it needs instead of relying on fixed numbers that move every time the game updates.
- **Dead options removed.** A few tier options were pointing at code that no longer exists in
  Season 10. They did nothing, so they are gone.

## Other

- The whole application, including every log line, is now in English.

## Still being tested

The Mythic (purple) option and the Maledict stat fix are new in this release. They have
been checked against the game's code but not yet through long play sessions. If something
looks wrong, use **Restore All** and please report it.

## Safety

- **Offline / single-player only.** Start Hero Siege with *Launch Without EAC*.
- The game file on your disk is never touched — changes live only in the running game and
  disappear when you close it.
- Use **Restore All** before switching to a different farming target.
- If your Hero Siege build is not recognised, the option is shown as MISMATCH and is **not**
  applied, rather than patching something blindly.

## Upgrade

Close any older Loot Forge, extract the new ZIP into a fresh folder, start Hero Siege
without EAC, then run `HSOfflineLootForge.exe`.
