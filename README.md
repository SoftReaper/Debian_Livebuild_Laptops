# DebianLiveBuildCfg_GA401

Before anything, a big thanks to the r/ZephyrusG14 and r/Debian reddit communities 
for their help, tips, encouragements and even cautions when needed while elaborating this set of tools.

This repos is the compilation of many research and tinkering and i want to thank:
- Armas Spann (ZappeL) (https://lab.retarded.farm/zappel/asus-rog-zephyrus-g14 & https://lab.retarded.farm/zappel/asus-rog-zephyrus-g14/-/wikis/home)
  For it's work on this laptop on arch and gentoo, he paved the way to many GA401 users
- Arch Linux community (https://wiki.archlinux.org/title/ASUS_GA401I)
- KanakShilledar from reddit (https://www.reddit.com/r/ZephyrusG14/comments/lyatm8/guide_to_install_arch_linux_on_zephyrus_g14/)
  for its "mic-mute" key code (i know if found it somewhere in arch wiki, but can't find it anymore, will edit this one if i find it)
- Luke Jones and Armas Spann for asusctl 
  
Hooks have been commented as much as possible to ease read and modifications. 
Some others (which require software agreements, like steam) can be found in my gists

The kernel used by this script can be found here:
https://github.com/SoftReaper/linux-image-5.16-znver2
(build it or get the binary version if you trust me enought, but i suggest to read a bit anyway)

the provided asusctl package has been compiled from this code source:
https://gitlab.com/c6248/asusctl (forked from https://gitlab.com/asus-linux/asusctl)
please don't bother devs with my package, debian is not officially supported by their project and this one stills in testing phase
for any debian relate issues, please contact me here: https://gitlab.com/c6248/asusctl/-/issues

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
