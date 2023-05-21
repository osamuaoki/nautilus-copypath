# nautilus-copypath
A small Nautilus extension for quickly copying file/Samba paths.

![Screenshot](https://github.com/ronen25/nautilus-copypath/blob/master/screenshots/screenshot.png)

## General
This repository contains two plugins for Nautilus:
1. `nautilus-copypath` - Quickly copy file/folder paths.
2. `nautilus-copywinpath` - Quickly copy Samba file/folder paths, converting them to Windows
paths on-the-fly.

You may choose to install both of the plugins, or only one of them, as you see fit.

## Installation from Source
To successfully install the plugin you need:
1. Python >= 3.2 (tested on Python 3.11.2)
2. GNOME >= 43 (tested on Debian 12/Bookworm )
3. GObject Python bindings (development libraries)
4. nautilus (tested on 43.2-1)
4. python3-nautilus (tested on 4.0-1+b1)

### Installing the Dependencies
Simply copy and paste the appropriate command for your distro:

| Distro | Command|
|--------|--------|
| Ubuntu | ``` $ sudo apt-get install python3-nautilus python3-gi ``` |
| Debian | ``` $ sudo apt-get install python3-nautilus python3-gi ``` |

<!--
| Fedora | ``` $ sudo dnf install nautilus-python python3-gobject ``` |
| Arch Linux | ``` $ sudo pacman -S python-gobject python-nautilus ``` |
-->

### Installing the Extension
Clone the repository:

```
git clone -b nautilus-43 https://github.com/osamuaoki/nautilus-copypath
```
<!--
```
git clone https://github.com/ronen25/nautilus-copypath
```
-->

Copy the file/s to the appropriate folder, creating it if needed:
```
mkdir ~/.local/share/nautilus-python
mkdir ~/.local/share/nautilus-python/extensions
cp nautilus-copypath.py ~/.local/share/nautilus-python/extensions/
cp nautilus-copywinpath.py ~/.local/share/nautilus-python/extensions/
```

Restart Nautilus and the extension will be available. If that doesn't work try logging out and back in.
