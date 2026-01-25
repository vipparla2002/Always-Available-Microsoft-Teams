# Status-Always-Active-Microsoft-Teams

# AHK Clicker Control - Documentation

## Quick Start (For Beginners)

1. Download the ZIP file from GitHub.
2. Extract the file to any folder.
3. Double-click the EXE file to run it.
4. If Windows shows a warning, click 'More info' and choose 'Run anyway'.

## Overview
This AutoHotkey v2 script provides a GUI-based mouse click automation tool, primarily designed to automate clicking in Microsoft Teams. It features a simple interface to start and stop the clicker, set the click interval, and monitor click activity.

## Features
- Always-on-top GUI for easy access
- Start and Stop buttons to control the clicker
- **Kill Script** button to immediately exit the script
- Clicking **Stop** halts the clicker but keeps the script running
- Clicking the **X** (close) button hides the GUI (script keeps running)
- Input field to set the click interval (in milliseconds)
- Displays status, elapsed time, start/stop times, and click count
- Tray menu for quick access to show the GUI or exit the script
- Hotkeys:
  - `F8`: Toggle start/stop
  - `Ctrl+Shift+G`: Show the GUI
 
<img width="613" height="540" alt="image" src="https://github.com/user-attachments/assets/7fa06f70-cae7-4130-9241-58fc1d0ae3ea" />

## Usage
1. Run the script with AutoHotkey v2.
2. Use the GUI to set your desired click interval (minimum 10,000 ms).
3. Click "Start" to begin automated clicking in Microsoft Teams.
4. Click **Stop** to halt the clicker (the script remains running and the GUI stays open).
5. Click **Kill Script** to immediately terminate the script if needed.
6. Click the **X** (close) button to hide the GUI (the script continues running in the background).
7. Use the tray icon or hotkeys for quick access.

<img width="421" height="509" alt="image" src="https://github.com/user-attachments/assets/6251d001-cd3e-4f52-8de8-0b52f0c7d8fb" />
in the above image, a click would be made every 250000ms/250s/4m.10s

<img width="375" height="492" alt="image" src="https://github.com/user-attachments/assets/0dbedab7-c30f-4d55-a191-22e57417fb0e" />
in this image, a click would be made every 11000ms/11s


## How It Works
- The script checks for a running Microsoft Teams window. If found, it maximizes and activates the window, then clicks at a specific location.
- If Teams is not running, it attempts to launch it and waits for the window to appear.
- The click count and elapsed time are updated in real time on the GUI.

## Customization
- You can change the click coordinates or target window by editing the `ClickLoop` function.
- The minimum interval is enforced to prevent excessive clicking that could make the system unresponsive.

## Requirements
- AutoHotkey v2.0 or later ([Download here](https://www.autohotkey.com/download/ahk-v2.exe))
- Microsoft Teams (if using the default automation target) ([Download here](https://statics.teams.cdn.office.net/production-windows-x86/lkg/MSTeamsSetup.exe))

## Notes
- The script is designed to be safe by enforcing a minimum interval.
- The GUI can be hidden instead of closed, allowing the script to keep running in the background (use the tray icon or hotkey to show it again).
- The **Kill Script** button provides a quick way to exit the script if needed.
- The **Stop** button halts the clicker but does not terminate the script.
- The **X** button only hides the GUI; it does not stop or terminate the script.

---

For further customization or issues, edit the script or contact the author.
