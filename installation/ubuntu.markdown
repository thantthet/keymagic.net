---
title: Installation on Ubuntu
date: 2019-03-01 17:23:00 +06:30
---

You may use one of the following methods to install KeyMagic on Ubuntu. These may also work for other Debian based Linux OSes. Thanks to Koko Ye and Ubuntu-MM for providing packages.

### Installing from kokoye2007 PPA
```
sudo add-apt-repository -y ppa:kokoye2007/ppa
sudo apt-get update
sudo apt-get install ibus-keymagic
```
### Installing from Ubuntu-MM PPA
```
sudo add-apt-repository -y ppa:ubuntu-mm/ppa
sudo apt-get update
sudo apt-get install ibus-keymagic
ibus-setup & ibus-daemon -rdx
```
