
# What is Linux?
Just like Windows, iOS, and Mac OS, Linux is an operating system. In fact, one of the most popular platforms on the planet, Android, is powered by the Linux operating system. An operating system is software that manages all of the hardware resources associated with your desktop or laptop. To put it simply, the operating system manages the communication between your software and your hardware. Without the operating system (OS), the software wouldn’t function.


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

🔸 **-F:**	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sometimes you want to know whether a given file is normal file, a directory, a symbolic link, an executable, or a network file, but don’t need information about permissions or owners. For this purpose, you can use the ls -F command.<br>
🔸 **-R:** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	List files recursively means show all the files inside the directories <br>
🔸 **-S:**	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; List files by size <br>
🔸 **-d:** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	Only directories <br>
🔸 **-A:** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 	The first two “files” listed above are . and .., which are implicit directories. To see hidden files with these suppressed, use the -A flag:<img align="right" width="250" height="35" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/90742383-88a7-4ad5-93bc-0bae83d4ecb4"/>	<br>

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
Most of linux distribution and most of its add-on software are installed via the package management system. Each package contain the files and other instructions needed to make one software component to work well and co-operate with other components that comprise the entire system. Packages can depend each other. There are two low level broad package families called package managers.  1- Debian 2- RPM <br>
**Package Managers : Two Levels**  <img align="right" width="350" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0773eea4-60eb-4f3e-8ffc-fd22ced2fc71"/>
Low level package manager take care of details of unpacking individual packages, running scripts, getting the software installed correctly.
High level tool such as apt-get, yum or zypper, works with group of packages. Download the packages from the vendor and figures out the dependencies. Most of the time user only work with the high level tool which will take care of calling the low level tool as needed. Dependency resolution is a particularly important feature of the high level tool. As it handles the details of finding and installing each dependency for user. One should be careful, as installing single package result in many dozens or even hundreds of dependent packages being installed. <br><br>

<p align="center">
  <img width="400" height="220" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/58495ec8-db7f-424a-8029-8d2ff66f2f4d">
  <img width="400" height="220" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/af00d576-692a-46d3-859b-42130810a0d3">
</p>


To see a particular package <img align="right" width="350" height="45" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/1e9b8b3a-972a-4de4-9137-5aa156ae3923"/>
<br>

To see what contained in this package list		<img align="right" width="330" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/a73d3857-8398-446b-8085-ca865feb1dda"/>			
<br>

All packages installed with name wget2						<img align="right" width="300" height="45" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/ab79bab2-89a4-4a17-9d2a-b079b7fc1c16"/>
Wget is a networking command-line tool that lets you download files and interact with REST APIs. <br>
Install 	wget						&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;			```sudo apt-get install wget2-dev``` <br>
Remove wget				&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;						```sudo apt-get remove wget```	





## Linux Documentation Sources

- **Man Pages**
To get the information about something, we use man pages or manual pages.
man socket 			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;			To get the info about socket <br>								
man -f socket		&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;					List of all the pages that called socket<br>
what is socket			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;	Same as man -f socket <br>
man 7 socket			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;				To see particular chapter <br>
man -a socket			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;				To see them all <br>
man -k socket			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;				To see the manual pages where socket is in the description.	<br>


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
  <img width="350" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/e3da29e5-5678-47dd-b1bf-07c78d1f4d1f">
  <img width="450" height="230" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/8c486a52-5649-421b-a30e-0beba89af21b">
</p> <br> 


## File Operations
File system is structured like a tree. In Linux, files are everything. Root directory is not the same as root user.


<p align="center">
  <img width="325" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/01b96e3e-2481-4885-b22d-e1b9d2e005b2">
  <img width="250" height="350" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/cc1bd7b7-c0da-4cc9-98d2-4bcc2cbd2486">
</p><br>

## Filesystem varieties <img align="right" width="400" height="290" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/c7557f0a-f31a-4d06-a1fd-d374af906efd"/>

