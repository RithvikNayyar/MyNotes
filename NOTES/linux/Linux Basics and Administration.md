#### Linux Basics - Introduction

**What is an Operating System (OS)?**
- An operating system (OS) is essential software that manages a computer’s hardware and software resources.  
- It acts as an intermediary between users and the physical components of the computer.  
- The OS handles key tasks such as memory allocation, process scheduling, file management, and device control.  
- These functions allow applications to run smoothly and efficiently.  
- Without an OS, programs like web browsers, games, or word processors could not interact with hardware such as the CPU, RAM, or storage devices.  
- The OS provides a user interface, which can be a graphical user interface (GUI) or a command-line interface (CLI).  
- This interface enables users to interact with the computer easily and perform various tasks.
___

**What is Linux?** 
- It is an open source software, Unix-like operating system kernel released in 1991 by Linus Torvalds.
- It acts as the core part of an operating system, managing hardware resources and enabling communication between software and the computer's physical components.
- Linux is the foundation for many operating systems knows as Linux distributions, such as Ubuntu, Debian (currently using). Fedora, Cent OS, etc.
- It is free to use, modify, and distribute, thanks to open-source licensing.
- Linux is stable, secure and efficient, making it a top choice for servers, cloud computing, and development environments.It is widely used in web hosting, networking, cyber-security, programming, and embedded systems due to its reliability and performance.
- It supports multitasking, multi-user operations, and runs on wide variety of hardware.
- Linux provide full transparency and customization of the system unlike mac or windows.
___

**What is root?**
- In Linux and UNIX operating systems, root refers to the most powerful user account on the system, often called superuser.
- This account has complete control over the entire system and can perform any action, regardless of restrictions that apply to regular users.
- The root user can modify system files, install or remove software, change permissions for users, manage hardware and configure critical settings.
- By default, root access is restricted as it is very dangerous for security reasons, and administrative tasks and performed using commands like `sudo`, which temporarily, grants privileges to the trusted users.
___
#### Working on Linux - System Access and File system

**Changing passwords in Linux:**
- To change password we use command `passwd` in terminal. The process is very simple
- Open terminal and type the command and enter your existing password, and type your new password along with confirm password.
- The system will update your password if both entries match and meet security requirements.
- If you are logged in as root then you can change other user's password.
___

**Linus file system:**
- Linux uses a unified, tree-like file system that starts from the root directory (`/`).
- Everything in Linux is treated as a file like regular files, directories, devices, and even processes.
- The file system is case-sensitive and supports various types such as `ext4`, ` XFS `, `BTRFS`, more.
___

**Linux Structure & Description:**
- The top level directory is `/` with is root directory, from which all other directories branch out.
- Key directory include:
	- `/bin` - essential user commands binaries (e.g., `ls, cp`)
	- `/etc` - configuration files for the system and applications
	- `/home` - personal directories for user
	- `/root` - home directory for root user
	- `/tmp` - temporary files (cleared on reboot)
	- `/usr` - secondary hierarchy for user programs libraries, documentation
	- `/var` - variable data like logs, database, emails
	- `/dev` - Device files (e.g., hard drives, terminals)
	- `/proc` - virtual file-system providing process and kernel information
	- `/boot` - files needed to boot the system (kernel, boot-loader)
___

**File-System Navigation Commands:** 
- `pwd` - Display the current working directory.
- `cd <dir>` - changes the current directory
- `cd ..` - moves one level up in the directory tree.
- `cd~` or `cd` - returns to the user's home directory.
- `ls` - lists directory contents; use `ls -a` to show hidden files and `ls -l` for detailed view.
___

**File or Directory Properties:** 
- Use `ls -l` to view properties: file type, permissions, number of links, owner, group, size, date (last modified), and name.
- Permissions are shown as `rwx` for read, write, and execute, and grouped by owner, groups, and others. 
- E.g., `drwxr-xr--`, `d` - directory, starts with owner ` rwx ` means he has full read, write and execute permission. Second comes with group, has `r-x` means he has read and execute permission. Third comes `r--` for others, means they have permission to read and nothing else.
- Each file has an Inode number that stores metadata about he file.
___

**Absolute and Relative Path:** 
- An absolute path starts from the root (`/`) and gives the full location (e.g., `/home/user/Documents/report.txt`).
- A relative path is relative to the current working directory (e.g., `Documents/report.txt` or `../Pictures/image.jpg`).
- `.` represents the current directory; `..` represents the parent directory.
___

**Creating Files and Directories (`touch`, `cp`, `vi or vim`, `mkdir`):** 
- `touch filename` - Creates an empty file or updates the timestamp of an existing file.
- `mkdir dirname` - Creates a new directory; use `mkdir -p dir/subdir` to create a nested directories.
- `cp source destination` - copies files or directories; use `-r` flag to copy directories recursively.
- `vi` or `vim` - text editors used to create or modify files; `vim filename` opens the file in editor mode.
___

