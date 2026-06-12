# Astro's Notoriety Tracker — v1.0

A screen-reading tracker for [Notoriety](https://www.roblox.com/games/21532277/Notoriety-A-PAYDAY-Experience) on Roblox. It automatically picks up your timer, cash and XP at the end of each heist so you can track earnings, plan rotations, and manage ECM timers without tabbing out or doing the math yourself.

---

## Download

**[Download the latest release here](https://github.com/notrealdude755/Astro-s-Notoriety-Tracker/releases/tag/1.0_PreRelese)**

> **Windows SmartScreen warning?** That's normal for small indie tools that aren't signed. Just hit **More info → Run anyway** — the full source is right here in the repo if you want to check it yourself.

---

## Getting started

Just grab the EXE from the [Releases](https://github.com/notrealdude755/Astro-s-Notoriety-Tracker/releases/tag/1.0_PreRelese) page, drop it anywhere, and double-click. No install, no setup.

---

## How to use it

The basic loop is simple:

1. Run a heist
2. When it ends, stay on the results screen
3. Hit **Num 0** — the tracker reads your timer, cash and XP automatically
4. Repeat and watch your stats build up

### What's in each tab

| Tab | What it does |
|-----|-------------|
| **Tools → Tracker** | Your main earnings view — per-second and per-minute rates |
| **Tools → Codes** | BB Code and Ozela Code helpers |
| **Tools → ECM Timers** | Track jammer cooldowns for up to 4 players |
| **Calc** | Do the math manually if you prefer |
| **RotSug** | Finds the best heist rotation for your goals |
| **Saves** | Browse and manage your heist history |
| **Settings** | Hotkeys, resolution, extras |

---

## ECM Timers

Tracks jammer cooldowns across your whole crew so nobody has to count in their head.

**Before the heist:**
1. Open **Tools → ECM Timers** (you may need to enable Addons in Settings first)
2. Set how many players are in your crew (1–4)
3. Set each player's skill level — **Maxed** (2 charges x 23.5s) or **No skill** (1 charge x 15s)

**During the heist:**
- **Num 5** starts the first ECM
- Press it again to start the next player's ECM while the current one is still running
- When a charge ends, the next one kicks off automatically — no button needed
- Hit **Reset All** (or the per-player X) to start fresh

The chain goes:
```
P1 C1 → P1 C2 → P2 C1 → P2 C2 → ... → P4 C2 → done
```
Pressing Num 5 early skips anyone already running and jumps to the next available charge.

---

## Hotkeys

| Key | Action |
|-----|--------|
| **Num 0** | Scan screen |
| **Num 1** | Reset session |
| **Num 2** | Quit |
| **Num 3** | Remove last heist from rotation |
| **Num 4** | Mark heist as infinite |
| **Num 5** | Start / advance ECM |
| **Num 6** | Scan override (uses manual input instead) |

Everything can be rebound in **Settings** — any key works.

---

## Supported resolutions

| Resolution | Supported |
|------------|-----------|
| 1920x1080 | Yes |
| 2560x1440 | Yes |

If OCR is reading wrong, double-check your resolution matches what's set in Settings.

---

## Troubleshooting

**Reading wrong numbers or nothing at all**
Make sure Roblox is in fullscreen or windowed fullscreen, and that your resolution in Settings matches your actual screen. If it's still off, just type the values manually in the input fields and press Num 6 to use those instead.

**ECM tab is missing**
Go to **Settings** and turn on **Addons** — that's what shows it.

**EXE won't open / flagged by antivirus**
False positive — this is common with PyInstaller-built tools. Right-click → Properties → check **Unblock** at the bottom, then try again. Or just click through the SmartScreen popup with **More info → Run anyway**.

**Window is too small or too big**
Drag the grip at the bottom to resize vertically, or adjust the UI scale in Settings.

---

## Changelog

### v1.0
- ECM charges now auto-chain on completion across all players
- Can start the next player's ECM before the current one finishes (Num 5 skips running players)
- Rotation suggester improvements
- BB Code and Ozela Code helpers
- Per-player skill toggle (Maxed / No skill)
- Fully customisable hotkeys
- 1920x1080 and 2560x1440 support

---

## Authors

Made by **Astro** and contributors. Full credits are in the **Authors** tab inside the tracker.

---

*Not affiliated with or endorsed by the Notoriety team or Roblox Corporation.*
