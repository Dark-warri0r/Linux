### **Process Management in Linux**


Process management in Linux involves controlling, monitoring, and handling processes (programs in execution). A process in Linux can be anything from a simple command to a complex program running in the background. Process management ensures that processes are allocated resources, such as CPU time, memory, and input/output devices. It also provides mechanisms for controlling processes (e.g., terminating, suspending) and monitoring their resource usage.


Here’s an overview of the main subcategories in **Process Management**:

<br>


## **1. Process Listing**

- **`top` Command**: Provides a dynamic, real-time process viewer. 

- **`htop` Command**: Advanced, interactive process manager with user-friendly visuals.  

- **`pgrep` Command**: Searches for process IDs by name.  

- **`pidof` Command**: Retrieves the PID of a specific program.  

---

<br>

| **Command** | **Flags**        | **Description**                                 |
|-------------|------------------|-------------------------------------------------|
| **ps**      | `aux`            | Displays all processes with detailed info.      |
|             | `-ef`            | Full-format listing of processes.               |
| **top**     | (No flags)       | Real-time interactive process viewer.           |
| **htop**    | (No flags)       | Enhanced version of `top`.                      |
| **pgrep**   | `<name>`         | Searches for processes by name.                 |
| **pidof**   | `<program>`      | Finds the PID of a running program.             |

<br><br>

## **2. Process Control**

- **`kill` Command**: Sends signals to processes to terminate or control them.  

- **`pkill` Command**: Terminates processes by matching names.  

- **`killall` Command**: Stops all processes with a specified name. 

- **`bg` Command**: Resumes suspended jobs in the background.  

- **`fg` Command**: Brings a background job to the foreground.  

- **`jobs` Command**: Lists running and suspended jobs.  

---

<br>

| **Command** | **Flags**              | **Description**                                 |
|-------------|------------------------|-------------------------------------------------|
| **kill**    | `-9 <PID>`             | Forcefully terminates a process by PID.         |
| **pkill**   | `<name>`               | Kills processes matching the given name.        |
| **killall** | `<name>`               | Terminates all processes with a specific name.  |
| **bg**      | (No flags)             | Resumes a suspended process in the background.  |
| **fg**      | (No flags)             | Brings a background process to the foreground.  |
| **jobs**    | (No flags)             | Lists all running or suspended jobs.            |

<br><br>

## **3. Process Monitoring**

- **`top` Command**: Displays resource usage and system performance in real time.  

- **`htop` Command**: Offers an interactive, graphical view of running processes.  

- **`vmstat` Command**: Reports CPU, memory, and I/O statistics over intervals.  

- **`iostat` Command**: Monitors CPU and device input/output statistics.  

- **`mpstat` Command**: Provides CPU usage metrics for multi-processor systems.  

- **`sar` Command**: Collects and reports comprehensive system activity.  

- **`pidstat` Command**: Displays process-specific resource usage statistics.  

---
<br>


| **Command** | **Flags**               | **Description**                                 |
|-------------|-------------------------|-------------------------------------------------|
| **top**     | (No flags)              | Displays real-time resource usage.             |
| **htop**    | (No flags)              | Interactive system monitoring tool.            |
| **vmstat**  | `<interval>`            | Reports CPU, memory, and I/O stats.            |
| **iostat**  | `-x`                    | Shows CPU and device I/O performance.          |
| **mpstat**  | `<interval>`            | Reports CPU usage statistics.                  |
| **sar**     | `-u`, `-r`, `-n DEV`    | Collects system activity for CPU, memory, etc. |
| **pidstat** | `-u`, `-r`              | Displays per-process CPU and memory usage.     |

<br><br>

## **4. Advanced Management**

- **`nice` Command**: Adjusts the priority of a process during execution. 

- **`renice` Command**: Modifies the priority of a running process.  

- **`nohup` Command**: Executes a command immune to hangups or logouts. 

- **`disown` Command**: Detaches a process from the shell session.  

---

<br>

| **Command** | **Flags**       | **Description**                                 |
|-------------|-----------------|-------------------------------------------------|
| **nice**    | `-n <value>`    | Runs a command with the specified priority.     |
| **renice**  | `<value> <PID>` | Changes the priority of a running process.      |
| **nohup**   | (No flags)      | Runs a command immune to hangups.               |
| **disown**  | (No flags)      | Detaches a running process from the shell.      |

<br><br>

## **5. Session Management**

- **`screen` Command**: Manages multiple terminal sessions simultaneously. 

- **`tmux` Command**: A powerful terminal multiplexer with enhanced features.  

- **`setsid` Command**: Runs a command in a new session, detaching it from the terminal.  

---
<br>


| **Command** | **Flags**       | **Description**                                 |
|-------------|-----------------|-------------------------------------------------|
| **screen**  | (No flags)      | Manages multiple terminal sessions.            |
| **tmux**    | (No flags)      | An advanced terminal multiplexer.              |
| **setsid**  | (No flags)      | Starts a command in a new session.             |


---