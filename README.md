# Void 634 Client w/ RuneLite

Public release channel for the Void Client. It is bundled with RuneLite.

![Release](https://img.shields.io/badge/latest-v0.1.0-6b4a2f)
![Revision](https://img.shields.io/badge/revision-634-8a6f4d)

## Download

Get the [latest release here](https://github.com/2011Scape/void-client-releases/releases/latest).

## Verify

After downloading both files, verify the jar before running it:

```bash
sha256sum --check void-client-x.jar.sha256
```

## Usage

Run with:

```bash
java -jar runelite-void-client-x.jar --address xxx.xxx.xxx.xxx --port xxxxx
```

## Changelog

<details open>
<summary><strong>0.1.0</strong></summary>

#### RuneLite UI
- Rebuilt the XP tracker panel to closely match RuneLite's original XP tracker.
- Fixed blurry/stretched skill-name rendering in the XP tracker.
- Enlarged skill icons and fixed small icon clipping.
- Added the bundled client/sidebar background image.
- Moved the plugin sidebar open button into the titlebar area next to the window controls.
- Added compact first-run client sizing and persisted window bounds/maximized state.

#### RuneLite API and Events
- Added a broad set of RuneLite API/client event classes for plugin compatibility.
- Added bridge hooks for stat, item, NPC, chat, script, varbit, inventory, projectile, graphics-object, area-sound, and tile-object events.
- Mapped deob zone packets for loc add/delete, map animations, projectiles, area sounds, and ground-item changes.
- Added client loop events including `PostClientTick`, `CanvasSizeChanged`, and `FocusChanged`.

#### Client
- Fixed XP tracker repaint flashing when gaining XP.
- Added support services intended for future RuneLite plugin work.
- Kept the release version aligned with `0.1.0`.

</details>

<details>
<summary><strong>0.0.4</strong></summary>

- Fixed stretched mode on Linux distributions.
- Fixed stretched mode scaling for resizable screen sizing.
- Switched stretched-mode resizable scaling from percentage integer to factor to resolve various rendering bugs.

</details>

<details>
<summary><strong>0.0.3</strong></summary>

#### XP Tracker
- Added skill icons.
- Adjusted progress bar height, spacing, and fill rendering.
- Made XP tracker state persist across restarts.
- Added a reset button.

#### Client
- Fixed sidebar side switching by removing the crash-prone forced redraw.
- Restored launcher options (e.g. `--address` and `--port`).
- Updated brown UI theme to match the 2011 styling.
- Fixed various crashes related to UI layouts and redrawing the client.

</details>

---

*This repository only hosts public release artifacts.*
