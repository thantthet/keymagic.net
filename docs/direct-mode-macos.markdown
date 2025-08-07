---
title: Direct Mode Guide - macOS
date: 2025-01-07 12:00:00 +06:30
---

# Configuring Direct Mode in macOS

## Overview

KeyMagic for macOS offers two text input modes:

- **Composition Mode** (default): Text appears with an underline while typing and is committed when complete
- **Direct Mode**: Text is inserted immediately into the application as you type

**Important**: Both modes produce exactly the same final text output. The composing string (whether shown underlined or not) is what will be committed. The only difference is how the text is displayed during typing. Note that most macOS applications don't support direct mode properly, so this option should only be used with applications known to work well with it.

## When to Use Direct Mode

Most macOS applications don't properly support direct mode due to how they handle text input. Only enable direct mode for applications that are known to work well with it:
- Applications tested and verified to handle direct text insertion correctly
- Apps that have issues with composition mode (rare)
- Applications included in the default list below (known to work)
- When you've tested an app and confirmed it works properly with direct mode

**Warning**: Enabling direct mode for untested applications may result in incorrect text input, missing characters, or other issues.

## How to Configure Direct Mode

### Step 1: Open KeyMagic Configurator

Launch the KeyMagic 3 Configurator from your Applications folder or Launchpad.

### Step 2: Navigate to Settings

Click on **Settings** in the left sidebar.

### Step 3: Find Direct Mode Section

Look for the **Direct Mode App Bundles** section.

![Direct Mode Settings](/assets/screenshots/macos-direct-mode-apps.png)

### Step 4: Add Applications

1. Click the **Add App Bundle** button
2. The application selection dialog will appear

![Application Selection Dialog](/assets/screenshots/macos-direct-mode-app-selection.png)

### Step 5: Select or Enter Application

You have two options:

#### Option A: Select from List
- Browse through the list of installed applications
- Click on the application you want to add
- The bundle identifier (e.g., `com.apple.Safari`) will be shown below the app name
- Use the search bar to quickly find applications

#### Option B: Manual Entry
- If the application isn't in the list
- Enter the bundle identifier manually in the text field
- Use the format: `com.company.AppName`
- Common examples:
  - `com.apple.Safari` - Safari
  - `com.google.Chrome` - Google Chrome
  - `com.apple.TextEdit` - TextEdit
  - `com.microsoft.Word` - Microsoft Word
  - `com.apple.finder` - Finder
  - `ru.keepcoder.Telegram` - Telegram
  - `com.tinyspeck.slackmacgap` - Slack

### Step 6: Confirm Selection

Click **Add Application** to add the application to the direct mode list.

### Step 7: Managing Applications

- To remove an application from direct mode, click the **Remove** button next to its bundle ID
- Changes take effect when you switch to the application

## Understanding the Behavior

### Applications WITH Direct Mode:
- Text is inserted directly without underline
- The same composing string is built internally and inserted character by character
- Only works properly with applications that can handle this approach
- May provide faster visual feedback when it works correctly

### Applications WITHOUT Direct Mode (Composition Mode):
- Text appears with an underline while typing
- The underlined text shows the exact composing string that will be committed
- Text is committed when the composition completes (e.g., when forming complete words/syllables)
- Default behavior and recommended for most macOS applications
- Standard macOS text input experience that works reliably

## Finding Bundle Identifiers

If you need to manually find an application's bundle identifier:

1. **Using Terminal**:
   ```bash
   osascript -e 'id of app "Application Name"'
   ```
   Example: `osascript -e 'id of app "Safari"'` returns `com.apple.Safari`

2. **Using Finder**:
   - Right-click the application in Finder
   - Select "Show Package Contents"
   - Open `Contents/Info.plist`
   - Look for `CFBundleIdentifier`

3. **From the Running App**:
   ```bash
   ps aux | grep "Application Name"
   ```

## Tips

1. **Testing**: Always test an application thoroughly before keeping it in direct mode
2. **Start with Defaults**: Stick to the default list unless you have specific needs
3. **Restart Not Required**: Changes take effect immediately when you focus the application
4. **If Issues Occur**: Remove the application from direct mode immediately if you experience input problems

## Default Applications for Direct Mode

KeyMagic includes a default list of applications that have been tested and verified to work correctly with direct mode:

- **System Apps**: Spotlight, Finder, Dictionary - Apple's system apps handle direct mode properly
- **Text Editors**: TextEdit - Works well with direct text insertion
- **Office Apps**: Microsoft Word - Has proper text handling for direct mode
- **Browsers**: Safari, Chrome - Modern browsers support direct input correctly
- **Communication**: Telegram, WeChat, Slack - These apps handle direct mode without issues
- **Development**: Xcode - Apple's IDE supports direct mode
- **Others**: Zoom, App Store - Verified to work with direct mode

**Important**: This list contains only applications that have been tested and confirmed to work properly with direct mode. Adding untested applications may cause input issues.

## Troubleshooting

If direct mode causes issues:

1. **Remove the application from direct mode immediately** - it likely doesn't support it
2. Verify you're using the correct bundle identifier
3. Make sure KeyMagic is enabled in System Preferences > Keyboard > Input Sources
4. Try switching away from and back to the application
5. Most importantly: **Most macOS apps don't support direct mode** - when in doubt, use composition mode

## Special Considerations

### Web Browsers
Web browsers may behave differently depending on the website. The direct mode setting applies to the entire browser, but some web applications may have their own text handling.

### Terminal Applications
Terminal and command-line applications typically work better with direct mode as they expect immediate character input.

### Microsoft Office
Microsoft Office applications have their own text composition system and generally work better with direct mode enabled.