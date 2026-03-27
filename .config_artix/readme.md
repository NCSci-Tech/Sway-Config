# Artix Sway Setup

Artix Linux with OpenRC, Sway WM, and a minimal black terminal aesthetic.

---

## File Structure

```
~/.config/
├── sway/
│   └── config            # Sway WM config
├── waybar/
│   ├── config            # Waybar modules
│   └── style.css         # Waybar theme
└── alacritty/
    └── alacritty.toml    # Terminal config

```

---

## Keybindings

| Key | Action |
|-----|--------|
| `Mod+Return` | Open terminal |
| `Mod+d` | App launcher (wofi) |
| `Mod+Shift+q` | Close window |
| `Mod+Shift+c` | Reload sway config |
| `Mod+Shift+e` | Exit sway |
| `Mod+Shift+x` | Lock screen |
| `Mod+f` | Fullscreen |
| `Mod+Shift+Space` | Toggle floating |
| `Mod+r` | Resize mode |
| `Mod+b` | Split horizontal |
| `Mod+v` | Split vertical |
| `Mod+1-5` | Switch workspace |
| `Mod+Shift+1-5` | Move window to workspace |
| `Mod+Shift+-` | Send to scratchpad |
| `Mod+-` | Show scratchpad |
| `Print` | Screenshot (full) |
| `Shift+Print` | Screenshot (select area) |
| `Ctrl+Print` | Screenshot to clipboard |

Focus and move with `Mod+h/j/k/l` (vim keys).

---

## Workspaces

| Workspace | Purpose |
|-----------|---------|
| 1:term | Terminal |
| 2:web | Browser |
| 3:code | Editor |
| 4:media | Media |
| 5:misc | Misc |

---

## Waybar Modules

| Module | Color | Info |
|--------|-------|------|
| Network | Pink | WiFi SSID via ConnMan |
| CPU | Red | Usage % |
| Memory | Green | Usage % |
| Battery | Yellow | Capacity + status |
| Volume | Cyan | PulseAudio sink volume |
| Clock | Purple | Date + time |

---

---

## Notes

- Wifi is managed by **ConnMan** only — do not enable `net.wlan0` or `wpa_supplicant` as separate OpenRC services or they will conflict
- User configs in `~/.config/` always override system configs in `/etc/xdg/`
- Sway reload (`Mod+Shift+c`) restarts Waybar automatically
- Lock screen activates after 5 min idle, display off after 10 min
