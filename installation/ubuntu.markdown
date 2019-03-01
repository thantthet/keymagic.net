---
title: Installation on Ubuntu
date: 2019-03-01 17:23:00 +06:30
---

You may use one of the following methods to install keymagic on Ubuntu. These may also work for other Debian based Linux OSes.

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
### Installing using deb
1. Download the keymagic deb package for iBus from [downloads](/downloads) page.
2. Open the downloaded folder and double click the `ibus-keymagic_1.4.1.20110528-1_i386.deb`. (`ibus-keymagic_1.4.1.20110528-1_i386.deb` could be different file name)
3. Ubuntu Software Center will be opened.
4. Click Install (If the system request to enter your user password fill out for the permissions)
5. Go the setting page `System > Preferences > Input Method Switcher`.
6. Then choose iBus.
7. Download one of the keyboard layout you like to use from [Keyboards](/keyboards).