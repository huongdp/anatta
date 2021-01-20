# INSTALLATION

## MacOS

- Homebrew Cask

```
brew install --cask alacritty
brew install --cask dash
brew install --cask docker
brew install --cask firefox
brew install --cask karabiner-elements
brew install --cask openkey
brew install --cask microsoft-edge
brew install --cask mpv
brew install --cask notion
brew install --cask visual-studio-code
```

- Commands

```
brew install font-hack-nerd-font
brew install pyenv
brew install fzf
brew install luajit --HEAD && brew install --HEAD nvim
brew install tmux
brew install vifm
brew install yabai
brew install zsh


```

## Ubuntu
 
- Install dependencies:
```
sudo apt purge -y picom
sudo apt install -y libxext-dev libxcb1-dev libxcb-damage0-dev libxcb-xfixes0-dev libxcb-shape0-dev libxcb-render-util0-dev libxcb-render0-dev libxcb-randr0-dev libxcb-composite0-dev libxcb-image0-dev libxcb-present-dev libxcb-xinerama0-dev libxcb-glx0-dev libpixman-1-dev libdbus-1-dev libconfig-dev libgl1-mesa-dev  libpcre2-dev  libevdev-dev uthash-dev libev-dev libx11-xcb-dev
sudo apt install -y cmake meson gcc
```

- Clone source code and build:
```
git clone https://github.com/jonaburg/picom

cd picom
meson --buildtype=release . build
ninja -C build
sudo ninja -C build install

```