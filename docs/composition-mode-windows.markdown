---
title: Composition Mode Guide - Windows
date: 2025-01-07 12:00:00 +06:30
---

# Configuring Composition Mode in Windows

## Overview

KeyMagic for Windows offers two text input modes:

- **Direct Mode** (default): Text is inserted immediately into the application as you type
- **Composition Mode**: Text appears with an underline while typing and is committed when complete

**Important**: Both modes produce exactly the same final text output. The composing string (whether shown underlined or not) is what will be committed. The only difference is how the text is displayed during typing - this is purely for application compatibility.

## When to Use Composition Mode

Consider enabling composition mode for applications that:
- Have compatibility issues with direct text input
- Don't handle immediate text insertion/deletion properly
- Support IME composition windows natively (like Microsoft Teams and Excel)
- Experience text input problems, cursor jumping, or text duplication in direct mode

## How to Configure Composition Mode

### Step 1: Open KeyMagic Configurator

Launch the KeyMagic 3 Configurator from your Start Menu or system tray.

### Step 2: Navigate to Settings

Click on **Settings** in the left sidebar.

### Step 3: Find Composition Mode Section

Scroll down to the **Composition Mode** section.

![Composition Mode Settings](/assets/screenshots/windows-composition-mode-apps.png)

### Step 4: Add Applications

1. Click the **Add Application** button
2. The application selection dialog will appear

![Application Selection Dialog](/assets/screenshots/windows-composition-mode-selection.png)

### Step 5: Select or Enter Application

You have two options:

#### Option A: Select from List
- Browse through the list of currently running applications
- Click on the application you want to add
- The executable name (e.g., `ms-teams.exe`) will be shown

#### Option B: Manual Entry
- If the application isn't running or not in the list
- Enter the executable name manually in the text field
- Use the format: `applicationname.exe`
- Common examples:
  - `ms-teams.exe` - Microsoft Teams
  - `excel.exe` - Microsoft Excel
  - `winword.exe` - Microsoft Word
  - `notepad.exe` - Notepad
  - `powershell.exe` - PowerShell

### Step 6: Confirm Selection

Click **Add Application** to add the application to the composition mode list.

### Step 7: Managing Applications

- To remove an application from composition mode, click the **Remove** button next to its name
- Changes take effect immediately for new text input sessions

## Understanding the Behavior

### Applications WITH Composition Mode:
- Text appears with an underline while typing
- The underlined text shows the exact composing string that will be committed
- Text is committed when the composition completes (e.g., when forming complete words/syllables)
- Better compatibility with applications that expect IME composition behavior

### Applications WITHOUT Composition Mode (Direct Mode):
- Text is inserted directly without underline
- The same composing string is built internally and inserted character by character
- May appear more responsive but can cause issues in some applications
- Default behavior for most Windows applications

## Tips

1. **Testing**: After adding an application, switch to it and test typing to ensure it works as expected
2. **Executable Names**: You can find an application's executable name in Task Manager (Details tab)
3. **System Applications**: Some system applications may require administrator privileges to modify their input behavior
4. **Restart**: Some applications may need to be restarted for changes to take full effect

## Troubleshooting

If composition mode isn't working as expected:

1. Verify the correct executable name is added
2. Restart the application
3. Check if the application supports standard Windows IME protocols
4. Try toggling KeyMagic off and on using Win+Space

## Default Applications for Composition Mode

By default, KeyMagic may include certain applications in composition mode that are known to work better with this mode, such as:
- Microsoft Teams (`ms-teams.exe`)
- Microsoft Excel (`excel.exe`)

You can always modify this list based on your preferences and needs.