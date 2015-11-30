# Debian-chainsaw-docker
<img src="http://www.clipartreview.com/_images_300/A_man_in_a_hockey_mask_chasing_a_turkey_with_a_chainsaw_110525-224942-343009.jpg">
Debian-chainsaw-docker  USED for CHROOT switch Distro stages, side order of 7-zip, Squashfs tools for unpacking ISO's IE your distro.
- [Debootstrap] (https://wiki.debian.org/Debootstrap)
- p7zip  7z x iso_file.iso
- squashfstools unsquashfs -f -d /media/location1 /media/location2/file.squashfs
- zsync  rsync equiv ftp or http 
- [csync] (https://www.csync.org) rsync equiv ftp or http more Libraires but often wicked fast. 
ie http://somepackage.host.someplace far far away...  > /usr/portage/packages (binaries) 
Else your distro's package dir. 

-"chainsaw" open iso in docker-hub is like an atari joypad and a chainsaw-on a robot arm 3000 miles over. 

https://github.com/gentoo/gentoo-docker-images/tree/master/amd64-hardened/Dockerfile
https://github.com/gentoo/gentoo-docker-images/blob/master/amd64-hardened/build.sh
make Debian or FROM busybox .. 

however light the gentoo Base Stage is so limiting and confining, why not get a fater iso with the tools wanted insted of stringing them together in progresive docker Stages. <img src="http://www.olgasflavorfactory.com/wp-content/uploads/2013/10/Slice-of-Chocolate-Strawberry-Layer-Cake.jpg" height="197" width="248"> yup you can stack containers like a layer cake or weding cake. however doing it in steps for 4 flavor varriants is a royal pest.  also one fine mess. <img src="http://www.nelcoproducts.com/blog/wp-content/uploads/2012/01/tangled-christmas-lights4.jpg" height="197" width="248">
and if a user pulls Cross stream packages from Default and hardened systems that not good. 
<img src="https://media0.giphy.com/media/Vse57fdw0kkLK/200_s.gif" height="197" width="248">

MY Primary Distro [Sabayon] is based upon Gentoo , I also Like [Pentoo]  
however some of my package scripts are more Exotic of the Pen-testing/IT-Security Audit  variety.. 
with sabayon Adding in many of the Pentoo tols is rather trivial, and as a repo its a good place to volentter them. 
ie spikelinux bin repo and or layman. 
however making sure if I upstream a package that it will build easily 
in the stock pentoo Enviorment is my specific use case ,
and or building into a Pentoo chroot, equo smart inflate tarball-name to transmogrify it to work in entropy. 
(entropy works with (wraps) portage binaires however walks though as if it were built on local. and faster) [circleCI](www.circleci.com) one can rig to build packages from docker , keep packages let the Ephemeral nature of the container pass. 
basicly a full fresh choot on docker pull my/beer or other image tag. 

7z x iso_file.iso
mkdir newWorldOrder;mkdir newWorldOrder/pentoo;  <<<--- WGET AN ISO
http://www.pentoo.ch/isos/latest-iso-symlinks/
cd newWorldOrder/pentoo && unsquashfs -f -d /newWorldOrder /newWorldOrder/pentoo/system.squashfs
