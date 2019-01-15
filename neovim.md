# Neovim

```bash
#!/bin/bash
```

## Introduction

The venerable vim(Neovim). Self explanatory.

## Installation

### Pre-reqs

First let's make sure we have software-properties-common so we can add the ppa

```bash
sudo apt-get install software-properties-common
```

In order to use Python Modules install the dependencies for that.

```bash
sudo apt-get install python-dev python-pip python3-dev python3-pip
```

### Add the PPA and Install Neovim

```bash
sudo apt-get update
sudo apt-get install neovim
```

### Python Provider

Follow the instructions once in nvim.

```vim
:help provider-python
```

Ultimately you will have to install the neovim package from pip

```sh
sudo pip3 install --upgrade neovim
sudo pip2 install --upgrade neovim

```

### Make Neovim Your Preferred Choice

```bash
sudo update-alternatives --install /usr/bin/vi vi /usr/bin/nvim 60
sudo update-alternatives --config vi
sudo update-alternatives --install /usr/bin/vim vim /usr/bin/nvim 60
sudo update-alternatives --config vim
sudo update-alternatives --install /usr/bin/editor editor /usr/bin/nvim 60
sudo update-alternatives --config editor
```