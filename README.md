# config-tmux

## Description

This is my custom tmux config. It requires a little work on your part, but the directions are pretty easy to follow.

### Notes:
- the `prefix` has been remapped to `C-a` (Ctrl+a)
- you may have to play around with the settings to get plugins to work for your location

## Requirements
- tmux >= 1.9
- git
- bash shell
- terminal that supports 256 color
    - if over SSH, make sure to define `SetEnv TERM=xterm-256color` in your local machine `.ssh/config`

## Installation

Git clone this repository

```shell
git clone git@github.com:beatzball/config-tmux.git ~/config-tmux/
```

Make a symbolic link of `~/tmux.conf`

```shell
ln -s ~/config-tmux/.tmux.conf ~/.tmux.conf
```

Install the Tmux Package Manager [TPM]()

```shell
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

Start a Tmux session

```shell
tmux new-session -As <whatever-you-want-to-call-it>
```

Trigger the installation
- `prefix` then `I`
- `Ctrl+A` then captial `i`

Update
- `prefix` then `U`

Remove/Uninstall plugins not on the plugin list
- `prefix` then `Alt+U`

## Uninstall

```shell
rm -rf ~/.tmux/ ~/tmux-config ~/.tmux.conf
```

## Screenshots
![Screenshot](https://github.com/beatzball/config-tmux/assets/38116726/b6893ae8-aa41-4681-89d2-63a63c1d0be9)
