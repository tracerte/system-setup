# Riot IM

```bash
#!/bin/bash
```

## Introduction

Riot is a secure messaging service built around the Matrix protocol

## Installing Riot

```bash
sudo sh -c "echo 'deb https://riot.im/packages/debian/ cosmic main' > /etc/apt/sources.list.d/matrix-riot-im.list"
curl -L https://riot.im/packages/debian/repo-key.asc | sudo apt-key add -
sudo apt-get update && sudo apt-get -y install riot-web
```

## Installing Room Keys

Add your Room Keys file via the application to access encrypted rooms.
