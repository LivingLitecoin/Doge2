
Debian
====================
This directory contains files used to package dogecoin2d/dogecoin2-qt
for Debian-based Linux systems. If you compile dogecoin2d/dogecoin2-qt yourself, there are some useful files here.

## dogecoin2: URI support ##


dogecoin2-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install dogecoin2-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your dogecoin2-qt binary to `/usr/bin`
and the `../../share/pixmaps/dogecoin2128.png` to `/usr/share/pixmaps`

dogecoin2-qt.protocol (KDE)

