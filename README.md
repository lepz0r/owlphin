# Owlphin

![preview](./images/preview.png)

A rounded waybar theme with dynamic bar color for Hyprland and sway.

## Requirements

- Nerd Font for icons (default font is MonaspiceNe Nerd Font)
- playerctl for music widget
- sway or Hyprland for workspace & dynamic bar color

## Installation

Clone this directory into `~/.config/waybar`

```
git clone https://github.com/lepz0r/owlphin ~/.config/waybar
```

#### Hyprland

Add this line below to `~/.config/hypr/hyprland.conf`, by default `config` is symlinked to `config-hyprland` so just running waybar without running will use the Hyprland config.

```
exec-once=waybar &
```

If you changed the `config` symlink to link to something else add this line below instead.

```
exec-once=waybar & -c ~/.config/waybar/config-hyprland
```

#### sway

For sway add this line below to `~/.config/sway/config`.

```
exec waybar -c ~/.config/waybar/config-sway
```

And don't forget to remove or comment out lines below to disable swaybar.

```
#
# Status Bar:
#
# Read `man 5 sway-bar` for more information about this section.
bar {
    position top

    # When the status_command prints a new line to stdout, swaybar updates.
    # The default just shows the current date and time.
    status_command while date +'%Y-%m-%d %I:%M:%S %p'; do sleep 1; done

    colors {
        statusline #ffffff
        background #323232
        inactive_workspace #32323200 #32323200 #5c5c5c
    }
}

```

## Features

- Now playing (requires playerctl)\
  ![mpris](./images/mpris.png)
- Dynamic bar color for single window

## Changing color scheme

Owlphin shipped with color schemes below, to change the color scheme just change lines below in `styleoptions.css`

```
@import url("colorschemes/<colorscheme_name>/style.css");
```

Available color schemes:

- [catppuccin-frappe](https://github.com/catppuccin)
- [catppuccin-latte](https://github.com/catppuccin)
- [catppuccin-macchiato](https://github.com/catppuccin)
- [catppuccin-mocha](https://github.com/catppuccin)
- [dracula](https://draculatheme.com/)
- [everforest-dark-hard](https://github.com/sainnhe/everforest)
- [everforest-dark-medium](https://github.com/sainnhe/everforest)
- [everforest-dark-soft](https://github.com/sainnhe/everforest)
- [everforest-light-hard](https://github.com/sainnhe/everforest)
- [everforest-light-medium](https://github.com/sainnhe/everforest)
- [everforest-light-soft](https://github.com/sainnhe/everforest)
- [fairyfloss](https://sailorhg.github.io/fairyfloss/)
- [gruvbox-dark](https://github.com/morhetz/gruvbox)
- [gruvbox-light](https://github.com/morhetz/gruvbox)
- [iceberg](https://cocopon.github.io/iceberg.vim/)
- [kanagawa-dragon](https://github.com/rebelot/kanagawa.nvim)
- [kanagawa-lotus](https://github.com/rebelot/kanagawa.nvim)
- [kanagawa-wave](https://github.com/rebelot/kanagawa.nvim)
- [noctis-lilac](https://github.com/liviuschera/noctis)
- [nord-dark](https://www.nordtheme.com/)
- [nord-light](https://www.nordtheme.com/)
- [onedark](https://github.com/atom/atom/tree/master/packages/one-dark-ui)
- [rose-pine-dawn](https://rosepinetheme.com/)
- [rose-pine-moon](https://rosepinetheme.com/) (default color scheme)
- [rose-pine](https://rosepinetheme.com/)
- [tokyo-night](https://github.com/enkia/tokyo-night-vscode-theme)
- [tokyo-night-day](https://github.com/enkia/tokyo-night-vscode-theme)
- [tokyo-night-moon](https://github.com/enkia/tokyo-night-vscode-theme)
- [tokyo-night-storm](https://github.com/enkia/tokyo-night-vscode-theme)
- [witchhazel](https://witchhazel.thea.codes/)
- [witchhazel-hypercolor](https://witchhazel.thea.codes/)
