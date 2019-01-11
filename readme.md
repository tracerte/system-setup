# How to Use this Repo
This repo is a set of literate shell scripts and some plain old markdown files used to provision my computers. Each file is written in markdown and most can run as a script.
## Tangling (Scriptifying) The Markdown Files Files
We can generate a bash script using any utility that can pull the markdown code blocks labeled with `bash`. A `sed` command like this is sufficient.
```sh
sed -n '/^```bash/,/^```/ p' < input.md | sed '/^```/ d'
```
## Current Systems
- Lenovo Thinkpad P50: Ubuntu 18.10 (Cosmic Cuttlefish)
## Table of Contents and Basic Order of Execution
## 1. The Basics
### [1.1 Git](git.md)
It is very hard to do anything these days without installing and configuring git.
### [1.2 SSH](ssh.md)
Installing and configuring ssh keys.
### [1.3 Mobile Power Management](mobile-power-management.md)
Installing =tlp= and other battery saving utilities.
### [1.4 Thinkpad Specific Software](thinkpad.md)
### [1.5 Installing ZSH and Oh My ZSH](zsh.md)
### [1.6 Symlinking .zshrc and .bashrc](shell-config.md)
## [2. Building and Installing Emacs](emacs.md)
## 3. Printing and Scanning
### [3.1 Brother DCP-7065DN](brother-dcp-7065dn.md)
## 4. Applications
### [4.1 Redshift](redshift.md)
Save your eyes from blue light.
### [4.2 Riot IM](riot-im.md)
### [4.3 Keybase](keybase.md)
### [4.4 pCloud](pcloud.md)
### [4.5 Signal](signal.md)
## 5. Programming Environments
### [5.1 Shell Script](file:bash-env.md)
### [5.2 Python](python-env.md)
### [5.3 Nim](nim-env.md)
