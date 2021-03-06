![](preview/bolt.gif)

# Bolt: Lighting fast launcher for the fastest Unix workflow ever

Bolt prompts you for keywords to your local files, directories or Google search and launches them respectively.

# Features

-  A **paths** file to generate a personalized search list

-  A **filters** file to filter out irrelevant matches

-  A monitoring script to update the search list in real-time

-  A custom launch script to easily define launch programs (unlike **xdg-open**)

-  Googling capability

-  Runs as fast as it gets! (hint: shellscript)

## Dependencies

-  shift, grep, sed, find, awk, xargs, file

-  [Rofi](https://github.com/davatorium/rofi)

-  [Inotify-tools](https://github.com/inotify-tools/inotify-tools)

-  [Tmux](https://github.com/tmux/tmux) (optional)

-  [FZF](https://github.com/junegunn/fzf) (optional)

## Prerequisite

-  Modify the launch section of the source code according to your preference

## Installation

```sh
git clone https://github.com/salman-abedin/bolt.git && cd bolt && sudo make install
```

## Usage

-  Create a **paths** and a **filters** file in **~/.config/bolt**.
   Here is a couple of [examples](https://github.com/salman-abedin/bolt/tree/master/example_config)

-  run `bolt --generate --watch` at startup to generate and monitor the search list respectively

-  Bind a key combination with the command `bolt --rofi-search` to launch the prompt

-  Type the keyword, press enter and baam!

-  (Optional) You can also use `bolt --tmux-launch` && `bolt --fzf-search` at your own discretion

## Uninstallation

```sh
sudo make uninstall
```

## Patches

-  **24/06/20**:- Added two column prompt for more accurate searching

-  **30/06/20**:- Added googling support

-  **05/07/20**:- Added tmux and fzf support

## FAQ

### Why not use xdg-open?

I hate xdg-open. Because...

1. it will only work on linux

2. Second, You have to modify two files in two different locations writing no less than 5 lines with root level shell scripting.
   I would much rather have you use a one liner like in my script and keep it much more flexible.

---

## Repos you might be interested in

[Crystal](https://github.com/salman-abedin/crystal)
: The transparent setup

[Magpie](https://github.com/salman-abedin/magpie)
: The dotfiles

[Alfred](https://github.com/salman-abedin/alfred)
: The scripts

[Devour](https://github.com/salman-abedin/devour)
: Terminal swallowing

[Uniblocks](https://github.com/salman-abedin/uniblocks)
: The status bar

## Contact

SalmanAbedin@disroot.org
