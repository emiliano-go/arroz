# Titan

> "Rice" in Spanish is "arroz". This is my rice ("arroz" in Spanish).

Two themes with cool sci-fi accents for Hyprland, Quickshell, opencode, VS Code, and PyCharm:

- **Titan Black** — Vanta Black-based dark theme, inspired by deep space imagery: near-black backgrounds with teal/cyan ambient glow and warm highlights.
- **Titan Light** — daylight counterpart with soft grey surfaces and the same teal accent.

![wallpaper](screenshots/wallpaper.jpg)

## Apps

| App | Directory | Install |
|-----|-----------|---------|
| **Hyprland** | `hyprland/themes/titan-black/`, `hyprland/themes/titan-light/` | Copy wallpaper to `~/.config/hypr/wallpapers/` and add colors to `hyprland.conf` (see below) |
| **opencode** | `opencode/themes/` | Copy `titan-black.json` to `~/.config/opencode/themes/` and set `"theme": "titan-black"` in `tui.json` |
| **VS Code** | `vscode-titan-black/` | `code --install-extension vscode-titan-black/titan-black.vsix` |
| **PyCharm** | `pycharm/titan-black.jar` | Settings → Plugins → Install Plugin from Disk → select `titan-black.jar` |
| **Quickshell** | `quickshell/` | Copy config and plugins (see below) |

## Color Palette

### Titan Black

| Role | Hex | |
|------|-----|-|
| Background | `#050508` | ![#050508](https://via.placeholder.com/15/050508/050508.png) |
| Dark BG | `#080810` | ![#080810](https://via.placeholder.com/15/080810/080810.png) |
| Selection | `#1a1a2a` | ![#1a1a2a](https://via.placeholder.com/15/1a1a2a/1a1a2a.png) |
| Muted | `#454555` | ![#454555](https://via.placeholder.com/15/454555/454555.png) |
| Foreground | `#c8c8d4` | ![#c8c8d4](https://via.placeholder.com/15/c8c8d4/c8c8d4.png) |
| Accent (teal) | `#5a9ebf` | ![#5a9ebf](https://via.placeholder.com/15/5a9ebf/5a9ebf.png) |
| Cyan | `#6ab0c8` | ![#6ab0c8](https://via.placeholder.com/15/6ab0c8/6ab0c8.png) |
| Green | `#60a080` | ![#60a080](https://via.placeholder.com/15/60a080/60a080.png) |
| Red | `#c05050` | ![#c05050](https://via.placeholder.com/15/c05050/c05050.png) |
| Orange | `#b87848` | ![#b87848](https://via.placeholder.com/15/b87848/b87848.png) |
| Yellow | `#c0b878` | ![#c0b878](https://via.placeholder.com/15/c0b878/c0b878.png) |
| Purple | `#8070a0` | ![#8070a0](https://via.placeholder.com/15/8070a0/8070a0.png) |

### Titan Light

| Role | Hex | |
|------|-----|-|
| Background | `#f4f5f7` | ![#f4f5f7](https://via.placeholder.com/15/f4f5f7/f4f5f7.png) |
| Dark BG | `#e9eaef` | ![#e9eaef](https://via.placeholder.com/15/e9eaef/e9eaef.png) |
| Selection | `#d7dce6` | ![#d7dce6](https://via.placeholder.com/15/d7dce6/d7dce6.png) |
| Muted | `#8a8a99` | ![#8a8a99](https://via.placeholder.com/15/8a8a99/8a8a99.png) |
| Foreground | `#23232e` | ![#23232e](https://via.placeholder.com/15/23232e/23232e.png) |
| Accent (teal) | `#5a9ebf` | ![#5a9ebf](https://via.placeholder.com/15/5a9ebf/5a9ebf.png) |
| Cyan | `#2f8aa0` | ![#2f8aa0](https://via.placeholder.com/15/2f8aa0/2f8aa0.png) |
| Green | `#4f8a6a` | ![#4f8a6a](https://via.placeholder.com/15/4f8a6a/4f8a6a.png) |
| Red | `#b04040` | ![#b04040](https://via.placeholder.com/15/b04040/b04040.png) |
| Orange | `#a05f2c` | ![#a05f2c](https://via.placeholder.com/15/a05f2c/a05f2c.png) |
| Yellow | `#9a8a3a` | ![#9a8a3a](https://via.placeholder.com/15/9a8a3a/9a8a3a.png) |
| Purple | `#6a5a8a` | ![#6a5a8a](https://via.placeholder.com/15/6a5a8a/6a5a8a.png) |

## Quickshell

Config for the Omarchy Quickshell bar: `shell.json`, the `Ocr` core indicator, and the `eclipse.*` plugins it references (`cpu`, `mpris`, `pomodoro`).

```bash
cp quickshell/shell.json ~/.config/omarchy/shell.json
cp -r quickshell/plugins/. ~/.config/omarchy/plugins/
sudo cp -r quickshell/shell/plugins/. "$OMARCHY_PATH/shell/plugins/"
```

The theme's `shell.toml` ships inside `hyprland/themes/titan-black/` and styles the shell when Titan Black is active. Re-run the `sudo cp` after Omarchy updates, which overwrite `$OMARCHY_PATH/shell`.

## Screenshots

### Hyprland
![Hyprland](screenshots/hyprland.png)

Add to your `~/.config/hypr/hyprland.conf`:

```conf
# Titan Black colors
$bg = rgb(050508)
$bgDark = rgb(080810)
$border = rgb(141420)
$accent = rgb(5a9ebf)
$fg = rgb(c8c8d4)

general {
    col.active_border = $accent
    col.inactive_border = $border
    border_size = 2
    gaps_in = 4
    gaps_out = 8
}

decoration {
    col.shadow = $bgDark
    col.shadow_border = $border
}

windowrulev2 = opacity 0.95 0.90, class:.*
```

For Titan Light, use:

```conf
# Titan Light colors
$bg = rgb(f4f5f7)
$bgDark = rgb(e9eaef)
$border = rgb(dfe1e8)
$accent = rgb(5a9ebf)
$fg = rgb(23232e)
```

### opencode
![opencode](screenshots/opencode.png)

### VS Code
![VS Code](screenshots/vscode.png)

### PyCharm
![PyCharm](screenshots/pycharm.png)
