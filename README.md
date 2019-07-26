# kernel-native
Provides Ubuntu/Debian users with the latest linux kernel. (https://github.com/torvalds/linux)

THE LATEST KERNEL MIGHT NOT BE FULLY COMPATIBLE WITH EXISTING PACKAGES, USE THIS WITH CAUSION.

# Supported Distribution
Ubuntu 18.04, 16.04 x64

# Usage
## Ubuntu
* Install:
	
	Add the repository:

		sudo add-apt-repository ppa:franklynchen/kernel
		sudo apt-get update

	Install the kernel:

		sudo apt install linux-image-native-desktop

	After a successful installation, the new kernel will become the default boot entry of GRUB in most cases since it is newer than the official Ubuntu kernel. 

	Reboot your system, and check the kernel version by running `uname -a`.

* Recovery:

	Under default setting, there will be a new entry in GRUB. If the new kernel breaks your system, just boot from the official Ubuntu kernel in the GRUB entry "Advanced Option for Ubuntu XX.YY" where XX.YY is your Ubuntu version.

* Remove:
	
	Remove the repository:

		sudo add-apt-repository --remove ppa:franklynchen/kernel

	Remove the installed package:

		sudo apt remove linux-image-native-desktop


# Packages
* linux-image-native-desktop: latest stable kernel for general desktop usage

	With configurations similar to Arch Linux.


[NOTE]: The PPA is still under construction and more version will be announced in the future.
