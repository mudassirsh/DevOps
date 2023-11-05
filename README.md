<<<<<<< HEAD
# Linux System


- **Kernel:**			is the core of operating system. Glue between hardware and application i.e. Linux kernel	

<p align="center">
  <img src="https://github.com/mudassirsh/Linux/assets/18271814/30174512-da82-475d-af56-f48abf0ae622">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/6358118b-3263-4596-8303-ea1c8febcb35">
</p>

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


- **Desktop Env:**		GUI on the top of operating system.			GNOME, KDE, Xfce and Fluxbox	are the examples of desktop environments.
- **Command line:**		Interface for typing commands on top of the operating system.
- **Shell:**			Command line interpreter that interprets the command line input and instructs the operating system to perform any necessary tasks and command. i.e. bash, tcsh, and zsh
			        Large organizations use commercially supported Distributions from RedHad, Susie and Canonical (Ubuntu) 
                  Linux is a full multitasking multiuser operating system with built-in networking and service processes known as deamons.



- **BIOS:**			Basic Input/Output System. When computer turned on, it runs the self test called POST (power-on self test). Bios software is stored on a ROM chip on the motherboard.

- **BootLoader:**		That boots the operating syste.  Examples of boot loader GRUB & ISOLinux, dos u-boot . Once the post completed, control went to bootloader. Bootloader is stored on the Hard disk.
			Bootloader is responsible for loading the Kernel image and initial Ram disk or the file system into memory.
			Bootloader loads the kernel and the initial ram based file system into memory so it can be used directly by the kernel. 
  		Most of other processes running trace their origin to init
			Init is responsible for keeping the system running and for shutting it down cleanly.


<p align="center">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/b212dbf9-f8c6-4f20-96a8-9bc29cba7ee7">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/804d4384-d83a-4c83-ad19-25092dfbcabe">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/1db53431-3f86-4576-9ab3-6dc5979a571c">
</p>


- **File systems supported by Linux:**

<p align="center">
  <img width="700" height="250" src="https://github.com/mudassirsh/Linux/assets/18271814/9b7c1228-8172-4218-a4a8-58180e0aafae">
  <img width="250" height="250" align="right" src="https://github.com/mudassirsh/Linux/assets/18271814/2c97fb00-50c4-4341-b7de-b445f383dcf5">
</p>


- **Root Directory and file system Hierarchy:**

<p align="center">
  <img width="700" height="550" src="https://github.com/mudassirsh/Linux/assets/18271814/26c0ee5a-49ef-479e-9771-5e2fd4ffcbd0">
</p>


## Dual Boot installation:


- Downloaded Linux Ubuntu system from
```
   https://ubuntu.com/download/desktop
```
- Download RUFUS tool that converts ISO files to bootable USB drive.  Follow instructions
```
  https://www.onlogic.com/company/io-hub/how-to-dual-boot-windows-11-and-linux/
```

- **Create partition:** 
  - Right click on the start button and select Disk management
  - Find the largest partition
  - Right click the largest partition and select Shrink Volume
  - Disk space needed for Linux system multiply by 1024 (100GB * 1024= 102400 MB ), specify this space to be removed from the partition and that will show as ‘Unallocated’
  - While preparing the dual boot system, I tried to shrink C:\ drive but the available Disk space was 248 GB but space available to shrink was only 20G
  - The main reason for not being able to shrink the disk are that there are unmovable files on the disk at the time of trying to shrink the volume. Use tool (MiniTool partition) to resize the c:\ drive and this way we can get more space as unallocated

- **In Case of BIOS Lagacy system:** 
		Create bootable usb drive for BIOS legacy based system through using tool Rufus, select partition type = MBR
    If during Linux installation, unallocated disk space showing un-useable. Its because, in BIOS Legacy system max 4 partitions are allowed S legacy system, which are there already.
    In order to resolve this we can create Logical Partition with the help of tool
```
  https://www.diskpart.com/windows-10/how-to-create-logical-partition-in-windows-10-3889.html
 ```

# System Terminologies and Important info
- 💡 **Run Command**             : Alt+F2

- 💡 **GNOME**                   : Gnome is a popular desktop environment and GUI that runs on the top of Linux system. The default display manager of gnome is GDM. Gnome tweaks being used to change settings of different things

- 💡 **Lock/Unlock Session**     : Supper key (Windows key)+L 		Supper key+Esc

- 💡 **Logging out**				     : It kills all the processes

- 💡 **Suspending** 				     : Puts the computer in sleep mod		Nautilus/file manager		Gives three formants to view files

- 💡 **Hidden files**				     : Ctr+H

- 💡 **Delete file**				     : Deleted files automatically moved to location under user home directory: 		.local/share/trash/file

- 💡 **Permanently delete file:**	Shift+delete

- 💡 **To create a document**	 :		Go to search bar:	gedit

