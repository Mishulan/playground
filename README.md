# Mac OS setup

## Brew
Link: https://brew.sh/
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew upgrade
```
Brew installed packages location:
> /opt/homebrew/Cellar & /opt/homebrew/Caskroom

## Bourne Again SHell
Link: https://www.gnu.org/software/bash/ \
Installation: https://dev.to/bphogan/use-modern-bash-shell-on-macos-22a6
```
brew install bash
echo "$(brew --prefix)/bin/bash" | sudo tee -a /etc/shells;
chsh -s "$(brew --prefix)/bin/bash"
```
> To see where Homebrew installed Bash, run the following command:
```
ls "$(brew --prefix)/bin/bash" 
```

## Alacritty
Link: https://alacritty.org/
Themes: https://github.com/alacritty/alacritty-theme
```
brew install --cask alacritty
# We use Alacritty's default Linux config directory as our storage location here.
mkdir -p ~/.config/alacritty/themes
git clone https://github.com/alacritty/alacritty-theme ~/.config/alacritty/themes
alacritty.toml
import = [
    "~/.config/alacritty/themes/themes/{theme}.toml"
]
```
> You can now swithch to Alacritty and continue from there

## Nerd font
Link: https://gist.github.com/davidteren/898f2dcccd42d9f8680ec69a3a5d350e / https://www.nerdfonts.com/
```
brew tap homebrew/cask-fonts && brew install --cask font-jetbrains-mono-nerd-font
```

## Starship prompt
Link: https://starship.rs/
```
brew install starship
# ~/.bashrc
eval "$(starship init bash)"
```

## Rectangle
Link: https://github.com/rxhanson/Rectangle
```
brew install --cask rectangle
```

## Numi calculator
Link: https://github.com/nikolaeu/numi
```
brew install nikolaeu/numi/numi-cli
```

## zsh
> aleady installed on mac > 10.15

## oh my zsh
> plugin manager for zsh - need to evaluate
