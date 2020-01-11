---
title: Manual Installation on Linux
date: 2019-03-01 17:23:00 +06:30
---
# ibus-keymagic 
## Linux Keymagic with iBus Engine 
- Debian, Ubuntu, Mint, Kali and other Debian base, Arch Linxu, Redhat, CentOS, Fedora and other RPM base Linux Disro . See Installing to start using KeyMagic today!

You may use one of the following methods to install KeyMagic on Ubuntu. These may also work for other Debian based Linux OSes. Thanks to Ko Ko Ye and Ubuntu-MM for providing packages.

### Ubuntu - Installing from kokoye2007 PPA
```
sudo add-apt-repository -y ppa:kokoye2007/ppa
sudo apt-get update
sudo apt-get install ibus-keymagic
```
## Manual Install Keymagic 

first, download your Linux Distro base DEB, RPM, or tar.gz.xz file [here](https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/)

### Debian Base

first, download your Linux Distro base DEB, RPM, or tar.gz.xz file [DEB here](https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/DEBIAN_Ubuntu_Mint_Pinguy_Kali_Deb/)

- Debian base
 -- Ubuntu, Mate, Kali, Debian, Pinguy, Mint, etc

```
sudo dpkg -i ibus-keymagic*.deb

```


### Redhat Base

first, download your Linux Distro base DEB, RPM, or tar.gz.xz file 

[Fedora fc-x86-64](https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/Redhat_Fedora_CentOS_RPM/Fedora/)

[CentOS el7 x86-64](https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/Redhat_Fedora_CentOS_RPM/CentOS/)

- Redhat base
-- Redhat, Fedora, CentOS, etc

```
sudo -ivh ibus-keymagic*.rpm

```

### Arch Linux

[ibus-keymagic-x86_64.pkg.tar.xz](https://sourceforge.net/projects/ubuntumm/files/ibus-keymagic/ARCH_Linux/ibus-keymagic-x86_64.pkg.tar.xz/download)

```
 pacman -U ibus-keymagic*.xz

```

### Keyboard Layout 

- Download Keyboard Layout [here](https://github.com/thantthet/keymagic-keyboards)
-- Example KhmerNiDA, Myanmar, Mon, Shan, Malay 

Add and Configure

```
mkdir ~/.keymagic
copy .km2 ~/.keymagic
ibus-daemon -rdx
ibus-setup &
ibus-daemon -rdx
```

```
#if using gnome ?
gnome-control-center region
```
> Keymagic is under the English Group
> Add your Additional Keyboard

Logout and try your keyboard

[Ko Ko Ye](https://ubuntu-mm.net)
[Thant Thet Khin Zaw](https://keymagic.net)
