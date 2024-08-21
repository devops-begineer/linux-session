# Essential Linux Commands Cheat Sheet

This guide offers a quick reference to essential Linux commands, their usage, and examples.

## File and Directory Management

### `ls -lrta`
List directory contents, including hidden files, in reverse chronological order.
- **Usage**: `ls [options] [file...]`
- **Examples**:
  ```bash
  ls -lrta  # Lists all files, including hidden ones, sorted by modification time in reverse order.

### `cp`

Copy files or directories from one location to another.

    Usage: cp [options] source destination
    Examples:

    bash

    cp source.txt destination.txt  # Copy a file to another location.
    cp -r source_dir/ destination_dir/  # Copy a directory and its contents.

### `mv`

Move or rename files or directories.

    Usage: mv [options] source destination
    Examples:

    bash

    mv old_name.txt new_name.txt  # Rename a file.
    mv file.txt ~/Documents/  # Move a file to a different directory.

### `mkdir`

Create a new directory.

    Usage: mkdir [options] directory...
    Examples:

    bash

    mkdir new_directory  # Create a new directory.

### `rmdir`

Remove empty directories.

    Usage: rmdir [options] directory...
    Examples:

    bash

    rmdir old_directory  # Remove an empty directory.

### `touch`

Create empty files or update the timestamps of existing files.

    Usage: touch [options] file...
    Examples:

    bash

    touch new_file.txt  # Create a new empty file.

### `vi, vim, nano`

Create or edit files using text editors.

    Examples:

    bash

    vi file.txt   # Edit file using vi.
    vim file.txt  # Edit file using vim.
    nano file.txt # Edit file using nano.

### `shred`

Delete files securely by overwriting them multiple times.

    Usage: shred [options] file...
    Examples:

    bash

    shred -u sensitive_data.txt  # Securely delete and overwrite a file.

### `grep`

Search for patterns within files.

    Usage: grep [options] pattern [file...]
    Examples:

    bash

    grep 'search_term' file.txt  # Search for 'search_term' in a file.

### `egrep (or grep -E)`

Search for extended regular expressions in files.

    Usage: egrep [options] pattern [file...]
    Examples:

    bash

    egrep 'term1|term2' file.txt  # Search for 'term1' or 'term2' in a file.

### `find`

Search for files in a directory hierarchy.

    Usage: find [path...] [expression]
    Examples:

    bash

    find /home -name "*.txt"  # Find all .txt files under /home directory.

### `chmod`

Change file modes or Access Control Lists.

    Usage: chmod [options] mode file...
    Examples:

    bash

    chmod 755 script.sh  # Change permissions to rwx for owner and rx for group and others.

### `chown`

Change file owner and group.

    Usage: chown [options] owner[:group] file...
    Examples:

    bash

    chown user:group file.txt  # Change the owner and group of a file.

### `gzip / gunzip`

Compress or decompress files using GNU zip.

    Examples:

    bash

    gzip file.txt   # Compress file.txt to file.txt.gz
    gunzip file.txt.gz  # Decompress file.txt.gz to file.txt

### `df`

Display disk space usage.

    Usage: df [options] [file...]
    Examples:

    bash

    df -h  # Show disk space usage in human-readable form.

### `top`

Display Linux processes.

    Usage: top [options]
    Examples:

    bash

    top  # Display dynamic real-time view of a running system.

### `man`

Interface to the system reference manuals.

    Usage: man [options] keyword
    Examples:

    bash

    man ls  # Display the manual page for the 'ls' command.

### `rm`

Remove files or directories.

    Usage: rm [options] file...
    Examples:

    bash

    rm file.txt  # Remove a file.
    rm -r folder/  # Remove a directory and its contents.

### `whoami`

Print the user name associated with the current effective user ID.

    Usage: whoami
    Examples:

    bash

    whoami  # Display the current user name.

### `pwd`

Print the name of the current working directory.

    Usage: pwd
    Examples:

    bash

    pwd  # Display the current directory path.

### `Viewing File Contents

### `cat, less, more are commands to view the content of files.`

    Examples:

    bash

    cat file.txt  # Display the content of file.txt.
    less file.txt # View the content of file.txt interactively.
    more file.txt # View the content of file.txt page by page.

### `getfacl`

Display file access control lists.

    Usage: getfacl file
    Examples:

    bash

    getfacl file.txt  # Display the access control list of file.txt.

### `wc -l`

Count the number of lines in a file.

    Usage: wc [options] file...
    Examples:

    bash

    wc -l file.txt  # Count the lines in file.txt.

### `diff`

Compare files line by line.

    Usage: diff [options] file1 file2
    Examples:

    bash

    diff old_version.txt new_version.txt  # Compare two versions of a text file.

### `cat <file1> <file2> > <file3>`

Concatenate multiple files and redirect the output to a new file.

    Examples:

    bash

    cat file1.txt file2.txt > combined.txt  # Combine file1.txt and file2.txt into combined.txt.

### `sort`

Sort lines of text files.

    Usage: sort [options] [file...]
    Examples:

    bash

    sort unsorted.txt > sorted.txt  # Sort contents of unsorted.txt and save to sorted.txt.

### `systemctl`

Control the systemd system and service manager.

    Examples:

    bash

    systemctl status nginx  # Check the status of the nginx service.
    systemctl start nginx   # Start the nginx service.
    systemctl stop nginx    # Stop the nginx service.

### `ps, kill`

Manage running processes.

    Examples:

    bash

    ps -ef | grep nginx  # List processes related to nginx.
    kill 1234            # Kill process with PID 1234.
    kill -9 1234         # Forcefully kill process with PID 1234.

### `ping`

Check the reachability of a host on an IP network.

    Usage: ping [options] destination
    Examples:

    bash

    ping google.com  # Ping google.com to check connectivity.

### `wget, curl`

Download files from the internet or interact with web servers.

    Examples:

    bash

    wget http://example.com/file.txt  # Download file.txt from the internet.
    curl -X POST http://example.com/api  # Make a POST request to an API.

### `apt, rpm, dnf`

Package management commands to install, update, and manage packages.

    Examples:

    bash

    sudo apt install nginx  # Install nginx using apt on Debian-based systems.
    rpm -q | grep nginx     # Check if nginx is installed using rpm on RedHat-based systems.
    dnf list installed      # List installed packages using dnf on Fedora.

### `awk, sed, tr`

Text processing commands to manipulate files.

    Examples:

    bash

    awk -F, '{print $2}' file.csv  # Print the second column from a CSV file.
    sed -n '5p' file.txt           # Display the fifth line of file.txt.
    tr [:lower:] [:upper:] < file.txt  # Convert lowercase letters to uppercase in file.txt.


