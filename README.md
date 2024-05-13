# Operating System Lab - Commands
This Repository Contains a Collection of Linux Commands Taught in each OS Lab Class Separated by Weeks

Table of Contents
* [Week 1 to 6](#week-1-to-6)
* [Week 7](#week-7)
* Week 8 (Not Added Yet)
* Week 9 (Not Added Yet)
* Week 10 (Not Added Yet)
* Week 11 (Not Added Yet)
...
  
## Week 1 to 6
### Popular Operating Systems
* Windows, MacOS, Linux, Android and ...
### Operating Systems History
Operating systems evolved from simple mainframe setups in the 1950s to today's complex, user-friendly platforms like Windows, macOS, and Linux. Key milestones include the advent of Unix in the 1970s, Windows dominance in the PC market in the 1990s, and the rise of mobile operating systems like Android and iOS in the 2000s.
* Operating Systems Differences
* Operating Systems Distributions
* Open Source and Closed Source
### What is Linux ?
Linux is a family of open-source operating systems based on the Linux kernel. It's known for its flexibility, stability, and security, and it's widely used in servers, supercomputers, and embedded systems.
* Why Linux
* Install Linux
* Working with Linux
### Linux Commands
* [ls](#1-ls)
* [cd](#2-cd)
* [Path Address Symbols](#3-linux-path-address-symbols))
* [clear](#4-clear)
* [exit](#5-exit)
* [mkdir](#6-mkdir)
* [touch](#7-touch)
* [cat](#8-cat)
* [nano](#9-nano)
* [pwd](#10-pwd)
* [rm](#11-rm)
* [ln](#12-ln)
* [man](#13-man)
* [cp](#14-cp)
* [mv](#15-mv)
* [locate](#16-locate)
* [history](#17-history)
* [find](#18-find)

---

### 1. [ls](https://linuxcommand.org/lc3_man_pages/ls1.html)
List Directory Contents
```ruby
ls
```
ls also Can be Used with Options :

* ```ls -a```  ```ls --all``` Show All Including Hidden Items

* ```ls -t``` Show and Sort Items by Time, Newest First

* ```ls -l``` Show Items Information Including Size, Permissions and Creation Time

Options Also Can be Used Together

* ```ls -l -t -a ``` Separated Options

* ```ls -lta``` Merged Options
  
### 2. [cd](https://linuxcommand.org/lc3_man_pages/cdh.html)
Change Directory

```ruby
cd folder_name              # Go to any Folder You Want
cd Downloads                # Go to Download Directory of Linux if It is Available in Where You are Now At
cd ~/Downloads              # Go to Download Directory of Linux from Wherever You are
cd /home/user/Downloads     # Go to Download Directory of Linux from Root Path
cd ..                       # Go to Previous Folder
cd .                        # Go to Working Directory, Not Useful for cd Command
```
### 3. Linux Path Addres Symbols

```/``` Root Directory, All Paths Start from This Directory Like ```/proc/cpuinfo``` is Where Your Cpu Information is 

```/home/ramtin/Desktop``` Absolute Path, Absolute Address from Only Root Directory, Address from First

```Desktop/Class/OS-Lab``` Relative Path, Relative Address from Wherever You Want, Address between Directories

```~``` User Home Directory, Where User's Directories are Like : Downloads, Desktop and ... Like ```cd ~/Desktop``` Goes to Desktop

```.``` Working Path Address Like : ```cp ./file ~/Desktop``` Copy file from Wherever You are to Desktop

```..``` Previous Directory Like : ```cd ../../../``` Changes Your Directory to Previous Directory 3 Times

### 4. [clear](https://man7.org/linux/man-pages/man1/clear.1.html)
Clears Your Terminal
```ruby
clear
```
### 5. [exit](https://linuxcommand.org/lc3_man_pages/exith.html)
Exits Your Terminal Shell Session
```ruby
exit
```
### 6. [mkdir](https://linuxcommand.org/lc3_man_pages/mkdir1.html)
Create Directory
```ruby
mkdir My_Directory
```
if You Want to Create Directory with Name that Contains Blank Character Like Space, Add ```\``` before each Space
```ruby
mkdir My\ Directory\ Number\ 3
```
if You Want to Create Multiple Directories at Once Write Names Next to each Other
```ruby
mkdir dir1 dir2 dir3 dir4
```
### 7. [touch](https://linuxcommand.org/lc3_man_pages/touch1.html)
Updates Last Opened Time and Accessed User Info of File (Main Usage is to Create File)
```ruby
touch index.html styles.css
```
### 8. [cat](https://linuxcommand.org/lc3_man_pages/cat1.html)
Show (Concatenate) Files and Print Contents in Terminal
```ruby
cat index.html
```
### 9. [nano](https://linuxcommand.org/lc3_man_pages/nano1.html)
Opens File Editor and Writes into Files
```ruby
nano index.html
```
After You Added Your Lines do ```ctrl + s``` to Save and then ```ctrl + x``` to Exit
### 10. [pwd](https://linuxcommand.org/lc3_man_pages/pwd1.html)
Prints Working Directory
```ruby
pwd
```
### 11. [rm](https://linuxcommand.org/lc3_man_pages/rm1.html)
Removes Files or Directories
```ruby
rm my_file.txt            # Removes File
rm -r My_Directory        # -r Option Removes Directories by Expanding each Directory Recursively and Remove Its Contents
```
### 12. [ln](https://linuxcommand.org/lc3_man_pages/ln1.html)
Creates a Link to a File
```ruby
ln folder1/file.txt folder2/linked_file.txt
```
### 13. [man](https://linuxcommand.org/lc3_man_pages/man1.html)
Manual Page, Shows Information of Command
```ruby
man ls
man cd
man man
```
### 14. [cp](https://linuxcommand.org/lc3_man_pages/cp1.html)
Copies File or Directory
```ruby
cp index.html ~/Desktop    # Copy index.html File to Desktop
cp -r Directory/ ~/Desktop # -r Option Copy Directories by Expanding each Directory Recursively and Copy Its Contents
```
### 15. [mv](https://linuxcommand.org/lc3_man_pages/mv1.html)
Moves File or Directory
```ruby
mv index.html ~/Desktop    # Moves index.html File to Desktop
mv Directory ~/Desktop     # Moves Directory, -r Option is Not Needed
```
### 16. [locate](https://linuxcommand.org/lc3_man_pages/locate1.html)
Find Files by Name, While Booting Up Your OS, All Your Hard Drive is being Loaded and All File Paths is being Writing to Linux Database of Paths and ```locate``` Will Find Inside this Database to Find File. So, Every Files That is Created After Booting Up is Not Detectable by Locate Unless You Update Your File Paths Database
```ruby
locate my_file.txt
```
### 17. [history](https://linuxcommand.org/lc3_man_pages/historyh.html)
Displays History of Commands You have Entered
```ruby
history
```
### 18. [find](https://linuxcommand.org/lc3_man_pages/find1.html)
Searchs for Files and Directory
```ruby
find . -name 'index.html'     # -name Option is Needed to Find File or Directory by Name
```
Remember that You Can Use any Other Path Instead of Using ```.``` Working Directory

## Week 7
### What is Shell ?
Shell is a ```command-line interface (CLI)``` that allows users to interact with the computer system by entering commands. Shell is gateway to the operating system's services and functions. in Unix-based operating systems like Linux, MacOS and ... there are several popular shells :
* [Bash](https://www.gnu.org/software/bash/) - Linux, MacOS
* [zsh](https://www.zsh.org/) - Linux, MacOS
* [Power Shell](https://learn.microsoft.com/en-us/powershell/) - Windows

### What is Bash ?
Bash (Bourne Again Shell) is a popular ```command-line interpreter``` or shell for Unix and Unix-like operating systems. It's the ```default``` shell for most Linux distributions and macOS.

### What is Terminal ?
Terminal is a software interface that allows users to interact with a computer system using text-based commands ```(I/O)```. It provides a way to enter shell commands to the operating system and receive textual output.

### What is Shell Script
Shell Script is a ```script or program``` written in a scripting language that is interpreted by a shell, such as ```Bash``` in Unix-like operating systems. Shell scripts are used to ```automate tasks```, ```execute commands```, and perform ```system administration tasks```.

### Why ```Everything in Linux is File``` ?
The principle that "everything is a file" is a fundamental concept in Unix-like operating systems, including Linux. It embodies the idea that in the Unix/Linux environment, various system resources are represented as files or file-like objects. This simplifies the design and usage of the operating system, as it allows uniform access and manipulation of different resources through a common interface.
for example :
* Your computer's webcam is a file (located at ```/dev/video0```)
* Your mouse and keyboard (located at ```/dev/input/by-id/```)
* Your ls command (located at ```/usr/bin/ls```)
* Your SSD (located at ```/dev/disk/by-id```)
