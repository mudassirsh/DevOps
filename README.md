
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
  <img width="500" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/b212dbf9-f8c6-4f20-96a8-9bc29cba7ee7">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/804d4384-d83a-4c83-ad19-25092dfbcabe">
  <img width="300" height="300" src="https://github.com/mudassirsh/Linux/assets/18271814/1db53431-3f86-4576-9ab3-6dc5979a571c">
</p>


- **File systems supported by Linux:**

<p align="center">
  <img width="420" height="150" src="https://github.com/mudassirsh/Linux/assets/18271814/9b7c1228-8172-4218-a4a8-58180e0aafae">
  <img width="250" height="210" align="right" src="https://github.com/mudassirsh/Linux/assets/18271814/2c97fb00-50c4-4341-b7de-b445f383dcf5">
</p><br><br>


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

🎯 **Command:** Command is the name of the program we are executing <br>   
🎯 **Options:** Its followed by one or more options of switches, that modify the command may do. Options usually start with one or two dashes (-print   --print) 
				  Some of the commands have no options, no arguments 


🔸 **Sudo**
User with Administrative privileges. 
It allow users to run programs using the security privileges of another user, generally root (the super user). 
When we try to login through sudo, we need to create configuration file to enable our user account to use sudo. The file created in 	/etc/sudoers.d/   	with the file name same as my user name.
Sudo password would be my own user password.

🔸 **VT or Virtual Terminals**	<img align="right" width="350" height="225" src="https://github.com/mudassirsh/Linux/assets/18271814/08beb96a-b79b-48d3-b969-bc08052eccaa"/>

VT are the console sessions that use the entire display and keyboard outside of a graphical environment. Such terminals are considered virtual 
because although there can be multiple active terminals. Only one terminal remains visible at a time. VT is not quite the same as command line 
terminal window. You can have many of those visible at once on a graphical desktop. One virtual terminal usually number 1 or 7 reserve for the 
graphical env and text logins are usually enabled on the unused VTS. The example of a situation where the VTs helpful when we ran with the issues 
with graphical desktop. In this situation we can switch to one of the text VTs and troubleshoot. 

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 💡 Ctr+alt+vt6 for VT6
 
										
</br>


🔸 **Graphical Desktop**
Linux system can turn off or on the graphical desktop in various ways. In newer md-base distributions the display manager is run as a service. You can stop the GUI desktop with system control utility. 
Most distributions with the telinit command	  					

<p align="center">
  <img width="320" height="70" src="https://github.com/mudassirsh/Linux/assets/18271814/01eb8dec-0f66-4877-8d72-2443f2604f47">
  <img width="320" height="70" src="https://github.com/mudassirsh/Linux/assets/18271814/518f0b44-c5c6-491a-9ed8-b547291e75ba">
</p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
re-start after this command  	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	and login into the console with this command			
 				

<br>
<br><br>
	

🔸 **Basic Operations** <img align="right" width="300" height="250" src="https://github.com/mudassirsh/Linux/assets/18271814/8bcc7f39-949f-4027-9354-695771145f36"/>	<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	**To execute both above commands, need root user access**	<br>   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;				Halt or power off command	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	sudo shutdown -h	<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;				Reboot		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	
sudo shutdown -r

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **In case multi user env, we can leave message for other users**
										
<p align="left">
  <img width="6525 height="50" src="https://github.com/mudassirsh/Linux/assets/18271814/299fac4d-a5a3-49a1-8766-a888d9d1dce9">
</p>

🔸 **App Installation locations** 
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

🔸 **Navigating Directories** 
<p align="center">
  <img width="280 height="330" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/b34d7457-c218-44ce-9d30-a27c6c6cfb18">
  <img width="400" height="250" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/28eb40b4-9280-4131-9442-08710a091b69">
</p>
			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 💡 New command: &nbsp;&nbsp;&nbsp;&nbsp; pushd  & Popd command
			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; cd -  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Shows where you were last
</br>
</br>

