# Linux Commands Handbook

## Introduction to Linux and shells

### The Linux man command

#### Description:
The man command displays the manual pages for other commands. It provides detailed information about command syntax, options, and usage.

#### Example: man ls

### The Linux ls command

#### Description:
ls is used to list files and directories in the current directory. It displays information such as file permissions, ownership, size, and modification date.

#### Example: ls -l


### The Linux cd command

#### Description:
cd is used to change the current working directory. You can use it to navigate to different directories within the file system.

#### Example: cd /path/to/directory


### The Linux pwd command

#### Description:
pwd stands for "print working directory." It displays the full path of the current working directory.

#### Example: pwd


### The Linux mkdir command

#### Description:
mkdir is used to create new directories (folders) within the file system.

#### Example: mkdir new_directory


### The Linux rmdir command

#### Description:
rmdir is used to remove empty directories from the file system.

#### Example: rmdir empty_directory


### The Linux mv command

#### Description:
mv is used to move files or directories from one location to another. It can also be used to rename files or directories.

#### Example: mv file1.txt /path/to/destination


### The Linux cp command

#### Description:
cp is used to copy files or directories from one location to another.

#### Example: cp file1.txt /path/to/destination


### The Linux open command

#### Description:
This command is not standard in Linux. It might refer to opening files or directories in a graphical file manager.

## Text Processing and Viewing

### The Linux touch command

#### Description:
touch is used to create new empty files or update the timestamps of existing files. It's commonly used to create placeholder files or update file timestamps.

#### Example: touch new_file.txt


### The Linux find command

#### Description:
find is used to search for files and directories in the file system based on various criteria such as file name, size, permissions, and modification time.

#### Example: find /path/to/search -name "*.txt"



### The Linux ln command

#### Description:
ln is used to create links between files. There are two types of links: hard links and symbolic links (also known as soft links).

#### Example: ln -s /path/to/file symbolic_link


### The Linux gzip command

#### Description:
gzip is used to compress files. It reduces the size of files by replacing repetitive sequences of characters with shorter codes.

#### Example: gzip file.txt


### The Linux gunzip command

#### Description:
gunzip is used to decompress files that have been compressed with gzip.

#### Example: gunzip file.txt.gz


### The Linux tar command

#### Description:
tar is used to create and manipulate archive files (tarballs). It can bundle multiple files and directories into a single archive file, which can then be compressed with gzip or another compression tool.

#### Example: tar -cvf archive.tar file1.txt file2.txt


### The Linux alias command

#### Description:
alias is used to create shortcuts or aliases for frequently used commands. It allows users to define custom shorthand commands for longer or complex commands.

#### Example:alias ll='ls -l'


### The Linux cat command

#### Description:
cat is used to concatenate and display the contents of files. It can also be used to create new files or append content to existing files.

#### Example: cat file.txt


### The Linux less command

#### Description:
less is a pager program used to view the contents of text files one page at a time. It allows scrolling forward and backward through files, searching for text, and navigating to specific line numbers.

#### Example: less file.txt


### The Linux tail command

#### Description:
tail is used to display the last few lines of a text file. It's commonly used to monitor log files in real-time or extract the most recent entries from large files.

#### Example: tail -n 10 file.log


### The Linux wc command

#### Description:
wc is used to count the number of lines, words, and characters in a text file. It can also be used to count the number of bytes in a file.

#### Example:  wc file.txt


### The Linux grep command

#### Description:
grep is used to search for text patterns in files. It's a powerful tool for pattern matching and is commonly used in combination with other commands and utilities.

#### Example: grep "pattern" file.txt


### The Linux sort command

#### Description:
sort is used to sort the lines of text files alphabetically or numerically. It can also be used to merge and compare sorted files.

#### Example: sort file.txt


### The Linux uniq command

#### Description:
uniq is used to filter out adjacent duplicate lines from a sorted text file. It's often used in combination with the sort command to remove duplicate entries.

#### Example: uniq file.txt


### The Linux diff command

#### Description:
diff is used to compare the contents of two text files and display the differences between them. It highlights added, deleted, and modified lines.

#### Example: diff file1.txt file2.txt


### The Linux echo command

#### Description:
echo is used to display text or variables on the terminal. It's commonly used in shell scripts to print messages or output variable values.

#### Example: echo "Hello, World!"


### The Linux chown command

#### Description:
chown is used to change the ownership of files and directories. It allows users to transfer ownership from one user to another or change group ownership.

#### Example: chown user:group file.txt


### The Linux chmod command

#### Description:
chmod is used to change the permissions of files and directories. It allows users to specify who can read, write, or execute a file.

#### Example:chmod 755 file.txt


### The Linux umask command

#### Description:
umask is used to set default file permissions for newly created files. It masks out certain permissions from being granted by default.

#### Example: umask 022


### The Linux du command

#### Description:
du is used to estimate the disk usage of files and directories. It displays the disk space occupied by each file and directory in a human-readable format.

#### Example: du -sh directory/


### The Linux df command

#### Description:
df is used to display information about disk space usage on filesystems. It shows the total, used, and available disk space on mounted filesystems.

#### Example: df -h


### The Linux basename command

