# alacritty-use-theme

Small utility to switch the selected theme used by alacritty terminal.

# Install
1. `pacman -U alacritty-use-theme`
2. Source the script by adding this to your .bashrc
`[[ -f /usr/bin/alacritty-use-theme/use-theme.sh ]] && source /usr/bin/alacritty-use-theme/use-theme.sh`
3. Add themes to the themes directory `$HOME/.config/alacritty/themes/<theme>`
4. Import the selected theme
```TOML
[general]
import = ["themes/selected.toml"]
```

# Creating aliases
1. Create an aliases file inside of your alacritty configuration
`touch $HOME/.config/alacritty/alaises.toml`

```toml
# aliases.toml

day = "pencil-light"
# night =  "your-theme-name"
```

# Usage
  _alacritty-use-theme will attempt to switch the theme to one that is installed.
  If the theme cannot be found alacritty-use-theme will use its default theme "tomorrow-night"_

`alacritty-use-theme day`
`alacritty-use-theme night`