🔸 **Two types of path names:	Absolute or Relative paths**
In Absolute path, we move directory to directory and start with slash /
In Relative path, in order to reach to destination directory we may jump the directories

<p align="center">
  <img width="230" height="150" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/50458821-cc77-47e4-bfaf-8a1a283929a1">
  &nbsp;&nbsp;&nbsp;
  <img width="450" height="350" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/8ee30641-d957-4e16-a8ff-3ac8c4042e47">
</p>
</br>
</br>


🔸 **Exploring File System**

Examples of Navigating directories
<img align="left" width="250" height="80" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/70ae704a-3077-4556-8eb0-59e6f5845334"/>
<br><br>


<p align="center">
  <img width="380" height="180" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/572c5767-4571-4b3e-bc5c-abb23e66ddd2">
  <img width="200" height="360" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/288a2bf4-b2fb-4e63-8220-c4a5dfd158ff">
</p><br>

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


<p align="center">
  <img width="335" height="100" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/e9f2fffb-c8b4-47c9-9367-45f9880b4065">
  &nbsp;
  <img width="350" height="170" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/814b66f8-3541-4030-82fa-97da6d792560">
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
<td>rmdir</td> <td></td>
</tr>


<tr>
<td>Remove directory and its contents</td>
<td>rm -rf</td> <td></td>
</tr>  

<tr>
<td>Create empty file</td>
<td>echo > file1 </td> <td></td>
</tr>


<tr>
<td>remove file interactive way</td>
<td>rm -i [filename]</td> <td></td>
</tr>

</table>

</br>

- **Standard File streams**	<img align="right" width="380" height="170" src="https://github.com/mudassirsh/17marchdemo/assets/18271814/8bfd4af4-3569-44d1-9798-254eef3de216"/>
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
</p> <br>


- **Pipes**  <img align="right" width="350" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/2b7fd332-a678-43c6-b763-7b10b2bdce08"/>


Locate directories and files with both zip and bin in their name. <img align="right" width="350" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/f21f9925-f634-4ca4-ad48-ca5c68ad0f0e"/>
<br>
Find file with string in the name	 find . [filename]	<img align="right" width="350" height="60" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/7cc65030-4b33-4f32-98f0-eda62a507643"/>		
💡 dot  means in the current directory 

<br>
ls option gives us more info , who own it etc. <img align="right" width="450" height="40" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/9b32df91-b300-41ee-9d1d-aa04d1017775"/>
<br><br><br><br>
To locate file through Linux database &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	  locate [filename]

To update Linux Database	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;					sudo updatedb


- **Wildcards and mismatching file names**  <img align="right" width="460" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/bb2c0773-be95-4e85-ade3-362bc40bd8eb"/>

<br><br> <br> <br><br> <br><br>
🔅 Disk usage of files or directory starts with name a   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   du -sh a*  <img align="right" width="300" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0d6a0e65-71b4-4e3e-8dd0-ebf1f5770193"/>

<br>
Switch sh means  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	s = size &nbsp;&nbsp;   h = human readable form


<br> <br>

🔅 Disk usage of files start with name a but only log files		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;					
```
du -sh a*log*
```

<br> <br>
🔅 File/folder names start with letter 'a' but after only contain p to z alphabets in the name <img align="right" width="300" height="100" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/66b91ce6-d002-4751-886a-9502ae135b08"/>


<br><br><br><br>

- **Search Utility**

Linux admin some time search for diagnostic information after a program fails which matches specific conditions 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Find directory name gcc		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```sudo find /usr -type d -name gcc``` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Find file name gcc				   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 							```sudo find /usr -type f -name gcc```


<br>

- **Advance find options**

Run the command matches on my search criteria. -exec option used for this purpose			
```
find -name “*.swp” -exec rm {} ‘;’
```
Find the .swp files and delete them. Curly brackets are the place holder for file names 
Resolved from the find expression. We have to end the command with ‘;’ or '\\;'

Find files greater that 10MB in size and running a command on those files <img align="right" width="450" height="90" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/135326a9-c088-48ac-b6ca-5edde6ad16f5"/>

