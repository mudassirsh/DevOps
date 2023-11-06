
# Linux System


- **Kernel:**			is the core of operating system. Glue between hardware and application i.e. Linux kernel	

<p align="center">
  <img src="https://github.com/mudassirsh/Linux/assets/18271814/30174512-da82-475d-af56-f48abf0ae622">
  <img width="250" height="250" src="https://github.com/mudassirsh/Linux/assets/18271814/6358118b-3263-4596-8303-ea1c8febcb35">
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
  <img width="180" height="550" align="right" src="https://github.com/mudassirsh/Linux/assets/18271814/b45a486b-1d5c-4700-91c8-9bb8292d284e">
  <img width="500" height="350" src="https://github.com/mudassirsh/Linux/assets/18271814/65a1dd41-51bd-4ee2-9c70-efdaf79b3f00">
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
 
										
</br>


🔸**Graphical Desktop**
Linux system can turn off or on the graphical desktop in various ways. In newer md-base distributions the display manager is run as a service. You can stop the GUI desktop with system control utility. 
Most distributions with the telinit command	  					

<p align="center">
  <img width="320" height="70" src="https://github.com/mudassirsh/Linux/assets/18271814/01eb8dec-0f66-4877-8d72-2443f2604f47">
  <img width="320" height="70" src="https://github.com/mudassirsh/Linux/assets/18271814/518f0b44-c5c6-491a-9ed8-b547291e75ba">
</p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
re-start after this command  	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	and login into the console with this command			
 				

<br>
<br>
	

</br>
🔸**Basic Operations**  <img align="right" width="300" height="250" src="https://github.com/mudassirsh/Linux/assets/18271814/8bcc7f39-949f-4027-9354-695771145f36"/>	<br>
		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	**To execute both above commands, need root user access**	<br>   
		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;				Halt or power off command	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	sudo shutdown -h	<br>
		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;				Reboot		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	
    sudo shutdown -r

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **In case multi user env, we can leave message for other users**
										
<p align="left">
  <img width="6525 height="50" src="https://github.com/mudassirsh/Linux/assets/18271814/299fac4d-a5a3-49a1-8766-a888d9d1dce9">
</p>

🔸**App Installation locations** 
<img align="right" width="350" height="40" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/2f79b85d-d7b1-4e03-99cd-bb99895887ee"/>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Apps live either in the below or screenshot directories     
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;🎯 /opt   OR	 /usr/local/bin		OR 		/usr/local/sbin   OR  in User Account space:   /home/student/bin


One way to locate the program is to employ the ‘which utility’. 	For example find out where the ‘diff’ program is running on the file system.  	
```
Command:                                which diff
If which doesn’t work then use 		where is diff 
```
<p align="center">
  <img width="650 height="50" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/8df12b3d-4ca1-4e6f-8330-8fe002e25db0">
</p>
</br>

🔸**Navigating Directories** 
<p align="center">
  <img width="300 height="350" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/b34d7457-c218-44ce-9d30-a27c6c6cfb18">
  <img width="500 height="350" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/28eb40b4-9280-4131-9442-08710a091b69">
</p>
			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 💡 New command: &nbsp;&nbsp;&nbsp;&nbsp; pushd  & Popd command
			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; cd -  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Shows where you were last
</br>
</br>

🔸**Two types of path names:	Absolute or Relative paths**
In Absolute path, we move directory to directory and start with slash /
In Relative path, in order to reach to destination directory we may jump the directories

<p align="center">
  <img width="250" height="170" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/50458821-cc77-47e4-bfaf-8a1a283929a1">
  <img width="450" height="350" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/8ee30641-d957-4e16-a8ff-3ac8c4042e47">
</p>
</br>
</br>


🔸**Exploring File System**

Examples of Navigating directories
<img align="left" width="300" height="100" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/70ae704a-3077-4556-8eb0-59e6f5845334"/>
<p align="center">
  <img width="500" height="200" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/572c5767-4571-4b3e-bc5c-abb23e66ddd2">
  <img width="200" height="400" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/288a2bf4-b2fb-4e63-8220-c4a5dfd158ff">
