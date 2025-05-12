# QEMU-Termux 
Termux QEMU package with SPICE support without chroot/proot.

Current Release QEMU Version : 4.2

# How to install this packages ?
1) pkg update && pkg upgrade
2) Download these packages(.deb) from Releases and enable storage permission of termux
3) apt install path-to-file.deb
 
# How to use spice with qemu ?
1) Install aSPICE free apk from here :
  https://github.com/iiordanov/remote-desktop-clients/releases
 2) In command line , remove -vnc and add 
   -spice port=5900,disable-ticketing=on
 3) Now open aspice app and add address as 127.0.0.1 and port 5900