<br><br><br><br>


🔥 **Ls command switches:**

🔸 **-F:**	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sometimes you want to know whether a given file is normal file, a directory, a symbolic link, an executable, or a network file, but don’t need information about permissions or owners. For this purpose, you can use the ls -F command.
🔸 **-R:** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	List files recursively means show all the files inside the directories
🔸 **-S:**	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; List files by size
🔸 **-d:** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	Only directories
🔸 **-A:** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	The first two “files” listed above are . and .., which are implicit directories. To see hidden files with these suppressed, use the -A flag:<img align="right" width="250" height="35" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/90742383-88a7-4ad5-93bc-0bae83d4ecb4"/>	

* 🤔 Sudo find .			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;every single fine and directory underneath here
* 🤔 Sudo find . -type d			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;only show directories and sub directories
* 🤔 Sudo find . -type d -maxdepth 1		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	only show directories at depth 1 
* 🤔 find . -type f -exec grep -H log {} \;	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; 	it search the every single  file that has the word log inside the file
* 🤔 find . -type f -exec grep ls -l {} \;		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	give us listing of all the files
* 🤔 find . -type f -ls			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  		show us files
* 🤔 sudo find . -size 0			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	all the files/directories of zero size
* 🤔 sudo find . -size 0 -ls 
* 🤔 sudo find . -newer btmp				&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;show files newer than the file btmp




## Package Management System on Linux**  
Most of linux distribution and most of its add-on software are installed via the package management system. Each package contain the files and other instructions needed to make one software component to work well and co-operate with other components that comprise the entire system. Packages can depend each other. There are two low level broad package families called package managers.  1- Debian 2- RPM 
**Package Managers : Two Levels**  <img align="right" width="350" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0773eea4-60eb-4f3e-8ffc-fd22ced2fc71"/>
Low level package manager take care of details of unpacking individual packages, running scripts, getting the software installed correctly.
High level tool such as apt-get, yum or zypper, works with group of packages. Download the packages from the vendor and figures out the dependencies. Most of the time user only work with the high level tool which will take care of calling the low level tool as needed. Dependency resolution is a particularly important feature of the high level tool. As it handles the details of finding and installing each dependency for user. One should be careful, as installing single package result in many dozens or even hundreds of dependent packages being installed. 

<p align="center">
  <img width="310" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/58495ec8-db7f-424a-8029-8d2ff66f2f4d">
  <img width="310" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/af00d576-692a-46d3-859b-42130810a0d3">
</p>


To see a particular package <img align="right" width="350" height="45" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/1e9b8b3a-972a-4de4-9137-5aa156ae3923"/>
<br>

To see what contained in this package list		<img align="right" width="330" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/a73d3857-8398-446b-8085-ca865feb1dda"/>			
<br>

All packages installed with name wget2						<img align="right" width="300" height="45" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/ab79bab2-89a4-4a17-9d2a-b079b7fc1c16"/>
Wget is a networking command-line tool that lets you download files and interact with REST APIs. <br>
Install 	wget						&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;			```sudo apt-get install wget2-dev```
Remove wget				&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;						```sudo apt-get remove wget```	


-------


## Linux Documentation Sources

- **Man Pages**
To get the information about something, we use man pages or manual pages.
man socket 			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;			To get the info about socket 								
man -f socket		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;					List of all the pages that called socket
what is socket			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;	Same as man -f socket
man 7 socket			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;				To see particular chapter
man -a socket			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;				To see them all
man -k socket			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;				To see the manual pages where socket is in the description.	


## Info Page Structure
Info pages are another way to know about the topic.
Info make	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;						Give that command and info would display about the topic


- **Help Command**
Help command is another way to get help on topics.

<br>

## Different Process Types
- PID = 	Process ID number

Processes can be killed with this command <img align="center" width="170" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/5db66d36-0e8e-4bb0-a376-a2d34f9d45bd"/><br>
We can not kill other user processes until we are not a root user
<p align="center">
  <img width="300" height="120" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/8b217235-b850-4e8f-a05a-b81ac973405a">
  <img width="300" height="120" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/4580c516-d907-486d-8d25-f328b986e267">