</p>

- **Commands**
<table>
<tr>
<td width="500">To get list of files </td>
<td>ls</td>
</tr>
<tr><td>To get a list of files and hidden files</td>
<td>ls -a</td>
</tr>

<tr>
<td>To display the contents of some specific directory</td>
<td> ls -l /etc/skel </td>
</tr>

<tr>
<td>Will show only directories</td>
<td>tree -d</td>
</tr>

<tr>
<td>How many lines in the file</td>
<td>wc [file name]</td>
</tr>

<tr>
<td>show the file contents</td>
<td>cat [file name]</td>
</tr>

<tr>
<td>Show the file contents with row numbering</td>
<td>cat -n [filename]</td>
</tr>

<tr>
<td>To see the file page by page</td>
<td>less [filename]</td>
</tr>

<tr>
<td>Page by page with row numbering</td>
<td>less -N [filename]</td>
</tr>

<tr>
<td>First few lines of the file</td>
<td>head [filename]</td>
</tr>

<tr>
<td>Number of rows we want to see. It will show top 20 rows</td>
<td>head -20 [filename]</td>
</tr>

<tr>
<td>Last few lines</td>
<td>tail [filename]	&nbsp;&nbsp;&nbsp;	tail -20 [filename]</td>
</tr>

<tr>
<td>If we want to load file backwards, last page and upwards</td>
<td>tac [filename]</td>
</tr>
<tr>
<td>Create empty file as place holder</td>
<td>touch [filename]</td>
</tr>

</table>


<p align="left">
  <img width="450" height="150" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/e9f2fffb-c8b4-47c9-9367-45f9880b4065">
  <img width="450" height="200" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/814b66f8-3541-4030-82fa-97da6d792560">
</p>


<table border: 0>
<tr>
<td>Make directory inside certain directory</td>
<td>mkdir /usr/sampledir</td>
<td><img align="right" width="300" height="40" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/58e25908-26e2-4651-ae4e-264e6901d6de"/>
</td>  
</tr>

<tr>
<td>Remove empty directory</td>
<td>rmdir</td> 
</tr>


<tr>
<td>Remove directory and its contents</td>
<td>rm -rf</td> 
</tr>  

<tr>
<td>Create empty file</td>
<td>echo > file1 </td> 
</tr>


<tr>
<td>remove file interactive way</td>
<td>rm -i [filename]</td> 
</tr>

</table>

</br>

- **Standard File streams**	<img align="right" width="400" height="150" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/8bfd4af4-3569-44d1-9798-254eef3de216"/>
	When commands are executed, by default there are 3 file streams or descriptors always open for use.These are standard input, standard output and standard error. 
  - standard input	 is keyboard
  - standard output is terminal 
  - standard error are the log files, usually nothing goes in there.
<br>

- **I/O Redirection**		
Through the command shell we can redirect the 3 standard file stream so that we can get input either from file or from another command 
instead of from our keyboard. And we can write output and errors to files or use them to provide input for subsequent commands. 
<br>For example if we have a programme called do-something reads from standard in and write to standard out and to standard error. <img align="right" width="350" height="25" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/a6d8643c-1c02-4f39-a242-b243c1973835"/>
We can change its input source by using the less than sign < followed by the name of the file to be consumed for input data.<br>
If we want to send the out to a file, use the greater than sign as in this example. <img align="right" width="350" height="25" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/65198f72-1a03-467e-b1d1-4607e3936315"/> <br> <br>
As the error is different than standard output, so it will still be seen on terminal window. Error output we and send this way <img align="right" width="350" height="25" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/7d1994f5-54b4-4b0c-bf08-125e96c8eded"/> <br>
We can send both descriptor 2 and 1 to the same file 	

<p align="center">
  <img width="550" height="25" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/f8ebc1eb-4377-4fb2-b3a7-aa8a2708080b"> <br>
  OR
  <br>
  <img width="550" height="25" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/6489ba40-e297-4a31-9d0c-a082571d826b">
</p>
