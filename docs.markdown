---
title: Documentation
date: 2025-01-07 12:00:00 +06:30
---

# KeyMagic Documentation

Welcome to the KeyMagic documentation. Here you'll find detailed guides on configuring and using KeyMagic's features across different platforms.

## Platform-Specific Guides

### Windows

#### [Composition Mode Configuration Guide](/docs/composition-mode-windows)
Learn how to configure composition mode for Windows applications that work better with IME-style text input. This guide covers when and how to enable composition mode for specific applications like Microsoft Teams and Excel.

### macOS

#### [Direct Mode Configuration Guide](/docs/direct-mode-macos)
Understand how to configure direct mode for macOS applications. While most macOS apps work best with composition mode, some applications can benefit from direct text input. This guide explains the differences and how to configure apps for direct mode.

### Developer Tools

#### [KMS to KM2 Conversion Guide](/docs/kms-to-km2-conversion)
Learn how to convert KeyMagic Script (KMS) files to compiled KM2 keyboard files using the KeyMagic Configurator. This guide covers the conversion process, troubleshooting common errors, and tips for keyboard development.

## Key Concepts

### Input Modes

KeyMagic supports two text input modes across platforms:

- **Direct Mode**: Text is inserted immediately into the application as you type
- **Composition Mode**: Text appears with an underline while typing and is committed when complete

Both modes produce exactly the same final text output. The difference is purely in how the text is displayed during typing, which affects application compatibility.

### Platform Differences

- **Windows**: Direct mode is the default, with composition mode available for apps that need it
- **macOS**: Composition mode is the default, as most macOS apps don't support direct mode properly

## Need Help?

If you have questions or encounter issues:

1. Check the platform-specific guides above
2. Visit our [FAQ](/faq) section
3. [Report an issue](/report) on our GitHub repository