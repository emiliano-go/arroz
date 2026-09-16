# Titan Black

> "Rice" in Spanish is "arroz". This is my rice ("arroz" in Spanish).

Vanta Black-based dark theme with cool sci-fi accents for Hyprland, opencode, VS Code, and PyCharm.

Inspired by deep space imagery: near-black backgrounds with teal/cyan ambient glow and warm highlights.

![wallpaper](screenshots/wallpaper.jpg)

## Apps

| App | Directory | Install |
|-----|-----------|---------|
| **Hyprland** | `hyprland/themes/titan-black/` | Copy wallpaper to `~/.config/hypr/wallpapers/` and add colors to `hyprland.conf` (see below) |
| **opencode** | `opencode/themes/` | Copy `titan-black.json` to `~/.config/opencode/themes/` and set `"theme": "titan-black"` in `tui.json` |
| **VS Code** | `vscode-titan-black/` | `code --install-extension vscode-titan-black/titan-black.vsix` |
| **PyCharm** | `pycharm/titan-black.jar` | Settings → Plugins → Install Plugin from Disk → select `titan-black.jar` |

## Color Palette

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

### opencode
![opencode](screenshots/opencode.png)

### VS Code
![VS Code](screenshots/vscode.png)

### PyCharm
![PyCharm](screenshots/pycharm.png)