Lagacy file system such as FAT is also supported
<br><br><br><br><br><br><br> <br><br>

## Linux Partitions
Each file system on a linux system occupies a disk partition  i.e. 	

&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; <b>file system = /dev/sda1		using partition		/dev/sda </b>

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

&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Device node = 	/dev/sda5 <br>
&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Mount point= 	/home

This will attach the file system contained in the disk partition associated with /dev/sda5 device node into the file system tree at the /home mount point. <br><br><br>		
	
To un-mount				<img align="right" width="250" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/5665740c-a1cc-484f-99fd-dbc0e411f8e5"/> 
Mount shows all the present mount systems				

<br>

- **/Bin and /Sbin Directories**	
<b>/Bin</b> directory contains executable binaries , <b>/sbin</b> directory, essential binaries related to system administration
<p align="center">
  <img width="770" height="290" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/1af1124c-a508-4513-88cd-aa83d11a40cc">
</p> 


- **/dev directory**		
Contains device nodes. A type of pseudo file used by most hardware and software devices, except for network devices.<img align="right" width="450" height="70" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0bdb0cc2-220f-4407-ab0d-b94fb13f15c3"/> <br><br><br>
<br>

- **/var directory**      <img align="right" width="350" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/498d3a3e-1e80-4df2-9748-33b964c200f1"/>
Contain files expected to change in size and content. <br><br><br><br><br><br><br><br><br><br>

- **/etc directory**
Home for system configuration files. It contain no binary porgrames although some executable scripts. Supper user can modify config files.


-	**/boot directory**
User specific configuration files found under this directory. 


-	**/lib and /lib64 directories**       
/lib contain library which are common codes shared by applications and essential programs <img align="right" width="450" height="70" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/30bbd9fa-2d19-4ff4-87cf-43670385b76d"/>present in /bin and /sbin. These file names start with LD or LB. Most of them are dynamically loaded libraries, knows as shared libraries or Shared objects. Some Linux system contain lib64 directory containing. Lib64 is 64 bit library while lib is 32bit versions. 


- **Kernel modules or kernel code**       
Often device drivers that can be loaded and unloaded <img align="right" width="450" height="100" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0f9e2cec-5334-41cc-8ba8-62c4d24212b7"/>
without restarting the system, are located in /lib/modules and then the kernel version number.
<br><br><br><br>

- **/media, /run and /mnt**
We need to use removeable media such as usb, cd, dvd drive. <img align="right" width="350" height="120" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/463b5ce3-6aa7-45bc-8a0d-46b99bb0f3ad"/>
To make the material accessible through the regular file system, 
it has to be mounted at a convenient location. Any removeable media automatically mounted when the system notices something has been plugged in, while historically this was done under the /media directory. Modern lunux system mount under the /run directory. User STUDENT usb will be mounted at:	/run/media/student/myusbdrive


- **Additional directories** found under the root directory   <img align="right" width="450" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/f4c58e5d-50ea-4a8f-bcc5-487b3bab67ba"/>
<br><br><br><br><br><br><br><br> <br><br>

- **/usr   directory tree** 
Theoretically contain non-essential programs and <img align="right" width="450" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/3a5b199a-ccdb-4924-b38e-94499981604d"/>
scripts in the sense they should not be needed to initially boot the system and has at least following subsidiaries. 
<br><br><br><br><br><br><br><br><br><br>

- **Diff** 
used to compare files and directories. This often <img align="right" width="450" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/83e9edfa-3405-4da9-a8fe-0ebc7559ba0a"/>
use utility program has many options including the ones we see here. 
Diff is used to text files, for binary files one can use CMP. 
<b>To compare two files use this command.</b>
<p align="center">
  <img width="350" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/fb8c028e-fae8-47ce-b2f4-f3e633d705b7">
</p>
<br><br><br><br><br><br><br>

