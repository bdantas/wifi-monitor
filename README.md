# wifi-monitor
Show a system tray icon while wifi is connected

# Purpose
Show wifi icon in system tray while connected; hover over icon for current SSID

# What you need
0. GNU/Linux operating system and this script
1. Suitable icon (provided)
2. **iwconfig** (usually part of *wireless-tools* package) and **netcat**
3. **mktrayicon** (x86_64 binary provided; source code [here](https://github.com/jonhoo/mktrayicon)) or **yad** or **wbar**
4. If you go with mktrayicon or yad, you'll also need **gtk3**
5. Any panel with a system tray
6. Check "user variables" at top of script for correctness

# Example installation
```
$ sudo apt install wireless-tools netcat yad
$ cd /tmp
$ wget https://github.com/bdantas/wifi-monitor/archive/master.zip
$ unzip master.zip
$ sudo cp ./wifi-monitor-master/wifi-monitor /usr/local/bin/
$ sudo chmod a+x /usr/local/bin/wifi-monitor
$ sudo mkdir -p /usr/local/share/icons
$ sudo cp ./wifi-monitor-master/wifi.png /usr/local/share/icons/
```
Note: If your operating system is not Debian-like, adjust the first step

# Usage
Run `wifi-monitor &` at boot.

# Want to ditch your bloated network manager?
Check out https://github.com/bdantas/autowifi
