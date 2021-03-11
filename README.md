# Custom config for support bash or zsh :computer:

1. Aliasas
1. Function

Clone this repository to `user configuration` directory to your home directory: `$HOME/.config`

```bash
# Install configs
$ git clone https://github.com/asapmac/yabai-config.git "${HOME}"/.config/asapmac
```

Add script to load `functions` and `aliases` to ZSH or BASH config `(.zshrc or bashrc)` on the bottom.

```bash
source $HOME/.config/asapmac/aliases
source $HOME/.config/asapmac/functions
```

## Note:

> Change your environment variables config on `.env`

example:

```bash
EDITOR='vim'
```

# Yabai and skhd configs

My personal yabai and skhd configs

See my [dotfiles](https://gitlab.com/julian-heng/dotfiles.git) repo for my other configs

NOTE: yabai requires System Integrity Protection to be disabled to work properly. See [here](https://github.com/koekeishiya/yabai/wiki/Disabling-System-Integrity-Protection) for more information.

## Installing for yabai

```sh
# Remove previous links
$ rm -f "${HOME}"/.{yabai,skhd}rc

$ ln -s "${HOME}/.config/asapmac/yabai/yabairc" "${HOME}/.yabairc"
$ ln -s "${HOME}/.config/asapmac/yabai/skhdrc" "${HOME}/.skhdrc"
```

## Keyboard shortcuts

### Yabai

#### Changing focus

<kbd>alt</kbd> + <kbd>hjkl</kbd>

#### Resize windows

| Action       | Key Combination                                 |
| ------------ | ----------------------------------------------- |
| Resize left  | <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>h</kbd> |
| Resize down  | <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>j</kbd> |
| Resize up    | <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>k</kbd> |
| Resize right | <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>l</kbd> |
| Equalise     | <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>0</kbd> |

#### Move windows

<kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>hjkl</kbd>

#### Move windows to workspace

| Action                      | Key Combination                                    |
| --------------------------- | -------------------------------------------------- |
| Send to last active desktop | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>m</kbd>   |
| Send to previous workplace  | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>p</kbd>   |
| Send to next workplace      | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>n</kbd>   |
| Send to workplace           | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>num</kbd> |

#### Rotate windows

| Action               | Key Combination                                  |
| -------------------- | ------------------------------------------------ |
| Rotate clockwise     | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>r</kbd> |
| Rotate anticlockwise | <kbd>alt</kbd> + <kbd>r</kbd>                    |
| Flip on x-axis       | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>x</kbd> |
| Flip on y-axis       | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>y</kbd> |

#### Window actions

| Action            | Key Combination                                  |
| ----------------- | ------------------------------------------------ |
| Fullscreen        | <kbd>alt</kbd> + <kbd>f</kbd>                    |
| Native fullscreen | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>f</kbd> |
| Center window     | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>c</kbd> |

#### Insertion point

| Action                       | Key Combination                                                    |
| ---------------------------- | ------------------------------------------------------------------ |
| Insert left                  | <kbd>shift</kbd> + <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>h</kbd> |
| Insert down                  | <kbd>shift</kbd> + <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>j</kbd> |
| Insert up                    | <kbd>shift</kbd> + <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>k</kbd> |
| Insert right                 | <kbd>shift</kbd> + <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>l</kbd> |
| Cancel insert (chunkwm only) | <kbd>shift</kbd> + <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>x</kbd> |

#### Misc

| Action          | Key Combination                                                    |
| --------------- | ------------------------------------------------------------------ |
| Toggle float    | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>space</kbd>               |
| Toggle gaps     | <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>g</kbd>                    |
| Restart chunkwm | <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>r</kbd> |

### Non-chunkwm

#### Show information

##### Description

Uses `osascript` to show information like CPU, memory, battery, etc. The CPU script requires [osx-cpu-temp](https://github.com/lavoiesl/osx-cpu-temp) installed. The song script supports iTunes and cmus.

Click [here](scripts) to view the script folder

Note: May have to change the location of the scripts in skhdrc

##### Key Combination

<kbd>fn</kbd> + <kbd>alt</kbd> + <kbd>num</kbd>

##### Screenshots

<img width="382" height="101" src="screenshots/cpu.png?raw=true"><img width="382" height="101" src="screenshots/mem.png?raw=true">
<img width="382" height="101" src="screenshots/bat.png?raw=true"><img width="382" height="101" src="screenshots/disk.png?raw=true">
<img width="382" height="101" src="screenshots/song.png?raw=true">

```
fn + alt - 1 : /path/to/script
fn + alt - 2 : /path/to/script
fn + alt - 3 : /path/to/script
...
```

#### Opening applications

#### Launch iTerm2

##### Description

Launches iTerm2 using like in i3-wm.

Click [here](scripts/open_iterm2.sh) to view the script

##### Key Combination

<kbd>cmd</kbd> + <kbd>return</kbd>

```
cmd - return : /path/to/launch/terminal
```

Refrence :

- [Yabai Config](https://github.com/Julian-Heng/chunkwm-yabai-config)
- [Emoji Log](https://github.com/ahmadawais/Emoji-Log)

If any issue please contact me [@asapdotid](mailto:asapdotid@gmail.com) :point_left:
