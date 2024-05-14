# Operating System Lab - Commands
This Repository Contains a Collection of Linux Commands Taught in each OS Lab Class Separated by Weeks

Table of Contents
* [Week 1 to 6](#week-1-to-6)
* [Week 7](#week-7)
* [Week 8](#week-8)
* [Week 9](#week-9)
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

### How to Write Shell Script ?
1. Open your terminal and create a new file like ```touch my_script.sh```. You can name it whatever you like, but make sure it has a ```.sh``` extension to indicate it's a ```shell script```.
2. Use any text editor you are comfortable with, for example use nano
3. The ```first line``` of your script should be the ```shebang line```. This tells the system which ```interpreter``` to use to run the script. For a ```Bash``` shell script, use :
```bash
#!/bin/bash
```
4. Add the commands you want to execute. Here’s an example script that create new file named file.txt and directory named copy_here and then copy file.txt to copy_here directory :
```bash
#!/bin/bash

touch file.txt
mkdir copy_here
cp file.txt copy_here
```
5. save your file
Now you have created a shell script.


### How to Run (Execute) Shell Script ?
Before you can run the script, you need to make it executable. Use the chmod command to do this :
```sh
chmod +x my_script.sh
```
but what is ```chmod``` and ```+x``` ?  
In Unix-like operating systems (like Linux), every file and directory has a set of permissions that determine who can read, write, or execute the file  
There are three types of permissions:
* Read (r): Permission to read the file.
* Write (w): Permission to modify the file.
* Execute (x): Permission to run the file as a program.
for example if you do command ```ls -l``` that shows lsit of file as detailed list, you see this line for ```my_script.sh``` :
```sh
ls -l

-rw-rw-r-- 1 qb qb 0 May 14 08:30 my_script.sh
```
First part ```-rw-rw-r--```'s 3-charactered section ```rw-``` only has ```r``` and ```w```, it means my_script.sh can be writen or read but not execute because execute part is ```-```. to add execute permission you must do that ```chmod +x my_script.sh``` command, if you that you will see this instead :
```sh
ls -l

-rwxrwxr-x 1 qb qb 0 May 14 08:30 my_script.sh
```
Now you can see execute permission ```x``` has been added to file and it can be seen like ```rwx``` instead ```rw-```, that means my_script.sh can be run in terminal like this :
```sh
./my_script.sh
```
that ```./``` at first shows current directory ```.``` explained in [this part](#3-linux-path-addres-symbols). It can be other path if you are not inside my_script.sh's directory like :
```bash
# - Home path
~/Desktop/my_script.sh
# - or full path (needed in systemd services projects)
/home/qb/Desktop/my_script.sh
```

### Why i can not use ```my_script.sh``` to run my script instead of ```./my_script.sh```
When you try to run a script using my_script.sh instead of ./my_script.sh, your shell looks for the script in the directories listed in your ```PATH environment variable```. If the ```current directory (.)``` is not in your PATH, the shell ```won't find the script```.

### Linux Commands
* [echo](#19-echo)
* [grep](#20-grep)

### 19. [echo](https://www.geeksforgeeks.org/echo-command-in-linux-with-examples/)
The echo command is a basic command-line utility in Unix and Unix-like operating systems that prints the specified arguments to the standard output. It is commonly used to display text or variables in shell scripts or interactively in a terminal session :
```bash
echo "Hello, world!"
```

### 20. [grep](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
The grep command is a powerful tool used in Linux and Unix-like operating systems for searching ```text patterns``` within files or ```streams of input```.  
Examples :
1. Search text or pattern (here hello) in file
```bash
grep "hello world" file.txt
```
Common Options :
* -i: Ignore case distinctions.
```bash
grep -i "hELlO WOrlD" file.txt
```
* -r, -R: Recursively search subdirectories listed.
```bash
grep -r "hello world" directory/
```
* -n: Display line numbers along with matched lines.
```bash
grep -n "hello world" file.txt
```
* -v: Invert the match, i.e., display non-matching lines.
```bash
grep -v "bye world" file.txt
```
* -c: Only count the number of matching lines. (Here shows amount of your cpu cores)
```bash
grep -c "processor" /proc/cpuinfo
```
* -E: Interpret the pattern as an extended regular expression (ERE). (Here will shows lines that are mails and their extention is @gmail.com)
```bash
grep -E '\b[A-Za-z0-9._%+-]+@gmail\.com\b' emails.txt

# - \b: Matches a word boundary, ensuring that the pattern matches complete email addresses and not partial ones.
# - [A-Za-z0-9._%+-]+: Matches one or more characters that can appear in the local part of an email address. This includes letters (upper and lower case), digits, and special characters commonly allowed in email addresses.
# - @gmail\.com: Matches the domain part of a Gmail address.
# - \b: Matches another word boundary, ensuring that the pattern matches complete email addresses and not partial ones.
```

## Week 8
Review learned lessons and do some class exercises

## Week 9
### Variables
Like programming languages there are variables that we can store numbers, texts and other data types to them to use in our program. in Linux, variables are like that and used extensively in ```scripting``` and ```system configurations```.

### How to Define a Variable ?
Variables are assigned values using the ```= operator```. For example :
```bash
name="Lida"
age=22
major="computer engineering"
```
⚠️ You can define your variables everywhere that use bash, like your ```terminal``` or ```shell script``` file  
⚠️ In shell scripting, variable assignments ```shouldn't have spaces``` around the = sign :
```bash
age = 22    # - Will error
age=22      # - Will assign 22 to age
```

⚠️ Variable names in Linux are case-sensitive and can consist of letters, numbers, and underscores. By convention, variable names are usually in uppercase, especially for environment variables, to distinguish them from other variables and constants :
```bash
age=22
AGE=44
# - age is not AGE
```

### How to Access Value of Variables ?
To access the value stored in a variable, you prepend a $ to its name. For example :
```bash
name="Neda"
echo "My name is $name"
```

### ```$``` Usages
There are several usages for ```$``` in bash :
* Variable Expansion ```$```
Accesses the value stored in a variable :
```bash
text="Hello World"
echo $text
```
* Command Substitution ```$()```
Executes a command and replaces the command with its output.
```bash
file_name="emails.txt"
echo "File $file_name has $(grep -c '@gmail' $file_name) mails available inside it"
```
* Arithmetic Expansion ```$(())```
Evaluates an arithmetic expression and returns the result. Remember that inside ```$(())``` there is no need to use ```$``` to access value of variables, you can only write their names.
```bash
num1=20
num2=30
sum=$((num1 + num2))
echo "$num1 + $num2 = $sum"
# - or you can do this inside string :
echo "$num1 + $num2 = $((num1 + num2))"
```

### Curly Braces ```${}```
The curly braces ```{}``` are used to clearly delimit the variable name from surrounding text. For instance :
```bash
name="Zhila"
```
Without the braces, Bash might not interpret the variable correctly if it is followed by characters that are part of the variable name. Compare :
```bash
echo "Hello, $name!"
echo "Hello, $name1"
echo "Hello, ${name}1"
```
Curly braces can also be used for parameter expansion, which provides more advanced features :
* Length of the Variable's Value
```bash
text="Hello World"
echo ${#text}       # - Will Show 10 (Length of text)
```
* Substring Extraction
```bash
text="Hello World"
echo ${text:0:5}    # - Will Show 'Hello ' (from Index 0 to 5)
```

### Bash Conditional Statements
In Bash, conditional statements are used to perform different actions based on whether certain conditions are true or false. The if statement is a primary construct for this purpose. Here is how you can use if statements in Bash :
* Basic Syntax
```bash
text1="hello"
text2="hello"

if [ $text1 == $text2 ]; then
    echo "text1 and text2 are same"
fi
```
* Using ```if-else```
```bash
text1="hello"
text2="bye"

if [ $text1 == $text2 ]; then
    echo "text1 and text2 are same"
else
    echo "text1 is not equal to text2"
fi
```
* Using ```if-elif-else```
```bash
text1="how are you ?"
text2="bye"
text3="how are you ?"

if [ $text1 == $text2 ]; then
    echo "text1 and text2 are same"
elif [ $text1 == $text3 ]; then
    echo "text1 and text3 are same"
else
    echo "text1 is not equal to text2"
fi
```

### Types of Conditions
Conditions in Bash can include comparisons, file tests, and string tests. Here are some common examples :
* Comparison Operators (Used for Numbers)
   * ```-eq``` equal to
   * ```-ne``` not equal to
   * ```-lt``` less than
   * ```-le``` less than or equal to
   * ```-gt``` greater than
   * ```-ge``` greater than or equal to
* String Operators
   * ```==``` equal to
   * ```!=``` not equal to
   * ```-z``` string is null (has zero length)
   * ```-n``` string is not null (has non-zero length)
* File Test Operators
   * ```-e``` file exists
   * ```-d``` file is a directory
   * ```-f``` file is a regular file
* Logical Operators
   * ```&&``` Logical AND
   * ```||``` Logical OR
   * ```!``` Logical NOT

Examples :
* Comparison Operators
```bash
num=7

if [ $num -gt 10 ]; then
    echo "The number is greater than 10"
elif [ $num -gt 5 ]; then
    echo "The number is greater than 5 but less than or equal to 10"
else
    echo "The number is 5 or less"
fi
```
* String Operators
```bash
str="hello"

if [ "$str" = "hello" ]; then
    echo "The string is hello"
else
    echo "The string is not hello"
fi
```
* File Test Operations
```bash
file="example.txt"

if [ -e "$file" ]; then
    echo "The file exists"
else
    echo "The file does not exist"
fi
```
* Using ```(())``` for Mathematical Conditions Instead of Using Brackets
```bash
num1=20
num2=30

if ((num1 < num2)); then
   echo "num1 is lower than num2"
elif ((num1 > num2)); then
   echo "num1 is higher than num2"
else
   echo "num1 is equal to num2"
fi
```

### Advanced Conditions
For more complex conditions, you can use double brackets ```[[ ]]``` :
```bash
if [[ $num -gt 5 && $num -lt 15 ]]; then
    echo "The number is between 5 and 15"
fi
```
Also you can use this if you don't want to use double brackets :
```bash
if [ $num -gt 5 ] && [ $num -lt 15 ]; then
    echo "The number is between 5 and 15"
fi
```

### Common Conditional Statements Mistakes
* No Spaces Around Condition
Be careful that there should be spaces between the square brackets and the condition like ```[ condition ]```, bash does not support ```[condition]```.
* Using == for Numeric Comparison
Use ```-eq```, ```-ne```, ```-lt```, ```-le```, ```-gt```, ```-ge``` for numeric comparisons
```bash
# - Incorrect for Numbers
if [ $num == 10 ]; then
# - Correct for Numbers
if [ $num -eq 10 ]; then
```
* Quoting Strings
Always quote string variables to avoid issues with spaces or special characters
```bash
str="hello world"
# - Incorrect
if [ $str = "hello world" ]; then
# - Correct
if [ "$str" = "hello world" ]; then
```
* Semicolon ```;``` at the end of condition brackets  
Remember to use ```;``` at close bracket like ```[ condition ]; then```

<!--
## Week 10
### Special Variables
Linux also has special variables like $0 (the name of the script), $1, $2, etc. (for script arguments), and $? (the exit status of the last command).

### Variable Scope
Variables in shell scripts have scope, meaning they are only accessible within the script or the shell session in which they are defined unless they are exported.

### types of variable (user-defined and environment)
Environment Variables: These are variables that are available system-wide and can be accessed by all processes. They are usually set in configuration files like .bashrc, .bash_profile, or in scripts. Common environment variables include PATH, HOME, USER, etc.

User-defined Variables: These are variables created by users within shell scripts or directly in the shell environment. They can be used to store temporary data or configuration values.


### What is Process Environment ?

### Exporting Variables

### for, while


-->
