# Linux System

The Linux operating system comprises several different pieces:

- **Bootloader** -  The software that manages the boot process of your computer. For most users, this will simply be a splash screen that pops up and eventually goes away to boot into the operating system.
Examples of boot loader GRUB & ISOLinux, dos u-boot . Once the post completed, control went to bootloader. Bootloader is stored on the Hard disk.
			Bootloader is responsible for loading the Kernel image and initial Ram disk or the file system into memory.
			Bootloader loads the kernel and the initial ram based file system into memory so it can be used directly by the kernel. 
  		Most of other processes running trace their origin to init
			Init is responsible for keeping the system running and for shutting it down cleanly.

<p align="center">
  <img width="500" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/b212dbf9-f8c6-4f20-96a8-9bc29cba7ee7">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/804d4384-d83a-4c83-ad19-25092dfbcabe">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/1db53431-3f86-4576-9ab3-6dc5979a571c">
</p>

- **Kernel** – This is the one piece of the whole that is actually called ‘Linux’. The kernel is the core of the system and manages the CPU, memory, and peripheral devices. The kernel is the lowest level of the OS. Its the core of operating system. Glue between hardware and application i.e. Linux kernel

<p align="center">
  <img src="https://github.com/mudassirsh/Linux/assets/18271814/30174512-da82-475d-af56-f48abf0ae622">
  <img width="250" height="250" src="https://github.com/mudassirsh/Linux/assets/18271814/6358118b-3263-4596-8303-ea1c8febcb35">
</p>

- **Init system** – This is a sub-system that bootstraps the user space and is charged with controlling daemons. One of the most widely used init systems is systemd, which also happens to be one of the most controversial. It is the init system that manages the boot process, once the initial booting is handed over from the bootloader (i.e., GRUB or GRand Unified Bootloader).
- **Daemons** – These are background services (printing, sound, scheduling, etc.) that either start up during boot or after you log into the desktop.
- **Graphical server** – This is the sub-system that displays the graphics on your monitor. It is commonly referred to as the X server or just X.
- **Desktop environment** – This is the piece that the users actually interact with. There are many desktop environments to choose from (GNOME, Cinnamon, Mate, Pantheon, Enlightenment, KDE, Xfce, etc.). Each desktop environment includes built-in applications (such as file managers, configuration tools, web browsers, and games).
- **Applications** – Desktop environments do not offer the full array of apps. Just like Windows and macOS, Linux offers thousands upon thousands of high-quality software titles that can be easily found and installed. Most modern Linux distributions (more on this below) include App Store-like tools that centralize and simplify application installation. For example, Ubuntu Linux has the Ubuntu Software Center (a rebrand of GNOME Software) which allows you to quickly search among the thousands of apps and install them from one centralized location.


- **Distribution:**		

<p align="center">
  <img width="700" height="600" src="https://github.com/mudassirsh/Linux/assets/18271814/00a51592-2196-4de6-8d54-f02db99541dc">
</p>

- **Service:**			programe that runs as a background process		i.e.	httpd, nfsd, ntpd, ftpd and named
  
<p align="center">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/613906a4-db2e-43e7-b24e-e43f84f841ed">
</p>

- **FileSystem:**    <img align="right" width="275" height="275" src="https://github.com/mudassirsh/Linux/assets/18271814/5f2ec485-0212-43aa-9d61-ac800ffe5951" />
  Method for storing and organizing files in linux. 	i.e. ext3, ext4, FAT, XFS, NTFS and Btrfs		

- **X Window System:**     
                      Provides the standard toolkit and protocol to build graphical user interfaces on nearly all Linux System 		

- **Command line:**		Interface for typing commands on top of the operating system.
- **Shell:**			Command line interpreter that interprets the command line input and instructs the operating system to perform any necessary tasks and command. i.e. bash, tcsh, and zsh
			        Large organizations use commercially supported Distributions from RedHad, Susie and Canonical (Ubuntu) 
                  Linux is a full multitasking multiuser operating system with built-in networking and service processes known as deamons.

- **BIOS:**			Basic Input/Output System. When computer turned on, it runs the self test called POST (power-on self test). Bios software is stored on a ROM chip on the motherboard.


- **File systems supported by Linux:**

<p align="center">
  <img width="420" height="150" src="https://github.com/mudassirsh/Linux/assets/18271814/9b7c1228-8172-4218-a4a8-58180e0aafae">
  <img width="250" height="210" align="right" src="https://github.com/mudassirsh/Linux/assets/18271814/2c97fb00-50c4-4341-b7de-b445f383dcf5">
</p><br><br>


- **Root Directory and file system Hierarchy:**

<p align="center">
  <img width="700" height="550" src="https://github.com/mudassirsh/Linux/assets/18271814/26c0ee5a-49ef-479e-9771-5e2fd4ffcbd0">
</p>
