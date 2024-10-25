## Overview of Command-Line Interface (CLI)<br>
<div style="text-align: justify;">
&nbsp;&nbsp;&nbsp;&nbsp;The Linux Command Line Interface (CLI) serves as a vital tool for users to interact with their operating system efficiently and effectively. It allows for quick navigation, file manipulation, and system management through a series of text-based commands. The CLI offers greater control and flexibility compared to graphical interfaces, enabling users to automate repetitive tasks, execute scripts, and access advanced system features. 
</div>

#### Key Features of CLI

- **Text-Based Input**: Users enter commands in a terminal, which is efficient for experienced users.

- **Scripting and Automation**: Supports scripts to automate repetitive tasks, boosting productivity.

- **Direct Access to System Functions**: Allows execution of commands that interact directly with the OS, often offering more features than GUIs.

- **Low Resource Usage**: Requires fewer system resources, ideal for low-resource or remote environments.

- **Remote Management**: Commonly used for remote server management, particularly via SSH for secure command execution.
<br><br>

## Basic Structure of Commands

The basic structure of commands in the Linux Command Line Interface (CLI) is as follows:


```bash 
command [options] [arguments]
```

**command**: This is the main instruction you want to execute. For example, ls is a command that lists files in a directory.

[**options]**: These are optional flags that modify the behavior of the command. They usually start with a dash (-). For instance, -l with the ls command gives you more detailed information about each file.

   - **Example: ls -l (lists files in long format)** 

**[arguments]**: These are the targets for the command, such as files or directories that you want to work with. You can specify one or more arguments.

   - **Example: ls -l /home/user (lists files in the /home/user directory in long format)**

<br><br>

# Linux Terminal Shortcuts
<br>



## Open Terminal
| Shortcut               | Action                                      |
|------------------------|---------------------------------------------|
| `Ctrl + Alt + T`      | Open terminal                               |

## Cursor Movement
| Shortcut               | Action                                      |
|------------------------|---------------------------------------------|
| `Ctrl + A`             | Go to the beginning of the line            |
| `Ctrl + E`             | Go to the end of the line                  |
| `Ctrl + XX`            | Move between the beginning and current position of the cursor |
| `Alt + F`              | Move cursor forward one word                |
| `Alt + B`              | Move cursor backward one word               |
| `Ctrl + F`             | Move cursor forward one character           |
| `Ctrl + B`             | Move cursor backward one character          |

## Text Manipulation
| Shortcut               | Action                                      |
|------------------------|---------------------------------------------|
| `Ctrl + U`             | Cut from current position to the beginning  |
| `Ctrl + K`             | Cut from current position to the end        |
| `Ctrl + W`             | Delete the word before the cursor           |
| `Ctrl + Y`             | Paste the last thing from the clipboard     |
| `Alt + T`              | Swap the last two words before the cursor   |
| `Alt + L`              | Make lowercase from cursor to end of word   |
| `Alt + U`              | Make uppercase from cursor to end of word   |
| `Alt + C`              | Capitalize from cursor to end of word       |
| `Alt + D`              | Delete to end of word starting at cursor    |
| `Alt + .`              | Print the last word written in previous command |
| `Ctrl + T`             | Swap the last two characters before the cursor |

## History Access
| Shortcut               | Action                                      |
|------------------------|---------------------------------------------|
| `Ctrl + R`             | Search through previously used commands      |
| `Ctrl + G`             | Leave history searching mode                 |
| `Ctrl + J`             | Copy current matched command to command line |
| `Alt + R`              | Revert changes to a command from history    |
| `Ctrl + P`             | Show last executed command                   |
| `Ctrl + N`             | Show next executed command                   |

## Terminal Control
| Shortcut               | Action                                      |
|------------------------|---------------------------------------------|
| `Ctrl + L`             | Clear the screen                            |
| `Ctrl + S`             | Stop all output to the screen               |
| `Ctrl + Q`             | Resume output to the screen                 |
| `Ctrl + C`             | End currently running process                |
| `Ctrl + D`             | Log out of the current shell session        |
| `Ctrl + Z`             | Suspend currently running foreground process |
| `Tab`                  | Auto-complete files and directory names     |
| `Tab Tab`              | Show all possibilities                       |

## Special Characters
| Shortcut               | Action                                      |
|------------------------|---------------------------------------------|
| `Ctrl + H`             | Same as Backspace                           |
| `Ctrl + J`             | Same as Return (Line Feed)                  |
| `Ctrl + M`             | Same as Return (Carriage Return)            |
| `Ctrl + I`             | Same as Tab                                 |
| `Ctrl + G`             | Bell Character                              |
| `Ctrl + @`             | Null Character                              |
| `Esc`                  | Deadkey equivalent to the Alt modifier      |

## Close Terminal
| Shortcut               | Action                                      |
|------------------------|---------------------------------------------|
| `Ctrl + Shift + W`     | Close terminal tab                          |
| `Ctrl + Shift + Q`     | Close entire terminal                       |




<br>

---






