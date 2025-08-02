---
title: Installation on Ubuntu
date: 2019-03-01 17:23:00 +06:30
---

## Quick Install

The easiest way to install KeyMagic 3 on Ubuntu:

```bash
curl -fsSL https://thantthet.github.io/keymagic-3/install.sh | bash
```

## Manual Installation

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

## Post-Installation

- Restart IBus: `ibus restart`
- Log out and log back in
- Add KeyMagic in your system input method settings

## System Requirements

- Ubuntu 20.04 or later
- Debian 10 or later
- Supported architectures: amd64, arm64
