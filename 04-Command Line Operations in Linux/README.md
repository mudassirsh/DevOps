# Command Line Operations in Linux

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
