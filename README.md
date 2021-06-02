# QEMU-Termux 
Termux QEMU package with SPICE support , includes qemu-system-i386, qemu-system-x86_64
without chroot/proot

# Note : Required Android 7 or more

# How to install this packages ?
1) pkg update && pkg upgrade
2) Download these packages(.deb) from Releases and enable storage permission of termux
3) apt install /sdcard/Download/liborc-0.4.32_aarch64.deb
   
   apt install /sdcard/Download/libspice-server-0.14.91_aarch64.deb
   
   apt install /sdcard/Download/qemu-system-x86-64-4.2_aarch64.deb

# How to use spice with qemu ?
 1) Install aSPICE client from playstore :
  https://play.google.com/store/apps/details?id=com.iiordanov.freeaSPICE
 2) In your qemu command line , remove -vnc and add 
   -spice port=5900,disable-ticketing $@
 3) Now open aspice app and add address as 127.0.0.1 and port 5900
