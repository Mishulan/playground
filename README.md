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
Link: https://www.gnu.org/software/bash/
```
brew install bash
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
```
> You can now swithch to Alacritty and continue from there

## Nerd font
Link: https://gist.github.com/davidteren/898f2dcccd42d9f8680ec69a3a5d350e / https://www.nerdfonts.com/
```
brew tap homebrew/cask-fonts && brew install --cask font-jetbrains-mono-nerd-font
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
