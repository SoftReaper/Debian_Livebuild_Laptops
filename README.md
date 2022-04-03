# Debian_Livebuild_Laptops for DELL Latitude 3550 (haswell i3)
  
Hooks have been commented as much as possible to ease read and modifications. 
Some others (which require software agreements, like steam) can be found in my gists

The kernel used by this script can be found here:
https://github.com/SoftReaper/linux-image-customized/tree/Latitude-3550
(build it or get the binary version if you trust me enought, but i suggest to read a bit anyway)

To use:

install live-build:
apt-get install live-build live-manual live-tools

clone this git and navigate to it with your favorite terminal emulator/SSH/everything you want when theres' a blinking cursor

copy basic scripts:

cp /usr/share/doc/live-build/examples/auto/build auto/build

cp /usr/share/doc/live-build/examples/auto/clean auto/clean

load config file:
lb config

and build (as root)
sudo lb build