</p>


💠 **Types of Users**
	Many users can access the system simultaneously <img align="right" width="150" height="90" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/7b33e864-790b-47d1-88d0-527acbd59258"/>
			- user start the process recognised from RUID, there are different kind of IDs 
			
<br>

💠 **Prosesses** 

In Linux, higher priority Processes get preferential access to CPU. Process priority is set by nice value or niceness of process.The lower the nice value, the higher the priority. -20 is the highest priority +20 is the lowest. 

<p align="center">
  <img width="250" height="130" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/046d5c3b-51b5-48a4-b619-1722b81b63b2">
  <img width="350" height="170" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/c1e97ac1-4262-4ffb-b0a1-ef2e28a83f01">
</p>
<br>
With gnome command, we can see processes in GUI.
<p align="center">
  <img width="250" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/099067f6-92d6-444b-85e7-672e2aacf684">
  <img width="370" height="180" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/3beb5605-2b22-4912-b832-0ebca8542351">
</p><br>


- We can see CPU utilization from boot time average. <img align="right" width="290" height="50" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/18d13176-5b0f-4206-807a-ef8baa53a2d4"/>

	- Command used for it is 		w	
	- .45 means, in last 1 minute cpu usage is 45%
	- .17 means, in last 5 minute cpu usage is 17%
	- .12 means, in last 15 minutes cpu usage is 12%


- ps			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; to see the processes <img align="right" width="250" height="240" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/9e0d0843-49d9-4cfe-be8c-766c66f82814"/>
- ps -f		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;						to see more details of processes being runing 
- ps -l		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;						show different details of processes.
- ps -elf | less		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;					shows all processes on the system
- ps aux | less
- pstree			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; this shows the processes in tree diagram, shows the relationship between itself and its parent process. 
<br>


💡 Once the physical memory is run out, system start using the swap space or temporary space.


Top command can be used to interactively control processes.	We can do the same from GUI   <b>  application > System Monitor		</b><br><br>


- **Scheduling Future Processes** <img align="right" width="350" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/736c9fc8-f254-4897-a34d-400a31cc0dce"/>

<br><br><br><br><br><br><br><br><br>

## Cron		
it’s a time base scheduling job
It start with cron expression, followed by script command to execute.


<p align="center">
  <img width="320" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/e3da29e5-5678-47dd-b1bf-07c78d1f4d1f">
  <img width="370" height="230" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/8c486a52-5649-421b-a30e-0beba89af21b">
</p> <br> 


## File Operations
File system is structured like a tree. In Linux, files are everything. Root directory is not the same as root user.


<p align="center">
  <img width="325" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/01b96e3e-2481-4885-b22d-e1b9d2e005b2">
  <img width="250" height="350" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/cc1bd7b7-c0da-4cc9-98d2-4bcc2cbd2486">
</p><br>

## Filesystem varieties <img align="right" width="350" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/c7557f0a-f31a-4d06-a1fd-d374af906efd"/>

Lagacy file system such as FAT is also supported
<br><br><br><br><br><br><br>

## Linux Partitions
Each file system on a linux system occupies a disk partition  i.e. 	

&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; file system = /dev/sda1		using partition		/dev/sda

Programs required to run are kept on a separate partition known as root or slash<br>

<b>This is the separate partition than the one contains the files owned by regular users of the system in /home</b>

The advantage of this is, when all the space on system is exhausted, system may operate normally. 
<br>


## Mount Points 
Before we start using a file system, we need to mount it on the file system tree at the mount point.
This is simply a directory.
We need to mount it on the file system tree at the mount point. 
				
Mount point are usually the empty directories.

The mount command is used to attach a file system.  (which can be local to the computer or on a network somewhere within
the file system tree) The basic arguments are the device node and mount point. 

<p align="right">
  <img width=330" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0a52099b-c81f-4693-8558-757e2e2f397d">
  <img width="350" height="270" align="right" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/d93d32d5-0d8c-463a-9f6e-a32169e52568">
