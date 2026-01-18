# FAQ

## How to I add themes?

To include a theme create a new toml file inside of your alacritty theme folder.
eg(`$HOME/.config/alacritty/themes/themes/`)
`touch $HOME/.config/alacritty/themes/themes/<theme-name>.toml`
edit your toml file with the colorscheme. Checkout some of the themes in [alacritty-theme](https://github.com/alacritty/alacritty-theme/tree/master/themes)

``` TOML
# Theme-name: pencil-light.toml

[colors.primary]
background = "0xf1f1f1"
foreground = "0x424242"

[colors.normal]
black = "0x212121"
red = "0xc30771"
green = "0x10a778"
yellow = "0xa89c14"
blue = "0x008ec4"
magenta = "0x523c79"
cyan = "0x20a5ba"
white = "0xe0e0e0"

[colors.bright]
black = "0x212121"
red = "0xfb007a"
green = "0x5fd7af"
yellow = "0xf3e430"
blue = "0x20bbfc"
magenta = "0x6855de"
cyan = "0x4fb8cc"
white = "0xf1f1f2"
```
