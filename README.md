# Essential Linux Commands

This guide provides an overview of essential Linux commands for managing files, processes, permissions, and system information.

## File and Directory Management
- **`ls`** - List directory contents. `ls -l /home`
- **`cd`** - Change directory. `cd /var/log`
- **`pwd`** - Print working directory. `pwd`
- **`cp`** - Copy files or directories. `cp file.txt /backup`
- **`mv`** - Move or rename files or directories. `mv old_name.txt new_name.txt`
- **`rm`** - Remove files or directories. `rm file.txt`
- **`mkdir`** - Create a new directory. `mkdir new_folder`
- **`rmdir`** - Remove empty directories. `rmdir empty_folder`

## Searching and Editing
- **`grep`** - Search text using patterns. `grep "hello" file.txt`
- **`find`** - Search for files in a directory hierarchy. `find /home -name "note.txt"`

## Permissions and Ownership
- **`chmod`** - Change file permissions. `chmod 755 script.sh`
- **`chown`** - Change file owner and group. `chown user:group file.txt`

## System Monitoring
- **`ps`** - Report a snapshot of current processes. `ps aux`
- **`top`** - Task manager. `top`
- **`df`** - Display disk space usage. `df -h`
- **`du`** - Estimate file space usage. `du -sh /home`

## Text Editing
- **Text Editors (`nano`, `vi`, `emacs`)** - Edit files using a text editor. `nano file.txt`

## Archiving and Network
- **`tar`** - Archive files. `tar -czvf archive.tar.gz /folder`
- **`wget`** - Non-interactive network downloader. `wget http://example.com/file.iso`
- **`ssh`** - Secure Shell client. `ssh user@192.168.1.100`

Feel free to explore these commands to enhance your Linux skills and manage your systems more effectively.
