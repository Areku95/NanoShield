# NanoShield

This project aims to provide a customized NanoBSD image for Stormshield and Netasq appliances, in order to recycle old appliances.

Please note that, for now, only the appliances Netasq U70S and Stormshield SN300 are tested and valided.

## How to build the image file ?

<ins>**Prerequisites:**</ins>

- Having a FreeBSD operating system running somewhere (virtual machine, old computer, ...)

### 1. Download the sources

First of all, we'll need to download the sources of FreeBSD :

`# fetch ftp://ftp.freebsd.org/pub/FreeBSD/releases/amd64/12.2-RELEASE/src.txz`

And extract it :

`# tar -C / -xzvf src.txz`

### 2. Download the required packages

`# mkdir /usr/src/packages`
`# pkg fetch -o /root/packages/ -d pkg isc-dhcp44-server`
