
# What is Linux?
Just like Windows, iOS, and Mac OS, Linux is an operating system. In fact, one of the most popular platforms on the planet, Android, is powered by the Linux operating system. An operating system is software that manages all of the hardware resources associated with your desktop or laptop. To put it simply, the operating system manages the communication between your software and your hardware. Without the operating system (OS), the software wouldn’t function.










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


