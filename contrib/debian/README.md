
Debian
====================
This directory contains files used to package sixcoind/sixcoin-qt
for Debian-based Linux systems. If you compile sixcoind/sixcoin-qt yourself, there are some useful files here.

## sixcoin: URI support ##


sixcoin-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install sixcoin-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your sixcoin-qt binary to `/usr/bin`
and the `../../share/pixmaps/sixcoin128.png` to `/usr/share/pixmaps`

sixcoin-qt.protocol (KDE)