**Wildcards:**
- `*` -- matches any number of characters (e.g., `*txt` matches all text files).
- `?` - matches exactly one character(e.g., `file?.log` matches `file1.log`, `fileA.log`).
- `[]` - matches any one character within brackets (e.g., `[abc].txt` matches `a.txt`, `b.txt`, `c.txt`).
- Used for pattern matching in commands like `ls`, `rm`, `cp`.
___

**Find and locate command:**
- `find/path-name "filename"` - Searches for files in real-time based on name, type, size or time(e.g., `find /home -name "*.pdf"`).
- `find` can also search by size (`-size`), modification time(`-mtime`), and permission (`-prem`) 
- `locate filename` - quickly finds files by searching a pre-built database (`updatedb`); faster than `find` but may miss recently added files.
- Run `sudo updatedb` to refresh the locate database.
- Some Linux distributions does not support `locate` command by default and needs to be installed by `sudo apt install locate` - Debian command only. 
___

**Soft-link:**
- A soft link is a shortcut pointing to another file or directory, created with `ln -s target linkname`.
- Soft link can span across file systems and have different inode numbers; they break if the original file is deleted.
**Hard-Link:**
- A hard link points directly to the same inode as the original file, created with `ln target linkname`.
- Hard links cannot point to directories and must stay within the same file system; they remain valid even if the original name is removed.
- Deleting the original file does not affect a hard link - it still accesses the same data.
___

#### Linux - Fundamentals

**What is Linux command syntax?**
- Linux command syntax follows a standard structure: 
  `command [option][auguments]`.
- The command is name of the program or action to execute:
  (e.g., `ls`, `cp`, `mkdir`).
- Options modify the behaviour of the command, usually starting with a dash `(-)` for short options (e.g., `-l`, `-h`) or double dash (`--`) for long options (e.g., `help`, `--human-readable`).
- Arguments are the targets the command acts on, such as filename, directories or user names (e.g., `file.txt`, `/home/user`).
- Options and arguments are optional depending on the command, but some commands require arguments to work.
- Multiple options can be combined after a single dash (e.g., `ls -la` is same as `ls -l -a`).
- Spaces are important; Each part of the command must be separated by spaces.
- You can chain command options like `;`, `&&`, or `||`, or use pipes (`|`) to pass output from one command to another.
- If a file directory contains spaces then enclose it with quotes:
  (e.g., `cat "my file.txt"`).
- Always press `Enter` to execute the command, and the shell will process it and display output he errors.
___

**Files and Directory Permissions (`chmod`):**
- Linux uses permissions to control access to files and directories.
- Each file has three types of permissions: 
  read (`r`), write (`w`), and execute (`x`).
- Permissions are set separately for three categories:
  Owner, group, and others.
- Use `chmod` to change permissions. For example: `chmod g+w file.txt` adds write permission for the group.
- Execute permission is required for running scripts or entering directories.
___

**File Permission Using Numeric Mode:**
- Permissions can be set using numbers (octal mode):
  `read (r) = 4`, `write (w) = 2`, and `execute (x) = 1`.
- Sum value to combine permissions:
  `rwx =7`, `rw- = 6`
- Specify three digits for owner, group and others. Example:
  `chmod 755 script.sh` gives owner `rwx`, group and other `r-x`.
- Here is the correct list from 0 to 7:
    - `0` = no permissions (`---`)
    - `1` = execute only (`--x`)
    - `2` = write only (`-w-`)
    - `3` = write and execute (`-wx`)
    - `4` = read only (`r--`)
    - `5` = read and execute (`r-x`)
    - `6` = read and write (`rw-`)
    - `7` = read, write, and execute (`rwx`)
___

**File Ownership Commands (chmod, chgrp):**
- Use `chown user:groupfile` to change both owner and group of a file.
  Example: `chmod alice:developers app.log`
- Change owner only: `chown:developers file.txt` or use `chgrp developers file.txt`.
- Only root or file owner can change ownership.
- Use `-R` flag to apply change recursively to directories.
___

**Access Control List (ACL):**
- ACL allows setting more detailed permissions beyond standard Unix permissions.
- Enable extended permissions on a file system using `mount -o acl/partition`.
- Use `setfacl` to add specific permissions for user or groups.
  Example: `setfacl -m u:alice:rw file.txt`.
- View ACL settings with `getfacl filename`
- ACL is useful when fine-grained access control is needed for multiple users or groups.
___

**Help command:**
- Use `--help` with most commands to display basic usage.
  Example: `ls --help`
- The `man` Command shows detailed manual pages.
  Example: `man chmod`.
- Use `info` for structured, in - depth documentation.
  Example: `info coreutils`.
- `apropos` searches for commands by keyword.
  Example: `apropos "copy file"`.
- These tools help understand syntax, options and examples directly from the terminal.
___


