# Brother DCP-7065dn
```bash
#!/bin/bash
```
## Introduction
Very rarely do I need to print, but scanning is certainly helpful.
## Installing The Brother Driver Utility
First, Navigate to the  [Brother Page for the DCP 7065dn](https://support.brother.com/g/b/downloadlist.aspx?c=us&lang=en&prod=dcp7065dn_all&os=128) and download the "Driver Install Tool"

Navigate to the download location and extract the gzip

```shell
$ gunzip linux-brprinter-installer-*.*.*-*.gz
```

As the superuser run the installer that was unzipped

```shell
$ sudo su
$ bash linux-brprinter-installer-*.*.*-* DCP-7065DN
```

Agree to the almost never-ending terms and conditions.

Since I have a networked printer. When asked if "Will you specify the DeviceURI ?", respond with a =Y= and search for your printer.

## Scanning
I like to scan to images as well as to pdfs. So skanlite and gscan2pdf come in handy.

```bash
sudo apt install skanlite gskan2pdf
```
