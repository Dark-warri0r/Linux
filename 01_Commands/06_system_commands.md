


## **System Information**

System Information commands help gather details about the operating system, disk usage, and uptime. These are useful for monitoring and managing system health.

| **Command**       | **Flags**        | **Description**                                              |
|-------------------|------------------|--------------------------------------------------------------|
| `uname`           | `-a`            | Shows all available system information.                     |
|                   | `-r`            | Displays the kernel release version.                        |
|                   | `-s`            | Prints the kernel name.                                      |
|                   | `-m`            | Displays the machine hardware name.                         |
| `df`              | `-h`            | Displays disk space usage in a human-readable format.        |
|                   | `-T`            | Displays filesystem type alongside disk usage.              |
|                   | `-a`            | Includes pseudo and unmounted filesystems.                  |
| `du`              | `-h`            | Provides human-readable file or directory sizes.            |
|                   | `-s`            | Displays only the total size for directories.               |
|                   | `-a`            | Lists sizes for all files and directories recursively.       |
| `uptime`          | N/A             | Displays the time since the last reboot and load averages.  |
| `history`         | `-c`            | Clears the command history for the session.                 |
|                   | `<N>`           | Shows the last `N` commands from history.                   |

---

## **System Management**

System Management commands are essential for controlling the system’s power states, such as shutdowns, reboots, and halts.

| **Command**       | **Flags**        | **Description**                                              |
|-------------------|------------------|--------------------------------------------------------------|
| `shutdown`        | `-h`            | Halts the system after shutting down services.              |
|                   | `-r`            | Reboots the system after shutdown.                          |
|                   | `-t`            | Schedules shutdown or reboot after a specified delay.       |
| `reboot`          | N/A             | Reboots the system immediately.                             |
| `halt`            | N/A             | Stops all system processes without powering off the machine.|
| `poweroff`        | N/A             | Shuts down the system and powers it off.                    |

---

## **Detecting Linux Distribution**

These commands are used to identify the Linux distribution and its version details, which is crucial for troubleshooting or software compatibility.

| **Command**            | **Flags**        | **Description**                                              |
|------------------------|------------------|--------------------------------------------------------------|
| `lsb_release`          | `-a`            | Displays all available information about the distribution.  |
|                        | `-d`            | Displays the distribution description.                      |
|                        | `-r`            | Shows the release number.                                   |
| `cat /etc/os-release`  | N/A             | Outputs operating system details such as name and version.  |
| `hostnamectl`          | N/A             | Displays system hostname and basic OS information.          |

---

## **Basic Linux Utilities**

Basic Linux utilities include essential commands for day-to-day system usage, such as checking the date, clearing the terminal, or identifying the current user.

| **Command**       | **Flags**        | **Description**                                              |
|-------------------|------------------|--------------------------------------------------------------|
| `date`            | `+<format>`      | Formats the date output (e.g., `+%Y-%m-%d` for YYYY-MM-DD). |
|                   | `-s`            | Sets the system date and time.                              |
| `clear`           | N/A             | Clears the terminal screen for better readability.          |
| `whoami`          | N/A             | Displays the username of the current user.                  |

---
