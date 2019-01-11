# Python Language Environment

```bash
#!/bin/bash
```
##  Introduction
I tend not to depend on the system installed python interepreters. I only really use python3 and miniconda3. This org file will go into detail on how to setup a python development environment. I currently use anaconda-mode in emacs, which at the moment, only requires setuptools.

## pyenv
### Dependencies
```bash
 sudo apt install -y build-essential libbz2-dev zlib1g-dev libssl-dev libreadline-dev libsqlite3-dev tk-dev libffi-dev
```
### Install
```bash
git clone https://github.com/pyenv/pyenv.git ~/.pyenv
```
## pyenv-virtualenv
```bash
git clone https://github.com/pyenv/pyenv-virtualenv.git $(pyenv root)/plugins/pyenv-virtualenv
```
## Make Changes to bashrc or zshrc
Add the following lines to enable pyenv and pyenv-virtualenv

```sh
# pyenv
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"

if command -v pyenv 1>/dev/null 2>&1; then
  eval "$(pyenv init -)"

  eval "$(pyenv virtualenv-init -)"
fi
```
## Python3 and Miniconda Installation
```sh
$ pyenv install 3.7.2
$ pyenv pyenv install miniconda3-4.3.30
```
## Setup Environments
### Python3 Ipython and Jupyter Global Environment
```sh
$ pyenv virtualenv 3.7.2 jupyter3   
$ pyenv activate jupyter3
$ pip install jupyter
$ python -m ipykernel install --user
$ pyenv deactivate
```
### Userland Utilities
Use virtual environments, whenever possible, do not pollute the global python package namespace. You can create a tools environment like so
```sh
$ pyenv virtualenv 3.7.2 tools3
```
### Set Python Global Environment(s)
For now I am just using my jupyter3 environment as my global.
```sh
pyenv global jupyter3 tools3
```
