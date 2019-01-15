# ZSH

```bash
#!/bin/bash
```

## Introduction

Bash is so boring, let's install ZSH.

## Install ZSH

Zsh is available via `apt`

```bash
echo "Install zsh..."
sudo apt install zsh
```

## Oh My Zsh
Let's install Oh My Zsh

```bash
echo "Cloning Oh My ZSH..."
git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
```

## Powerlines Fonts
Make our terminal use pretty symbols

```bash
echo "Installing Powerline Fonts..."
sudo apt install fonts-powerline
```

## ZSH Completions

```bash
echo "Installing ZSH Completions..."
git clone https://github.com/zsh-users/zsh-completions ~/.oh-my-zsh/custom/plugins/zsh-completions
```

## ZSH Autosuggestions

```bash
echo "Installing ZSH Autosuggestions..."
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
```

## Syntax Highlighting

```bash
echo "Installing Syntax Highlighting..."
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
```

## ZSH-256

Use all the available terminal colors

```bash
echo "Install ZSH-256..."
git clone https://github.com/chrissicool/zsh-256color ~/.oh-my-zsh/custom/plugins/zsh-256color
```

## Better Directory Colors

```bash
echo "Install dircolors..."
wget https://raw.githubusercontent.com/seebi/dircolors-solarized/master/dircolors.256dark -O ~/.dircolors
```

## Dotfiles
Please see my shell-config repository for the =.zshrc= used.

```bash
echo "Please install .zshrc from git repo"
```

## Making ZSH Default
You can change the default shell to zsh using the following command

```sh
$ chsh -s $(which zsh)
>
```