- 💡 **FOO** 					         :   Means insert file name here
- 💡 **Debian Package Management:**      <img align="right" width="185" height="185" src="https://github.com/mudassirsh/Linux/assets/18271814/e77e0558-ec3e-4b49-80e2-b2accef93d7e" />
                                        dpkg is the underlying package manager of the system. It can install remove or build packages.
                                        For Debian based systems, the higher level package management is the Apt (Advanced Package Tool).
                                        Apt creates its own user interface on top of the distribution.

- 💡 **App Store**			        : 	Activities > Applications > Software
- 💡 **App Store**			        :	Activities > Applications > Software

- 💡 **Synaptic Packet manager**				Green ones are already installed.
		

<p align="center">
  <img width="180" height="550" src="https://github.com/mudassirsh/Linux/assets/18271814/b45a486b-1d5c-4700-91c8-9bb8292d284e">
  <img width="780" height="350" align="right" src="https://github.com/mudassirsh/Linux/assets/18271814/65a1dd41-51bd-4ee2-9c70-efdaf79b3f00">
</p>

																					

- 💡**Linux Applications:**		 i.e Internet applications, Office productivity suites, Developer tools, Multimedia applications, Graphics editors
Linux support different email clients, both graphical and text base
Most of Linux system offers open source Libre Office
  - writer for word processing
  - Calc for spreadsheets
  - impress for presentations
  - draw for creating and editing graphics

- 💡**Program editors:**						V and emac can be compilers for every computer language
- 💡**Photo/Image editor:**					GIMP
<<<<<<< HEAD
=======

>>>>>>> main
=======

----

## Command Line Operations in Linux

We can initiate graphical applications directly from command line instead of hunting through menus.

We can open terminal from					Application > Tools > Terminal

- **Commands:** 
  	- Cat					used to type out a file
 	- Head					Used to show first few lines of the file.
 	- Tail					used to show the last few lines of a file
 	- Man					used to show the documentation.
 	- |  pipe symbol			used to take input for output of another
					

- **Command have 3 basic elements:** <img align="right" width="250" height="225" src="https://github.com/mudassirsh/Linux/assets/18271814/91fff871-6497-43a0-8f20-12e4c75bbaaa"/>
	- Command
	- Options
	- Arguments <br>

🎯**Command:** Command is the name of the program we are executing <br>   
🎯**Options:** Its followed by one or more options of switches, that modify the command may do. Options usually start with one or two dashes (-print   --print) 
				  Some of the commands have no options, no arguments 


🔸**Sudo**
User with Administrative privileges. 
It allow users to run programs using the security privileges of another user, generally root (the super user). 
When we try to login through sudo, we need to create configuration file to enable our user account to use sudo. The file created in 	/etc/sudoers.d/   	with the file name same as my user name.
Sudo password would be my own user password.

🔸**VT or Virtual Terminals**	<img align="right" width="350" height="225" src="https://github.com/mudassirsh/Linux/assets/18271814/08beb96a-b79b-48d3-b969-bc08052eccaa"/>

VT are the console sessions that use the entire display and keyboard outside of a graphical environment. Such terminals are considered virtual 
because although there can be multiple active terminals. Only one terminal remains visible at a time. VT is not quite the same as command line 
terminal window. You can have many of those visible at once on a graphical desktop. One virtual terminal usually number 1 or 7 reserve for the 
graphical env and text logins are usually enabled on the unused VTS. The example of a situation where the VTs helpful when we ran with the issues 
with graphical desktop. In this situation we can switch to one of the text VTs and troubleshoot. 

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 💡 Ctr+alt+vt6 for VT6
 
										


🔸**Graphical Desktop**
Linux system can turn off or on the graphical desktop in various ways. In newer md-base distributions the display manager is run as a service. You can stop the GUI desktop with system control utility. 
Most distributions with the telinit command	  					

<p align="center">
  <img width="320" height="70" src="https://github.com/mudassirsh/Linux/assets/18271814/01eb8dec-0f66-4877-8d72-2443f2604f47">
  <img width="320" height="70" src=https://github.com/mudassirsh/Linux/assets/18271814/518f0b44-c5c6-491a-9ed8-b547291e75ba">
</p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
re-start after this command  	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	and login into the console with this command			
 				

<br>
<br>
	
🔸**Basic Operations**  <img align="right" width="350" height="250" src="https://github.com/mudassirsh/Linux/assets/18271814/8bcc7f39-949f-4027-9354-695771145f36"/>	<br>
		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	**To execute both above commands, need root user access**	<br>   
		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;				Halt or power off command	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	sudo shutdown -h	<br>
		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;				Reboot		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	sudo shutdown -r

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **In case multi user env, we can leave message for other users**
										
<p align="left">
  <img width="6525 height="50" src="https://github.com/mudassirsh/Linux/assets/18271814/299fac4d-a5a3-49a1-8766-a888d9d1dce9">
</p>



>>>>>>> cee87a2a066bbf7b3ac7f8f90ff59f350293c120
