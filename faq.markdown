---
title: FAQ
date: 2019-03-01 17:43:00 +06:30
---

## Mac OS X <i class="fab fa-apple"></i>

### I cannot turn off KeyMagic at login window (Note: **Issue solved in macOS Sierra**)

KeyMagic has no control of switching on/off input methods on macOS. This likely to be a bug of macOS itself.

You can at least avoid this issue by selecting `System Preferences > Users & Group > Login Options > Show Input menu in login window`. (but not always work)

### How to install keyboard layouts?

On macOS, you can install keyboard layouts by copying `km2` file into `~/.keymagic` (Please create directory if not exists)

### KeyMagic keyboard menu is empty and KeyMagic won't work

This is known bug and still figuring out for a fix. In the meantime, you can kill KeyMagic process from Activity Monitor and try to type again.

### I don't like notifications being shown up when I switch keyboards

Go to System `Preferences > Notifications > KeyMagic`. Set alert style to None.

---

## Windows <i class="fab fa-windows"></i>

### I get runtime error when starting KeyMagic

This could be because of missing dependencies. Please refer to notes written at downloads page.