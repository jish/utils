This repo is generally split into two parts:

1. Little utilities for everyday use in `bin/`

  * `pomodoro` -- start a pomodoro timer
  * `readability` -- turn a URL into a content-only version using https://www.readability.com/
  * `set_author` -- setup author details in a Git repo

2. Scripts to help setup a new machine

  * Install Homebrew packages
  * Setup Vim
  * Install dotfiles

### Usage

Install all of the binaries in the `bin/` directory to `~/bin`:

    rake install

Bootstrap a new machine:

    ./script/bootstrap

#### Run single one off scripts:

Install homebrew packages:

    ./script/packages

Setup vim:

    ./script/setup_vim
