
Debian
====================
This directory contains files used to package taskevad/taskeva-qt
for Debian-based Linux systems. If you compile taskevad/taskeva-qt yourself, there are some useful files here.

## taskeva: URI support ##


taskeva-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install taskeva-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your taskevaqt binary to `/usr/bin`
and the `../../share/pixmaps/taskeva128.png` to `/usr/share/pixmaps`

taskeva-qt.protocol (KDE)

