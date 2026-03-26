# 🛠 Setup Guide

### 1. Required Integrations (HACS)
Before pushing the YAML, ensure the following are installed via the Home Assistant Community Store:
1. **Button Card:** Used for almost every UI element.
2. **Layout Card:** Handles the OS 9 Grid system.
3. **Stack-In-Card:** Keeps the Control Strip looking like one piece of hardware.
4. **Card Mod:** Critical for overriding theme colors and forcing the "Yellow" sticky note.

### 2. Required Helpers
Go to **Settings > Devices > Helpers** and create:
- **Type:** Toggle (Input Boolean)
- **Name:** `macos_notepad`
- **ID:** `input_boolean.macos_notepad`

### 3. Theme Recommendations
For the most authentic experience, use the **Default Home Assistant Theme** or a light theme. The dashboard code includes `!important` CSS flags to ignore "Dark Mode" where it would break the Platinum aesthetic.