#### Description:
basename is used to extract the filename from a given path. It removes any directory components and returns only the base name of the file.

#### Example: basename /path/to/file.txt


### The Linux dirname command

#### Description:
dirname is used to extract the directory component from a given path. It removes the filename and returns only the directory name.

#### Example: dirname /path/to/file.txt


## Process Management

### The Linux ps command

#### Description:
ps is used to display information about currently running processes. It shows process IDs, CPU and memory usage, and other details.

#### Example: ps aux


### The Linux top command

#### Description:
top is an interactive process viewer that displays a list of running processes and system resource usage in real-time. It's commonly used to monitor system performance.

#### Example: top


### The Linux kill command

#### Description:
kill is used to send signals to processes. By default, it sends the SIGTERM signal to gracefully terminate a process, but it can also send other signals for different purposes.

#### Example: kill PID


### The Linux killall command

#### Description:
killall is used to send signals to multiple processes by name. It terminates all processes with the specified name or sends a signal to them.

#### Example: killall process_name


### The Linux jobs command

#### Description:
jobs is used to display the status of background jobs in the current shell session. It shows a list of running or stopped background processes.

#### Example: jobs


### The Linux bg command

#### Description:
bg is used to resume a stopped background job and run it in the background. It's often used in combination with the jobs command.

#### Example: bg %job_number


### The Linux fg command

#### Description:
fg is used to bring a background job to the foreground and make it the active process. It's commonly used to interact with background processes.

#### Example: fg %job_number


## Command Information

### The Linux type command

#### Description:
type is used to display information about command types. It shows whether a command is a shell built-in, an alias, a function, or an external executable.

#### Example: type ls

### The Linux which command

#### Description:
which is used to locate the executable file associated with a given command. It displays the full path of the command if it's found in the system's PATH directories.

#### Example: which ls


## System Information

### The Linux nohup command

#### Description:
nohup is used to run a command immune to hangups (hup), meaning it allows a command to continue running even after the user logs out or the terminal is closed.

#### Example: nohup command &


### The Linux xargs command

#### Description:
xargs is used to build and execute commands from standard input. It's often used to process a list of items or filenames passed as input.

#### Example: echo "file1 file2 file3" | xargs rm


### The Linux vim editor command

#### Description:
vim is a powerful text editor that is highly customizable and comes with many features for editing text files, writing code, and more.

#### Example: vim filename.txt


### The Linux emacs editor command

#### Description:
emacs is another popular text editor that is highly extensible and comes with a wide range of features for editing text, writing code, and even browsing the web.

#### Example: emacs filename.txt


### The Linux nano editor command

#### Description:
nano is a simple and easy-to-use text editor that is ideal for beginners. It's lightweight and comes with basic editing features for editing text files.

#### Example: nano filename.txt


## User and Authentication

### The Linux whoami command

#### Description:
whoami is used to display the username of the current user. It prints the effective user ID associated with the current user session.

#### Example: whoami


### The Linux who command

#### Description:
who is used to display information about users who are currently logged into the system. It shows their usernames, terminal sessions, login times, and more.

#### Example: who


### The Linux su command

#### Description:
su is used to switch to a different user account. It allows users to execute commands as another user, typically the root user, after providing the correct password.

#### Example: su username


### The Linux sudo command

#### Description:
sudo is used to execute commands with superuser (root) privileges. It allows authorized users to perform administrative tasks without logging in as the root user.

#### Example: sudo command


## Network and Connectivity

### The Linux ping command

#### Description:
ping is used to test the reachability of a host on a network by sending ICMP echo request packets and waiting for ICMP echo reply packets.

#### Example: passwd


## Network and Connectivity

### The Linux ping command

#### Description:
ping is used to test the reachability of a host on a network by sending ICMP echo request packets and waiting for ICMP echo reply packets.

#### Example: ping example.com


### The Linux traceroute command

#### Description:
traceroute is used to trace the route that packets take from the local host to a specified destination host. It shows the IP addresses of routers along the path.

#### Example: tracert example.com


## Terminal Navigation and Management

### The Linux clear command

#### Description:
clear is used to clear the terminal screen. It removes all previous output from the terminal and scrolls the screen to the top.

#### Example: clear


### The Linux history command

#### Description:
history is used to display a list of previously executed commands in the current shell session. It shows command numbers and allows users to re-execute commands by their numbers.

#### Example: history



### The Linux export command

#### Description:
export is used to set environment variables in the current shell session. It allows users to define variables that are accessible to child processes.

#### Example: export PATH=$PATH:/new/path


### The Linux crontab command

#### Description:
crontab is used to schedule recurring tasks (cron jobs) on Linux systems. It allows users to define commands or scripts that run at specified times or intervals.

#### Example: crontab -e


### The Linux uname command

#### Description:
uname is used to display system information about the current operating system. It shows details such as the system name, kernel version, machine architecture, and more.

#### Example: uname -a


### The Linux env command

#### Description:
env is used to display the current environment or set environment variables for executing a command. It shows a list of environment variables and their values.

#### Example: env


### The Linux printenv command

#### Description:
printenv is used to display the values of environment variables. It shows a list of all environment variables and their current values.

#### Example: printenv



















































