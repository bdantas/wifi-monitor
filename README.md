# wifi-monitor
Show a system tray icon while wifi is connected

# Purpose
Show wifi icon in system tray while connected; hover over icon for current SSID

# Usage
Run `wifi-monitor &` at boot

# What you need
0. GNU/Linux operating system and this script
1. Suitable icon (provided)
2. **netcat** and **wireless-tools** (provides iwconfig) installed
3. **mktrayicon** utility somewhere in your PATH (x86_64 binary provided; source code [here](https://github.com/jonhoo/mktrayicon))
4. Check "user variables" at top of script for correctness

# Want to ditch your bloated network manager?
Check out https://github.com/bdantas/autowifi
