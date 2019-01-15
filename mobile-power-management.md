# Mobile Power Management

```bash
#!/bin/bash
```

## Introduction

Let's make sure to try to squeeze as much juice out of this battery that we can.

## Installation

`tlp`: Advanced power management tool
`tlp-rdw`: Radio Device Wizard - needed to enable/disable & Power saving (Wifi / Bluetooth )
`smartmontools`: needed by tlp-stat to display disk drive S.M.A.R.T. data
`ethtool`: is needed to disable wake on LAN

```bash
sudo apt install tlp tlp-rdw smartmontools ethtool 
```

## Setup

Now start the service.

```bash
sudo tlp start
```

Check Stats, and ensure it's enabled

```bash
sudo tlp-stat -s
```
