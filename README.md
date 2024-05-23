# Dotfiles

```markdown
dotfiles/
├── common
│   ├── .config
│   │   ├── alacritty
│   │   ├── fish
│   │   ├── flameshot
│   │   ├── nvim
│   │   ├── nvim_own_broken
│   │   ├── rofi
│   │   └── tmux
│   └── .ideavimrc
├── desktop
│   └── .config
│       └── qtile
├── laptop
│   └── .config
│       └── qtile
├── rofiscripts
│   └── screenSettings.sh
└── scripts
    ├── defaultResolution.sh
    ├── mirrorScreen.sh
    └── screenshot.sh
```
## Requirements
### Git
```bash
pacman -S git
```
### Stow
```bash
pacman -S stow
```
## Installation
Clone the repo
```bash
cd ~/git
```
```bash
git clone https://github.com/yumo4/dotfiles.git
```
```
cd ~/dotfiles 
```
Create the symlinks with ```stow```
```bash
cd ~/git/dotfiles/common
```
```bash
stow -t ~ .
```
### Desktop
Create the symlinks for the ```desktop-qtile-config```
```bash
cd ~/git/dotfiles/desktop
```
```bash
stow -t ~ .
```
### Laptop
Create the symlinks for the ```laptop-qtile-config```

```bash
cd ~/git/dotfiles/latop
```
```bash
stow -t ~ .
```

## Updating
Delete the files in ```~/.config/``` / ```~/``` and use this for updating
```bash
stow --adopt -t ~ .
```
