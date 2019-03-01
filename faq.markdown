---
title: FAQ
date: 2019-03-01 17:43:00 +06:30
---

## Mac OS X

### I cannot turn off keymagic at login window

keymagic has no control of switching on/off input methods on macOS.

This likely to be a bug of macOS. (Note: **Issue solved in macOS Sierra**)

You can at least avoid this issue by selecting `System Preferences > Users & Group > Login Options > Show Input menu in login window`. (but not always work)

### How to install keyboard layouts?

On macOS, you can install keyboard layouts by copying `km2` file into `~/.keymagic` (Please create directory if not exists)

### keymagic keyboard menu is empty and keymagic won't work

This is known bug and still figuring out for a fix. In the meantime, you can kill keymagic process from Activity Monitor and try to type again.

### I don't like notifications being shown up when I switch keyboards

Go to System `Preferences > Notifications > keymagic`. Set alert style to None.

---

## Windows

### I get runtime error when starting keymagic

This could be because of missing dependencies. Please refer to notes written at downloads page.