- **Use Diff3 and Ptaches** <img align="right" width="250" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/4115fa1b-08a1-49e2-b693-933f5588755b"/>
We can compare 3 files using Diff3 which uses one file as the reference basis for the other two.
For example, two people made changes to same file at the same time, diff3 can show changes being made to the original file. 
<p align="center">
  <img width="550" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/73aa3a7b-9da0-4e95-b2dc-6743ed754605">
</p><br>


&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Patch file is running diff with the correct options. <img align="right" width="450" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/98afa0fc-4a27-4a0f-a6e2-68ef6b3d96e7"/>


- **File Utility**
In linux system file extension does not categorise it as it may in other OS. We can not assume the .txt is only the text file, however can be an executable program. In Linux, the file name is meaningful to the user of the system than system itself.In Windows, exe is the executable binary file.

- **Backup (rsync)**
Cp command is used to copy paste file within the same machine, but rsync command used to copy from one machine to another.
Rsync is very effective when recursively copying one directory tree to another.									
Note: rysync can be very destructive, to avoid it, better test it by adding this to command.		-dry-run 				

<p align="">
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Backup &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;  <img width="500" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/284e12c9-67d7-40de-bd25-7438894d5181"> <br>
 &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Copying &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;<img width="320" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/3490b365-0808-4987-bbf5-20eae0ea4705"> <br>
  &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Copying &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;<img width="500" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0da5f21c-a065-45fd-a141-e16962a56032">
</p>
																		
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;Data is being compressed save the time and space in this operation. <br><br>

<p align="center">
  <img width="350" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/dfce539f-c6a8-4673-8a05-1eb23669f0f9"> &nbsp;&nbsp;&nbsp;
  <img width="350" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/a363cd97-c9d5-407d-9f2e-3757af623485">
</p>


## Text Editors

- **Creating files without Editor** 
	Single > send the output of a command to a new file	<img align="right" width="350" height="65" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0386b8a4-1d09-4941-a59d-c8d74874fa5f"/>

	Double >>   will append the new output to existing file	
<br>
	Second technique is to use the cat with re-direction <img align="right" width="250" height="100" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/b0698e90-9f5d-466f-bd99-2c0aed679b02"/>
<br>

<p align="center">
  <img width="450" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/ac440cd5-469f-4d64-9eb3-ec67e0f60979">
</p> <br>

- **Nano and gedit**	
	Nano is terminal based editor while gedit is GUI based editor.	
  To open file in nano   ```nano <filename>```					if doesn't exist, it will be created.
<br>

- **Vi**																
	Using vi, all commands given using keyboard.  <img align="right" width="300" height="170" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/883bc47b-02cd-4b96-b4e1-169f020d5ba3"/>

<p align="center">
  <img width="250" height="35" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/a6052141-27ae-4cf0-ac8e-33fe6d70de52">
  <img width="200" height="35" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/6fa8eb45-73bd-43c1-9408-a3d6449f25d1">
</p> 
<br> <br><br><br><br>
<p align="center">
  <img width="340" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/b8b776fd-1153-41f7-90d5-6c5b718bdc61">
  <img width="340" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/9c5205ea-4b68-4555-932a-fee5b8f4a9ee">
  <img width="340" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/f68ea96a-aff7-4f2e-87ce-09711ab23b96">
</p>

<br>

&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; When searching for text in vi	
<p align="center">
  <img width="300" height="100" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/2bd3b826-ec8f-45e4-9ab3-b171d3ae73d6"> &nbsp;&nbsp;&nbsp;
  <img width="320" height="100" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/33e95c12-b06d-45dc-ab46-d6037712ee2f">
</p>



## User Environments

- **Identify Current User**  <img align="right" width="340" height="100" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/c316f36b-1a1b-4202-be57-3f0dcbe64e9a"/>
Linux is a multi user operating system, 
means more than one user can login at the same time.
<br> <br><br>


- **User start up files**
	/etc directory define global settings for all users. <img align="right" width="340" height="210" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/b7870469-99b1-4a48-a64e-b1f632a653fd"/>
  Once we login startup files ran in the order 	

