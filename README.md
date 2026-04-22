# Void 634 Client w/ RuneLite

Public release channel for the Void Client. It is bundled with RuneLite.

![Release](https://img.shields.io/badge/latest-v0.0.4-6b4a2f)
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
