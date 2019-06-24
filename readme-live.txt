Linux-live-slack-debian contains two folders, one for Slackware 142/current and one for Debian Stretch/Buster.

If you're wanting to remaster or build your own Slackware based distro you will need this kit plus a aufs-patched kernel, available in Slacker/Live Kernel folder. Additionally you can get aufs-patched kernel sources from https://xanmod.org/

If you're wanting to remaster or build your own Debian based distro you will need this kit plus a aufs-patched kernel. In Debian you can do this simply by adding aufs-dkms and aufs-utils from synaptic package manager or add the Xanmod.org repositories to your
apt list and install through synaptic.

YOU MUST EDIT! 
Files that must be edited by you for name of your distro/kernel etc are

linux-live-slack/bootfiles/isolinux/isolinux.cfg
linux-live-slack/bootfiles/syslinux/syslinux.cfg
linux-live-slack/config
linux-live-slack/build
linux-live-slack/initramfs/init

Same goes for the Debian version!

After installing your kernel, rebooting, editing the configs you just run the build script with
./build

That's it!


