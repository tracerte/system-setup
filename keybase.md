# Keybase

```bash
#!/bin/bash
```

## Introduction

Keybase is a program used to manage your identity with PGP. It also has a nifty encrypted and signed git component.

## Installing Keybase

```bash
# ensure curl is installed
sudo apt install curl
curl -O https://prerelease.keybase.io/keybase_amd64.deb
# if you see an error about missing `libappindicator1`
# from the next command, you can ignore it, as the
# subsequent command corrects it
sudo dpkg -i keybase_amd64.deb
sudo apt-get install -f
run_keybase
```
