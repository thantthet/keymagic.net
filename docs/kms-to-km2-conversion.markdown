---
title: KMS to KM2 Conversion Guide
date: 2025-01-07 12:00:00 +06:30
---

# Converting KMS to KM2 Using KeyMagic Configurator

## Overview

KeyMagic keyboards come in two formats:

- **KMS Files** (.kms): Text-based keyboard scripts that define typing rules
- **KM2 Files** (.km2): Compiled binary keyboards that KeyMagic uses

This guide shows how to convert KMS files to KM2 format using the KeyMagic Configurator.

## Steps to Convert

### Step 1: Open KeyMagic Configurator

Launch KeyMagic 3 Configurator from:
- **Windows**: Start Menu or system tray
- **macOS**: Applications folder or Launchpad  
- **Linux**: Application menu

### Step 2: Go to Create Keyboard

Click **Create Keyboard** in the Developer Tools section (bottom of the left sidebar).

![Create Keyboard Interface](/assets/screenshots/macos-kms-converter.png)

### Step 3: Choose Your KMS File

Click the **Choose KMS File** button to browse and select your `.kms` script file.

Once selected:
- The file name will appear below the button
- The converter will validate the file
- The action buttons will become enabled

### Step 4: Select an Action

After selecting your KMS file, choose one of two options:

#### Convert to KM2
- **Purpose**: Creates a KM2 file and saves it to your chosen location
- **Steps**:
  1. Click **Convert to KM2**
  2. Choose where to save the file
  3. The compiled KM2 file will be saved
- **Use when**: You want to share the keyboard or keep the file for later

#### Convert & Import  
- **Purpose**: Creates a KM2 file and immediately adds it to KeyMagic
- **Steps**:
  1. Click **Convert & Import**
  2. The keyboard is compiled and imported automatically
  3. It appears in your Keyboards list ready to use
- **Use when**: You want to start using the keyboard right away

## Understanding the Results

### Successful Conversion

When conversion succeeds:
- ✅ A success message appears
- The KM2 file is created
- For "Convert & Import": The keyboard appears in your Keyboards list

### Conversion Errors

If conversion fails, you'll see:
- ❌ An error message with details
- The line number where the error occurred  
- A description of what went wrong

Common errors:
- **Syntax error**: Check for typos in your KMS file
- **Missing file**: Ensure referenced icons exist
- **Invalid Unicode**: Verify character codes are correct

## What Happens During Conversion

The converter:
1. Reads your KMS text file
2. Validates all syntax and rules
3. Compiles rules into optimized binary format
4. Packages everything into a KM2 file
5. Reports success or any errors found

## Platform Note

The converter works identically on Windows, macOS, and Linux. KM2 files created on any platform work on all others.

## Quick Tips

- Keep your original KMS files - you'll need them to make changes
- The converter shows clear error messages if something goes wrong
- Use "Convert & Import" for quick testing of your keyboards
- Use "Convert to KM2" when preparing keyboards to share

## Next Steps

After converting:
- **Test your keyboard**: Switch to it and try typing
- **Check the Keyboards page**: Your imported keyboards appear there
- **Make changes**: Edit the KMS file and convert again if needed

## Learning to Write KMS Files

If you're interested in creating or modifying KMS keyboard scripts:
- **Example keyboards**: Browse existing KMS files at [github.com/thantthet/keymagic-keyboards](https://github.com/thantthet/keymagic-keyboards)
- **Learn by example**: Study how existing keyboards implement their rules
- **Start simple**: Modify an existing keyboard before creating one from scratch