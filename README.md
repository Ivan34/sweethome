# SweetHome
Configuration files for Python coding with Vim, Emacs, Xterm, Git and Qtile

## Installation
* Clone the repository into your home directory:
```bash
git clone --recursive https://github.com/tcsorrel/sweethome.git ~/sweethome
```

## Integration
Each part of sweethome may be integrated seperately,
depending on what is needed.

### VIM
* Use sweethome's vimrc and install plugins with
[Vundle](https://github.com/gmarik/Vundle.vim):
```bash
$ ln -s ~/sweethome/vim/vimrc ~/.vimrc
$ vim +PluginInstall +qa
```

### Emacs
* Use sweethome's .emacs:
```bash
$ ln -s ~/sweethome/emacs/emacs ~/.emacs
```
Mode packaging requires `emacs 24.4+` or `package.el`.

### Git
* Include the gitconfig file in your `~/.gitconfig`:
```INI
[user]
    name = Your Name
    email = your.name@email.example
...
[include]
    path = ~/sweethome/git/config
```
The .gitconfig `[include]` syntax requires `git 1.7.10+`.

### X resources
* Use sweethome's Xresources file to configure Xterm font and colors:
```bash
$ ln -s ~/sweethome/x/resources ~/.Xresources
$ xrdb -merge ~/.Xresources
```

### Qtile configuration
* Use sweethome's configuration for Qtile window manager:
```bash
$ ln -s ~/sweethome/qtile/config.py ~/.config/qtile/config.py
```
