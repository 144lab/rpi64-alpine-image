# rpi64-alpine-image
Alpine Linux bootable image for raspberrypi 3 or 4

Currently Alpine version 3.13.4!

### Usage:

#### step1

Format microSD-card for FAT32 with label 'ALPINE'.

#### step2

```
git clone https://github.com/144lab/rpi64-alpine-image.git
cd rpi64-alpine-image
git archive main | tar xv -C /Volumes/ALPINE
curl https://github.com/<your-github-account-id>.keys > /Volumes/ALPINE/authorized_keys
```

#### step3

- eject microSD-card from PC.
- insert microSD-card into raspberrypi3 or 4.
- connect ether cable from LAN rooter into raspberrypi.
- start power supply for raspberrypi.

#### step4

```
ssh root@raspberrypi.local
```