<br> <br> <br> <br> <br> <br>

- **Groups**
	Group membership administered through /etc/group files. This shows the <img align="right" width="300" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/2edced20-c35d-4d7f-9456-9b21f5492816"/>
	Groups and their members. Permissions on various files and directories administer
	at group level.
<br> <br><br><br><br><br><br>


- **Adding and Removing Users**
	Only root users add or remove users and groups.			
  ````
  sudo useradd user1					
  sudo userdel user1 
  ````

  Adding user, which by default sets home directory to <b>/home/user1 </b>

  And this directory will be populated with some basic files (user = bmoose) <img align="right" width="300" height="60" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/2432ce03-06fb-40bd-bacb-a188faaadc34"/>
  <br>By using the -r we not only remove the account but also the recursive directories associated to the account.
<br>

- **create user** 

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -m = to make home directory as some distr not do so by default 
  <br>
 	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -s = default shell to the bin bash	<br> <img align="right" width="470" height="60" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/07fb9eb4-b0ec-46e9-bf82-e6e751e6de0f"/> 
  <br><br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -c = name <br>   <img align="right" width="550" height="60" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/e12b3fb0-4fa4-4cd6-a8bc-2d88a548ee42"/> 
  <br><br><br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; To log into new user account  <img align="right" width="350" height="50" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/abff4656-1204-4398-9fac-a0ac7290ed56"/>
  <br><br><br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; To display the contents of some specific directory  <img align="right" width="450" height="50" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/53be3aae-87ee-47d2-9a2e-c701bdf77f8a"/>

<br><br>

- **Adding and Deleting group**

<p align="center">
  <img width="450" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/8188aff2-8e68-4dc6-8433-f0b218205087">
  <img width="400" height="25" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/02278963-65e5-428d-9b2e-f8937fc1593f">
</p>


- **Adding user to existing group (using mod)**
First look at what groups user already belongs to <img align="right" width="300" height="45" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/55c7a88a-81c9-4017-a219-1bc3bed18a3e"/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; rjsquirrel = group  
<br>
  
  Group mod is used to change group properties such as group ID with -G option <img align="right" width="400" height="50" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/d66affff-5ecc-4bca-93ec-42394361b53c"/>
<br><br><br>


- **Root account**	
	Root account is very powerful and has full access to the system. Its often called administrator account. 
	Use sudo to assign more limited privileges to user account, and used for temporary basis.
<br>

- **Environment Variable**
	Env variable is just a character string that contain information used by one or more application. There are number of ways to view the value of currently set environment variables.<br>
			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	<b> set  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	 	or &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	  export</b>

<br>

- **The Home Variable**
	Home is the environment variable that represent the home or login directory of the user.
	~ value is often used as abbreviation value to the home
<p align="center">
  <img width="220" height="220" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/18a20df0-7b32-4324-a97d-132ba6687223">
  <img width="500" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/2aecf75d-5664-41ac-8199-441745b2f634">
</p>
<br>


- **The Path Variable**
	Path is an order list of directories. Path is scanned when a command is given to find the appropriate program or script to run. Each directory in the path is separated by colons 

<p align="center">
  <img width="470" height="70" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/d332a6ae-85d5-40df-bccd-e4490330dfa5">
  <img width="350" height="60" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/ee33ffb8-a34d-4b16-8587-e7dd46170954">
</p><br>

- **The SHELL Variable**
	The environment variable shell, points to the user default command shell. The program whatever we type in a command window usually bash and it contains the full path name to the shell. <img align="right" width="230" height="50" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/96826ed3-804e-49a4-b1ea-f2cb3ab924ef"/>
<br><br><br>

- **The Command Line Prompt (PS1)**
	Prompt statement (PS) is used to customise whatever we would like to type in 
