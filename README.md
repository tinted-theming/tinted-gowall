# tinted-gowall

use [gowall](https://github.com/Achno/gowall) to make your wallpaper adhere to your [Base16]/[Base24] theme.

## Basic Usage Instructions

Add the following toml settings to your [Tinty] `~/.config/tinted-theming/tinty/config.toml` file:

```toml
[[items]]
path = "https://github.com/tinted-theming/tinted-gowall"
name = "wallpaper"
themes-dir = "themes" 
supported-systems = ["base16", "base24"]
```

This will create a gowall compatible JSON config file that you can then use to apply your theme:

`gowall convert [INPUT] [OPTIONAL OUTPUT] -t <PATH_TO_YOUR_THEME>`

## Example with [chicago]

`gowall convert wallpaper.jpg -t base16-chicago-day.json`

<span>
<img src="img/before.jpg" height="300" />
==>
<img src="img/after.jpg" height="300" />
</span>

[Base16]: https://github.com/tinted-theming/home/blob/main/styling.md
[Base24]: https://github.com/tinted-theming/base24/blob/main/styling.md
[gowall]: https://github.com/Achno/gowall
[Tinty]: https://github.com/tinted-theming/tinty
[chicago]: https://github.com/rwendell/chicago-theme
