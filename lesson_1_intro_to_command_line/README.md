# Linux Lesson #1 - Intro to the Command Line
The command line is your friend in linux. Understanding how to use the command line in your day to day workflows will make you more efficient and process work more quickly.
This lesson will be based on GNU bash version 5 with content based on Ubuntu 20.04

## Ideas Covered in this Lesson
- Important directories
- navigating directories
- tab completion

### Important directories
- /
    - This is the root directory, the start of the filesystem
- /bin
    - Essential binaries
- /dev
    - Device files (everything is a file in linux)
- /etc
    - System wide configuration files
- /home
    - User home folders where user local settings/configurations are stored along user files (Documents, Downloads, Pictures, etc...)
- /lib
    - Essential libraries for binaries in /bin and /sbin 
- /media
    - Removable media
- /mnt
    - Mounted file systems
- /opt
    - Optional packages
- /proc
    - Kernel and process files
- /root
    - root user home folder
- /usr
    - User binaries and read only data
- /tmp
    - Temporary files
- /var
    - Variable data like log files, mysql data, docker etc...

### Basic navigation
- `$` in the shell mean you are in non-priveleged mode while `#` means you're in privileged mode
- `cd` (change directory)
    - `cd ..` (go up one directory)
    - `cd path/to/destination`
    - `cd ~` (go to home directory)
- `pwd` (get current directory)
- `readlink -e filename` (get full path of file)

### Commands
Everything you do on the command line is recorded in ~/.bash_history and can be recalled with the `history` command
- `!!` will run the last command (up arrow will also get last command)
- `history` has line numbers and a specific command can be called by `!LINENUMBER`
- `!partial_command` will run the most recent command that matches the letters typed
    - Example: `!s` will match most recent command like `sudo -u www-data /run/this`


### File and Folder Commands
- touch
- mkdir (makes a directory)
- rm
- rmdir