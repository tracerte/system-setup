# Nim Language Environment
```bash
#!/bin/bash
```
## Introduction
Nim is a relatively new programming language with syntax similar to python, macros similar to a lisp and best yet, compiles down to C.
## Installation
### Dependencies
Ensure GCC is installed
```bash
sudo apt install build-essential
```
I also want the Clang compiler too, so we can take advantage of LLVM
```bash
sudo apt install clang cmake clang-format libclang-dev
```
### Install choosenim
=choosenim= is a tool similar to =pyenv= which allows you to have multiple versions of nim installed on your computer and switch between them, fairly seamlessly.
```bash
curl https://nim-lang.org/choosenim/init.sh -sSf | sh
```
### Configuration
We must add nim to our PATH.  Add this to your bashrc or zshrc file.
```sh
export PATH=~/.nimble/bin:$PATH
``` 
