---
title: Installation on Linux
date: 2019-03-01 17:23:00 +06:30
---

## Quick Install (All Distributions)

The easiest way to install KeyMagic 3 on any Linux distribution:

```bash
curl -fsSL https://thantthet.github.io/keymagic-3/install.sh | bash
```

## Distribution-Specific Installation

### Debian/Ubuntu

1. Add the GPG key:
```bash
curl -fsSL https://thantthet.github.io/keymagic-3/keymagic.gpg | sudo gpg --dearmor -o /usr/share/keyrings/keymagic.gpg
```

2. Add the repository:
```bash
echo "deb [signed-by=/usr/share/keyrings/keymagic.gpg] https://thantthet.github.io/keymagic-3/deb stable main" | \
  sudo tee /etc/apt/sources.list.d/keymagic.list
```

3. Install KeyMagic 3:
```bash
sudo apt update
sudo apt install keymagic3
```

### Fedora/RHEL/CentOS

1. Add the repository:
```bash
sudo curl -fsSL https://thantthet.github.io/keymagic-3/rpm/keymagic.repo \
  -o /etc/yum.repos.d/keymagic.repo
```

2. Install KeyMagic 3:
```bash
sudo dnf install keymagic3
```

## Build from Source

For distributions not covered above, you can build KeyMagic 3 from source:

1. Download the source code from the [KeyMagic 3 releases page](https://github.com/thantthet/keymagic-3/releases)

2. Extract the downloaded archive:
```bash
tar -xzf keymagic-3-*.tar.gz
cd keymagic-3-*
```

3. Navigate to the keymagic-ibus directory:
```bash
cd keymagic-ibus
```

4. Build and install:
```bash
make
sudo make install
```

## Post-Installation

After installation, complete the setup:

1. Restart IBus:
```bash
ibus restart
```

2. Log out and log back in to your session

3. Add KeyMagic in your system input method settings

## System Requirements

### Supported Distributions
- Debian 10 or later
- Ubuntu 20.04 or later  
- Fedora 35 or later
- RHEL 8 or later
- CentOS 8 or later

### Supported Architectures
- amd64 / x86_64
- arm64 / aarch64
