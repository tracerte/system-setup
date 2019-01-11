# Signal

```bash
#!/bin/bash
```

## Introduction
Signal is a secure communications service that implements the whisper protocol.

## Installation
### Add the repo keys
```bash
curl -s https://updates.signal.org/desktop/apt/keys.asc | sudo apt-key add -
echo "deb [arch=amd64] https://updates.signal.org/desktop/apt xenial main" | sudo tee -a /etc/apt/sources.list.d/signal-xenial.list
```
### Install the program from the repo
```bash
sudo apt update && sudo apt install signal-desktop
```
