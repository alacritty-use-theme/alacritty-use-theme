# alacritty-use-theme

Small utility to switch the selected theme used by alacritty terminal.

# Install
1. `yay -S alacritty-use-theme`
2. Source the script by adding this to your .bashrc
```sh
[[ -f /usr/bin/alacritty-use-theme/use-theme.sh ]] && source /usr/bin/alacritty-use-theme/use-theme.sh
```
4. Add themes to the "themes" directory usually located at

```SH
$HOME/.config/alacritty/themes/<theme>
```

_For additional information_ check out the [FAQ > How to add themes](docs/faq.md)
   
5. Import the selected theme

```TOML
[general]
import = ["themes/selected.toml"]
```


# Usage
  _alacritty-use-theme will attempt to switch the theme to one that is installed.
  If the theme cannot be found alacritty-use-theme will use its default theme "tomorrow-night"_

```sh
    alacritty-use-theme # Will use alacritty's default theme.
    alacritty-use-theme XTerm # uses a theme installed in ~/.config/alacritty/themes/<themeName>
    alacritty-use-theme day # uses an alias for an installed theme.
```
# Aliases

## Creating aliases
1. Create an aliases file inside of your alacritty configuration
```
touch $HOME/.config/alacritty/themes/alaises.toml
```

```toml
# aliases.toml
[aliases]
day = "pencil-light"
night =  "default" # "default" will use the default theme in alacritty
```
