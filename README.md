<p align="center">
  <img src="Useful Information/Blue Print.png" width="800">
  <img src="Useful Information/Grasspin.png" width="800">
  <img src="Useful Information/Saturn.png" width="800">
</p>

<h1 align="center">Blue Print Hardware FPGA Core</h1>

<p align="center">
  Bally/Midway & Jaleco arcade hardware implementation for MiSTer FPGA
</p>

---

## Overview

FPGA implementation of the Bally/Midway arcade hardware platform used by:

- Blue Print (1982)
- Grasspin (1983)
- Saturn (1983)

This core targets MiSTer FPGA and aims for accurate gameplay behavior, video timing, and sound reproduction across all supported titles.

---

## Supported Games

### Blue Print
| Field | Value |
|-------|--------|
| Year | 1982 |
| Publisher | Bally/Midway |
| Genre | Maze / Action |
| Players | 1–2 alternating |

### Grasspin
| Field | Value |
|-------|--------|
| Year | 1983 |
| Publisher | Jaleco |
| Genre | Maze / Action |
| Players | 1–2 alternating |

### Saturn
| Field | Value |
|-------|--------|
| Year | 1983 |
| Publisher | Jaleco / Zilec |
| Genre | Shooter |
| Players | 1–2 alternating |

---

## Controls

Default MiSTer gamepad mapping (may vary slightly per title):

| Input | Action |
|-------|--------|
| D-Pad / Joystick | Move |
| Button A | Primary Action |
| Button B | Secondary Action (if applicable) |
| Select | Insert Coin |
| Start | 1 Player Start |
| Right Shoulder | 2 Player Start |
| Left Shoulder | Pause |

*Note: Specific action behavior depends on the loaded game.*

---

## Features

- Shared hardware implementation for all supported titles
- Arcade-accurate CPU timing
- Sprite priority and layer handling
- High score saving support
- MiSTer-compatible .mra provided
- Verified ROM definitions with checksums

---

## ROM Requirements

ROM files are **not included**.

To use this arcade core, you must provide legally obtained ROM files.

To simplify setup:

- Separate `.mra` files are provided in the **Releases** section for each supported game.
- Each `.mra` specifies required ROM files along with checksums.
- The ROM `.zip` filenames correspond to the naming convention used by the MAME project.

For setup instructions and environment configuration, refer to:

MiSTer Arcade ROM guide:  
https://github.com/MiSTer-devel/Main_MiSTer/wiki/Arcade-Roms

---

## Installation

1. Copy the core `.rbf` file to your MiSTer `/_Arcade/cores` folder.
2. Copy the desired game `.mra` file to your MiSTer `/_Arcade` folder.
3. Place the appropriate ROM `.zip` file(s) in your `/games/mame` directory.
4. Launch from the MiSTer Arcade menu.

---

## Legal Notice

This project contains **no copyrighted game data**.

Users are responsible for obtaining and using ROM files in accordance with applicable laws.

Do not request ROM files in issues or discussions.

---

## Credits

FPGA core development: RodimusFVC  
Original arcade games © Bally/Midway, Jaleco, Zilec