# SSH

## Introduction

Setting up my SSH directory structure and adding the to the =ssh-agen=

## Setup SSH Keys

### Setup directories

- Home directory should not be accessible by groups or others: at most `755 (drwxr-xr-x)`
- SSH directory (`.ssh`): `700 (drwx------)`
- public key (=.pub= file): `644 (-rw-r--r--)`
- private key (=id_rsa= file): `600 (-rw-------)`

```sh

$ mkdir ~/.ssh
$ chmod 700 ~/.ssh/
$ chmod 644 ~/.ssh/id_rsa.pub
$ chmod 600 ~/.ssh/id_rsa
>
```

### Add Keys to ssh-agent

First start the ssh-agent

```sh
$ eval "$(ssh-agent -s)"
>
```

Now Add the keys to the ssh-agent

```sh
$ ssh-add ~/.ssh/id_rsa
>
```
