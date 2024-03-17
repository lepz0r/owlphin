# Owlphin

![preview](./images/preview.png)

A rounded waybar theme with dynamic bar color for Hyprland and sway.

## Requirements
- Nerd Font for icons (default font is FantasqueSansM Nerd Font)
- playerctl for music widget
- sway or Hyprland for workspace & dynamic bar color

## Installation

Clone this directory into `~/.config/waybar`

```
git clone https://github.com/lepz0r/owlphin ~/.config/waybar
```

#### Hyprland
For Hyprland add this line below to `~/.config/hypr/hyprland.conf`.
```
exec-once=waybar &
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
Owlphin shipped with color schemes below, to change the color scheme just change lines below in `style.css`
```
@import url("colorschemes/<colorscheme_name>/style.css");
@import url("colorschemes/<colorscheme_name>/app.css");
```

Available color schemes:
- [dracula](https://draculatheme.com/)
- [everforest-light-medium](https://github.com/sainnhe/everforest)
- [fairyfloss](https://sailorhg.github.io/fairyfloss/)
- [gruvbox](https://github.com/morhetz/gruvbox)
- [noctis-lilac](https://github.com/liviuschera/noctis)
- [rose-pine](https://rosepinetheme.com/)
- [rose-pine-dawn](https://rosepinetheme.com/)
- [rose-pine-moon](https://rosepinetheme.com/) (default color scheme)
- [catppuccin-latte](https://github.com/catppuccin)
- [catppuccin-frappe](https://github.com/catppuccin)
- [catppuccin-macchiato](https://github.com/catppuccin)
- [catppuccin-mocha](https://github.com/catppuccin)
