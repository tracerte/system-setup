# How to Use this Repo

This repo is a set of literate shell scripts and some plain old markdown files used to provision my computers. Each file is written in markdown and most can run as a script.

## Tangling (Scriptifying) The Markdown Files Files

We can generate a bash script using any utility that can pull the markdown code blocks labeled with `bash`. A `sed` command like this is sufficient.

```sh
sed -n '/^```bash/,/^```/ p' < input.md | sed '/^```/ d'
```

## Current Systems

- Lenovo Thinkpad P50: Kubuntu 18.10 (Cosmic Cuttlefish)

## Table of Contents and Basic Order of Execution

## 1. The Basics

### [1.1 Git](git.md)

It is very hard to do anything these days without installing and configuring git.

### [1.2 SSH](ssh.md)

Installing and configuring ssh keys.

### [1.3 Mobile Power Management](mobile-power-management.md)

Installing `tlp` and other battery saving utilities.

### [1.4 Thinkpad Specific Software](thinkpad.md)

### [1.5 Installing ZSH and Oh My ZSH](zsh.md)

### [1.6 Symlinking .zshrc and .bashrc](shell-config.md)

## 2. Printing and Scanning

### [2.1 Brother DCP-7065DN](brother-dcp-7065dn.md)

## 3. Applications

### [3.1 Redshift](redshift.md)

Save your eyes from blue light.

### [3.2 Riot IM](riot-im.md)

### [3.3 Keybase](keybase.md)

### [3.4 pCloud](pcloud.md)

### [3.5 Signal](signal.md)

### [3.6 Web Browser](web-browsers.md)

### [3.7 Visual Studio Code](vscode.md)

### [3.8 Neovim](neovim.md)

## 4. Programming Environments

### [4.1 Shell Script](bash-env.md)

### [4.2 Rust](rust-env.md)
