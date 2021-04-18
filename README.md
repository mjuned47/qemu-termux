# QEMU-Termux
Termux QEMU package with SPICE support , includes qemu-system-aarch64, qemu-system-i386, qemu-system-x86_64

Only For Android ARM64

# Note : Before installing these, make sure you have removed qemu provided by termux if installed

# How to install this packages ?
1) pkg update && pkg upgrade
2) Download these packages(.deb) and enable storage permission of termux
3) apt install /sdcard/Download/liborc_arm64.deb
   
   apt install /sdcard/Download/libspice-server_arm64.deb
   
   apt install /sdcard/Download/qemu-system-spice_arm64.deb

# How to use spice with qemu ?
 1) Install aSPICE client from playstore :
  https://play.google.com/store/apps/details?id=com.iiordanov.freeaSPICE
 2) In your qemu command line , remove -vnc and add 
   -spice port=5900,disable-ticketing $@
 3) Now open aspice app and add address as 127.0.0.1 and port 5900
