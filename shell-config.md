# Shell Configuration

```bash
#!/bin/bash
```
## Introduction

Like most people, my configuration files are source controlled. Time to install them.

## Shell Configuration Files
My shell configuration files are in my `shell-config` git repo.

Let's pull the repo.
```bash
  echo "Do you wish to clone the shell-config repo?"
  select yn in "Yes" "No"; do
      case $yn in
          Yes ) git clone https://github.com/tracerte/shell-config ~/shell-config;
                break;;
          No ) break;;
      esac
  done

```
Now we can enter the repo and Start Symlinking
## Bash
```bash
  echo "Do you wish to symlink the bashrc?"
  select yn in "Yes" "No"; do
      case $yn in
          Yes ) cd ~/shell-config;
                if [ -f ~/.bashrc ]; then
                    mv ~/.bashrc ~/.bashrc.orig
                fi
                ln -sfr ./bash/bashrc ~/.bashrc
                break;;
          No ) break;;
      esac
  done
```
## ZSH
```bash
  echo "Do you wish to symlink the zshrc?"
  select yn in "Yes" "No"; do
      case $yn in
          Yes ) cd ~/shell-config;
                if [ -f ~/.zshrc ]; then
                    mv ~/.zshrc ~/.zshrc.orig
                fi
                ln -sfr ./zsh/zshrc ~/.zshrc
                break;;
          No ) break;;
      esac
  done
```
