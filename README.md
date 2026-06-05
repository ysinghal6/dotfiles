# Unified Mnemonic Keymap Guide

This repository contains a unified, mnemonic-based keymap system designed to work identically across custom mechanical keyboards (Keychron K3 Max, Q1 Pro) and the standard MacBook keyboard.

## 1. The Universal Modifiers

To maintain muscle memory, all productivity shortcuts use the same "modifier shape":

| Hardware | Modifier Key |
| :--- | :--- |
| **MacBook Keyboard** | **Option (⌥)** / **Alt** |
| **Custom Keyboards** | **Spacebar** (Hold) |

---

## 2. Cheat Sheet

### Navigation (Arrows & HJKL)
- **Mod + Arrows**: Primary navigation (Works on MacBook and Custom boards)
- **Mod + h / j / k / l**: Secondary Vim-style navigation

### Tmux Productivity
*Mnemonics designed for speed and logic.*
- **Mod + \** or **|**: Vertical Split (Side-by-side)
- **Mod + -**: Split Horizontal (Top-bottom)
- **Mod + z**: **Z**oom Toggle (Zen mode)
- **Mod + x**: **X** (Kill) current pane
- **Mod + c**: **C**reate new window
- **Mod + s**: **S**ession list (choose-tree)
- **Mod + r**: **R**ename current window
- **Mod + [**: **Scroll** / Copy Mode
- **Mod + Space**: Cycle to next layout
- **Mod + 1-9**: Direct window access

### OS Window Management (Rectangle / Magnet)
*Uses **Mod + Shift** to separate OS controls from App controls.*
- **Mod + Shift + f**: **F**ullscreen Toggle (Universal)
- **Mod + Shift + m**: **M**aximize Window
- **Mod + Shift + h**: Snap Window Left
- **Mod + Shift + l**: Snap Window Right

### Browser & Tabs (Chrome / Safari)
- **Mod + [**: Previous Tab
- **Mod + ]**: Next Tab
- **Mod + t**: New Tab
- **Mod + w**: Close Tab

---

## 3. Hardware Implementation

### Custom Keyboards (AL80 / K3 Max / Q1 Pro)
- **Layer Toggle**: The Spacebar acts as a normal Space when tapped, but activates the **Productivity Layer** when held.
- **Space + Q**: Specialized macro to **Lock Mac** instantly.

### MacBook Keyboard
- No software installation (like Karabiner) is strictly required for the MacBook keyboard, as these shortcuts are bound directly to the **Alt/Meta** key in Tmux and Browser settings.

---

## 4. Installation & Sync
- **Tmux**: `cp configs/.tmux.conf ~/.tmux.conf` then `tmux source-file ~/.tmux.conf`.
- **Keyboards**: Load the corresponding `.json` file from the `qmk/` directory into [Keychron Launcher](https://launcher.keychron.com/) or VIA.