<p align="center">
  <img width="260" height="100" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/e376b114-cf36-4702-9525-42b8231babc4">
  <img width="240" height="180" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/0bbc12ff-107c-4418-b230-216d196ad7c9">
  <img width="250" height="180" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/c0946bd7-1168-4e2b-85d6-088195dc65fc">
</p>
<br>

- **Recalling Previous Commands**
<img align="right" width="350" height="130" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/51f7e131-2ff9-4ffb-b8e4-b7a5a574a126"/>
<br> <br><br><br><br>

- **Keyboard shotcuts**
<p align="right">
  <img width="400" height="300" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/475abc22-7fcf-438f-8fd4-c5f5b1ea4a42">
</p>
<br>


- **File Ownership AND Permission**
<p align="right">
  <img width="550" height="140" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/677363b8-aad8-43c5-a811-0040d16978a0">
</p>

<p align="center">
  <img width="110" height="60" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/638de802-d8c8-41fb-b66a-ea5c1b387146">
  <img width="200" height="120" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/ae2bb0ab-02a4-4463-97cb-bd570dc041cc">
  <img width="380" height="70" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/f77518a0-facd-4017-bd54-eab5c848c3f2">
</p><br>

<p align="center">
  <img width="230" height="180" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/eba3828b-cc30-4868-a253-c41ca57508ca">
  <img width="440" height="60" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/3b4637e4-483f-4615-a63d-ebd9bf343b23">
</p>
<br>

- **Change ownership and change group**
<p align="center">
  <img width="430" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/b8312047-2976-4c39-bda7-c9709fba4a39">
  <img width="300" height="170" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/030bc00e-c578-40ed-aa7d-ebaf4b2c605f">
</p>
<br>

- **Command line tools for manipulating text files**
	To read file		````  cat readme.txt	  ````	<br>		
	Main purpose of the cat is to combine or concatenate 

<p align="center">
  <img width="640" height="240" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/c5fff1b3-7da6-4942-b4f3-ae4ac2cd5473">
  <img width="640" height="240" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/b9720a8e-3fd7-4663-aec7-df05a17a1f1e">
</p>

Create file3 with the text of file 1 & 2   ```` Cat file1.txt file2.txt > file3.txt ````			

In case we want to load a very large file but we don’t want to overload the system, we can do so by apply the less switch <img align="right" width="250" height="50" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/c091bf03-10b9-4977-9ac8-b7357dce70ec"/>
<br><br>

- **Sort**
<p align="center">
  <img width="600" height="250" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/7404819d-3bd1-4782-9535-36ac596b9dfc">
</p>

- **Unique**		
unique is used to remove repetitive values. Sort and unique can applied together on multiple files. <img align="right" width="350" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/2d6683ea-e284-42df-859e-3463bbb83415"/> <br>
<img align="right" width="350" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/c9bf51cd-7c11-4da1-b1bc-92f673633cda"/><br>Count the number of duplicate entries<img align="right" width="350" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/bc758b51-0c5f-4f36-b17a-e138c8063c7e"/>
<br><br>

Below are two files containing Names and IDs and phone numbers
<p align="center">
  <img width="100" height="150" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/9435680e-34dd-4260-8ac7-78e13a03e248">&nbsp;&nbsp;
  <img width="100" height="150" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/ef34ea19-12da-4968-9c39-d3893d04fd7f">
</p>

We can combine these values and see them together in one file		-d = delimeter			<img align="right" width="350" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/fab89f36-c74b-4eec-82d6-a1f6f0b1e3b7"/>
<br>


<p align="center">
  <img width="600" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/41ca11a6-c18a-40e4-8c5b-acfffea24e3e">
  <img width="300" height="200" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/6c723490-8d77-48cd-b0c4-e19e5b15ae54">
</p>

<p align="center">
  <img width="400" height="30" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/babed564-62f5-4a5b-b292-0457074a03ed">
  <img width="560" height="180" src="https://github.com/mudassir-sh/17marchNew/assets/149414511/4c7042c8-6ba7-4f50-b408-2bd1b90c9431">
</p>