</p>

&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;Device node = 	/dev/sda5
&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;Mount point= 	/home

This will attach the file system contained in the disk partition associated with /dev/sda5 device node into the file system tree at the /home mount point. <br><br><br>		
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;								To un-mount				<img align="right" width="350" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/5665740c-a1cc-484f-99fd-dbc0e411f8e5"/>
		


<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;mount			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;				show all the present mount systems.

<br>

- **/Bin and /Sbin Directories**	
<b>/Bin</b> directory contains executable binaries , <b>/sbin</b> directory, essential binaries related to system administration
<p align="center">
  <img width="630" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/1af1124c-a508-4513-88cd-aa83d11a40cc">
</p>

- **/dev directory**		
Contains device nodes. A type of pseudo file used by most hardware and software devices, except for network devices.<img align="right" width="350" height="50" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0bdb0cc2-220f-4407-ab0d-b94fb13f15c3"/> <br><br><br>


- **/var directory**      <img align="right" width="350" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/498d3a3e-1e80-4df2-9748-33b964c200f1"/>
Contain files expected to change in size and content. <br><br><br><br><br><br><br><br><br><br>

- **/etc directory**
Home for system configuration files. It contain no binary porgrames although some executable scripts. Supper user can modify config files.
<br>
-	**/boot directory**
User specific configuration files found under this directory. 
<br>

-	**/lib and /lib64 directories**       
/lib contain library which are common codes shared by applications and essential programs <img align="right" width="450" height="70" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/30bbd9fa-2d19-4ff4-87cf-43670385b76d"/>present in /bin and /sbin. These file names start with LD or LB. Most of them are dynamically loaded libraries, knows as shared libraries or Shared objects. Some Linux system contain lib64 directory containing. Lib64 is 64 bit library while lib is 32bit versions. 
<br>

- **Kernel modules or kernel code**       
Often device drivers that can be loaded and unloaded <img align="right" width="450" height="100" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0f9e2cec-5334-41cc-8ba8-62c4d24212b7"/>
without restarting the system, are located in /lib/modules and then the kernel version number.
<br><br>

- **/media, /run and /mnt**
We need to use removeable media such as usb, cd, dvd drive. <img align="right" width="350" height="120" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/463b5ce3-6aa7-45bc-8a0d-46b99bb0f3ad"/>
To make the material accessible through the regular file system, 
it has to be mounted at a convenient location. Any removeable media automatically mounted when the system notices something has been plugged in, while historically this was done under the /media directory. Modern lunux system mount under the /run directory. User STUDENT usb will be mounted at:	/run/media/student/myusbdrive
<BR>

- **Additional directories** found under the root directory   <img align="right" width="450" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/f4c58e5d-50ea-4a8f-bcc5-487b3bab67ba"/>
<br><br><br><br><br><br><br><br>

- **/usr   directory tree** 
Theoretically contain non-essential programs and <img align="right" width="450" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/3a5b199a-ccdb-4924-b38e-94499981604d"/>
scripts in the sense they should not be needed to initially boot the system and has at least following subsidiaries. 
<br><br><br><br><br><br><br>

- **Diff** 
used to compare files and directories. This often <img align="right" width="450" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/83e9edfa-3405-4da9-a8fe-0ebc7559ba0a"/>
use utility program has many options including the ones we see here. 
Diff is used to text files, for binary files one can use CMP. 
<b>To compare two files use this command.</b>
<p align="center">
  <img width="350" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/fb8c028e-fae8-47ce-b2f4-f3e633d705b7">
</p>
<br><br><br>

- **Use Diff3 and Ptaches** <img align="right" width="250" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/4115fa1b-08a1-49e2-b693-933f5588755b"/>
We can compare 3 files using Diff3 which uses one file as the reference basis for the other two.
For example, two people made changes to same file at the same time, diff3 can show changes being made to the original file. 
<p align="center">
  <img width="550" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/73aa3a7b-9da0-4e95-b2dc-6743ed754605">
</p>


