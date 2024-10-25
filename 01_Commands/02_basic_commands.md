## These are basic commands categorized, with more details included in the following files.

<br>

### Basic Commands

| Command                     | Description                                                                         |
|-----------------------------|-------------------------------------------------------------------------------------|
| `echo "Hello World"`        | Print "Hello World" to the terminal.                                               |
| `hostname`                  | Display the hostname of the system.                                                |
| `clear`                     | Clear the terminal screen.                                                          |
<br>

### Directory Navigation

| Command                     | Description                                                                         |
|-----------------------------|-------------------------------------------------------------------------------------|
| `pwd`                       | Get the full path of the current working directory.                                 |
| `cd -`                      | Navigate to the last directory you were working in.                                 |
| `cd ~` or `cd`             | Navigate to the current user's home directory.                                      |
| `cd ..`                     | Go to the parent directory of the current directory.                                |
| `ls`                        | List files and directories in the current directory.                               |

<br>

### File Management

| Command                     | Description                                                                         |
|-----------------------------|-------------------------------------------------------------------------------------|
| `tree`                      | Generate a tree representation of the file system starting from the current directory. |
| `ls -l`                     | List files and directories in long (table) format for better readability.          |
| `ls -ld dir-name`          | List information about the directory `dir-name` instead of its contents.          |
| `ls -a`                     | List all files, including hidden ones (names starting with a dot).                |
| `cp -p source destination`  | Copy the file from `source` to `destination`, preserving original attributes.      |
| `mv source destination`     | Move or rename a file or directory.                                               |
| `rm filename`               | Remove a file.                                                                      |
| `rmdir dirname`             | Remove an empty directory.                                                          |
| `mkdir dirname`             | Create a new directory named `dirname`.                                            |
| `touch filename`            | Create an empty file or update the timestamp of an existing file.                  |

<br>

### Process Management

| Command                     | Description                                                                         |
|-----------------------------|-------------------------------------------------------------------------------------|
| `ps`                        | Display currently running processes.                                               |
| `top`                       | Display dynamic real-time information about running processes.                     |
| `kill PID`                 | Terminate a process by its Process ID (PID).                                     |
| `bg`                        | Resume a suspended job in the background.                                          |
| `fg`                        | Bring a background job to the foreground.                                         |

<br>

### Help and Documentation

| Command                     | Description                                                                         |
|-----------------------------|-------------------------------------------------------------------------------------|
| `man <name>`                | Read the manual page of `<name>`.                                                 |
| `info <name>`               | Display more detailed information about `<name>`, if available.                   |
| `--help`                    | Display help information for a command (e.g., `ls --help`).                       |

<br>

### System Information

| Command                     | Description                                                                         |
|-----------------------------|-------------------------------------------------------------------------------------|
| `df`                        | Display disk space usage.                                                          |
| `du`                        | Estimate file and directory space usage.                                           |
| `free`                      | Show memory usage.                                                                  |
| `uptime`                   | Display how long the system has been running.                                      |
| `who`                       | Show who is logged in.                                                             |

<br>

---