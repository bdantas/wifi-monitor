# wifi-monitor
Show a system tray icon while wifi is connected

# Purpose
Show wifi icon in system tray while connected; hover over icon for current SSID

# What you need
0. GNU/Linux operating system and this script
1. Suitable icon (provided)
2. **iwconfig** (usually part of *wireless-tools* package) and **netcat**
3. One of: **mktrayicon** (x86_64 binary provided; source code [here](https://github.com/jonhoo/mktrayicon)) or **yad** or **wbar**
4. If you use mktrayicon or yad, you need **gtk3**
5. Any panel with a system tray
6. Check "user variables" at top of script for correctness

# Example installation
```
$ sudo apt install wireless-tools netcat yad
$ cd /tmp
$ wget https://github.com/bdantas/wifi-monitor/archive/master.zip
$ unzip master.zip
$ sudo cp ./wifi-monitor-master/wifi-monitor /usr/local/bin/
$ sudo cp ./wifi-monitor-master/mktrayicon /usr/local/bin/
$ sudo chmod a+x /usr/local/bin/wifi-monitor /usr/local/bin/mktrayicon
$ sudo mkdir -p /usr/share/icons
$ sudo cp ./wifi-monitor-master/wifi.png /usr/share/icons/
```
Note: If your operating system is not Debian-like, adjust the first step

# Usage
Run `wifi-monitor &` at boot.

# Want to ditch your bloated network manager?
Check out https://github.com/bdantas/autowifi
