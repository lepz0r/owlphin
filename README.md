# Owlphin

![preview](./images/preview.png)

A rounded waybar theme with dynamic bar color support, currently support Hyprland only

## Installation

Clone this directory into `~/.config/waybar`

```
git clone https://github.com/lepz0r/owlphin ~/.config/waybar
```

## Features

- Now playing (requires playerctl)\
![mpris](./images/mpris.png)
- Dynamic bar color for single window

## Changing color scheme
Owlphin shipped with some color schemes, to change color scheme just change the line below in `style.css`
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
- [rose-pine-dawn](https://rosepinetheme.com/)
- [rose-pine-moon](https://rosepinetheme.com/) (default color scheme)
