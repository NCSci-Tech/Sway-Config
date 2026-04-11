# Sway Configuration

A clean and functional configuration for the [Sway](https://swaywm.org) Wayland compositor.

---

## Features

- **Vim-style navigation** (`$mod + h/j/k/l`)
- **Custom keybindings** for launching apps, resizing, and window movement  
- **Automatic idle & lock screen** handling via `swayidle` + `swaylock`
- **System controls** for volume, brightness, and screenshots
- **Touchpad and keyboard tweaks** (natural scroll, tapping, etc.)
- **Simple status bar** with date/time display
- **Dark minimal aesthetic**

---

## Requirements

Make sure these tools are installed:

- `sway`
- `swaylock`
- `swayidle`
- `foot` (terminal)
- `wofi` (app launcher)
- `mako` (notifications)
- `pamixer`, `brightnessctl`, `grim`, `slurp`, `wl-copy`

---

Keybindings Overview
Action	Shortcut
Launch terminal	<kbd>Mod</kbd> + <kbd>Enter</kbd>
Launch menu	<kbd>Mod</kbd> + <kbd>d</kbd>
Kill window	<kbd>Mod</kbd> + <kbd>Shift</kbd> + <kbd>q</kbd>
Focus move	<kbd>Mod</kbd> + <kbd>h/j/k/l</kbd>
Move window	<kbd>Mod</kbd> + <kbd>Shift</kbd> + <kbd>h/j/k/l</kbd>
Resize mode	<kbd>Mod</kbd> + <kbd>r</kbd>
Lock screen	<kbd>Mod</kbd> + <kbd>Shift</kbd> + <kbd>x</kbd>
Screenshot	<kbd>Print</kbd> / <kbd>Shift</kbd>+<kbd>Print</kbd>
Exit Sway	<kbd>Mod</kbd> + <kbd>Shift</kbd> + <kbd>e</kbd>

## Notes

The $mod key is set to the Super (Windows) key.

Adjust colors, keybindings, and preferred apps to fit your workflow.

For full configuration reference, see:

      man 5 sway
