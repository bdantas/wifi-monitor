# wifi-monitor
Show an icon while wifi is connected

# Purpose
Simple shell script for GNU/Linux that runs in the background, showing an icon when there is a wireless internet connection and hiding the icon when there is none. Hovering over the icon shows the current SSID (wireless network name).

# Usage
Run `$ wifi-monitor &` at boot or at any other time to launch the script, which will run in the background, periodically check for an internet connection, and show or hide a user-defined icon as appropriate. A suitable icon is provided.

The only adaptations you need to make (to the top of the script) are:
1. Make sure the wireless interface name is correct for your hardware
2. Make sure the path to the icon is correct
3. Choose whether you want the icon to appear in your systray (most users) or in your wbar

# Dependencies
- GNU/Linux OS with BusyBox or coreutils userland
- Required for all: **curl** and **wireless-tools** (provides iwconfig)
- Required (for system tray icon only): **yad**

# Want to ditch your bloated network manager?
Check out my *autowifi*
