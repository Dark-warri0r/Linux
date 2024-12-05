
### **Networking Basics in Linux**

Networking in Linux involves managing network interfaces, monitoring connections, transferring data, and ensuring seamless communication between systems. This domain is crucial for system administrators, developers, and anyone managing remote servers. Linux provides robust tools for configuring, troubleshooting, and monitoring networks. Below are the key subcategories and commands for networking basics:

---

### **1. Network Connectivity**

Commands in this category test network reachability and check communication between systems.

| **Command** | **Flags**             | **Description**                                      |
|-------------|-----------------------|------------------------------------------------------|
| **ping**    | `-c <count>`          | Sends ICMP packets to check connectivity, where `-c` limits the number of packets. |
|             | `-i <interval>`       | Sets the interval between packets in seconds.       |
|             | `-s <size>`           | Sends packets of a specified size.                 |
| **traceroute** | `<destination>`    | Traces the route packets take to a destination.     |
| **nslookup**| `<hostname>`          | Queries DNS to find IP information for a hostname.  |

---

### **2. Network Interface Configuration**

Commands for managing and configuring network interfaces.

| **Command**   | **Flags**             | **Description**                                      |
|---------------|-----------------------|------------------------------------------------------|
| **ifconfig**  | `<interface>`         | Displays or configures network interfaces (legacy). |
|               | `up/down`             | Activates or deactivates an interface.             |
| **ip**        | `addr`                | Shows or modifies IP addresses.                   |
|               | `link`                | Displays or configures network device properties.  |
|               | `route`               | Displays or modifies routing tables.              |

---

### **3. Network Statistics and Monitoring**

Commands to view and analyze network connections, sockets, and traffic.

| **Command**   | **Flags**             | **Description**                                      |
|---------------|-----------------------|------------------------------------------------------|
| **netstat**   | `-tuln`               | Displays active TCP/UDP ports and listening services.|
|               | `-i`                  | Shows network interface statistics.                 |
| **ss**        | `-tuln`               | Displays active ports and connections (modern alternative to `netstat`). |
|               | `-a`                  | Shows all sockets.                                 |
| **tcpdump**   | `-i <interface>`      | Captures and analyzes network traffic on an interface. |
| **nmap**      | `<IP>`                | Scans for open ports and services on a network.     |

---

### **4. Data Transfer**

Tools for transferring files or data between systems.

| **Command**   | **Flags**             | **Description**                                      |
|---------------|-----------------------|------------------------------------------------------|
| **curl**      | `-O <URL>`            | Downloads a file from a URL.                        |
|               | `-I <URL>`            | Fetches HTTP headers from a URL.                    |
| **wget**      | `<URL>`               | Downloads files non-interactively from a URL.       |
| **scp**       | `<src> <dest>`        | Securely copies files between systems using SSH.    |
| **rsync**     | `-av`                 | Synchronizes files and directories between systems. |

---

### **5. Remote Access**

Commands for securely accessing and managing remote systems.

| **Command**   | **Flags**             | **Description**                                      |
|---------------|-----------------------|------------------------------------------------------|
| **ssh**       | `<user@host>`         | Logs into a remote system securely.                 |
|               | `-p <port>`           | Specifies the remote port to use.                   |
|               | `-i <key>`            | Uses a specific private key for authentication.     |
| **telnet**    | `<host>`              | Connects to a host via Telnet (less secure than SSH).|
| **ftp**       | `<host>`              | Transfers files between systems using FTP protocol. |

---

### **6. DNS and Domain Management**

Commands for managing and troubleshooting DNS-related issues.

| **Command**   | **Flags**             | **Description**                                      |
|---------------|-----------------------|------------------------------------------------------|
| **dig**       | `<domain>`            | Queries DNS servers for information about a domain. |
|               | `+short`              | Outputs concise information about a domain.         |
| **host**      | `<domain>`            | Resolves IP address of a domain.                   |
| **whois**     | `<domain>`            | Retrieves detailed registration information about a domain. |

---

### **7. Firewall and Security**

Commands to manage network security, including configuring firewalls.

| **Command**   | **Flags**             | **Description**                                      |
|---------------|-----------------------|------------------------------------------------------|
| **iptables**  | `-L`                  | Lists firewall rules.                               |
|               | `-A`                  | Appends a rule to a chain.                         |
| **ufw**       | `enable/disable`      | Enables or disables the uncomplicated firewall.    |
|               | `allow <port>`        | Allows traffic on a specific port.                |

---

### **8. Network File Sharing**

Tools for sharing files over the network.

| **Command**   | **Flags**             | **Description**                                      |
|---------------|-----------------------|------------------------------------------------------|
| **nfs**       | `<options>`           | Shares directories using the NFS protocol.         |
| **smbclient** | `<share>`             | Accesses shared files via SMB/CIFS protocol.        |

<br>

---
