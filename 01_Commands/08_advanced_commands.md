# Advanced Commands

 Understanding how to effectively chain commands, use redirection and pipes, and work with environment variables is crucial for efficiently working in the shell. These concepts allow users to combine multiple commands, manage data flows between commands, and configure system environments to suit specific tasks.

- **Command Chaining** enables you to run multiple commands in a sequence, with control over the execution flow based on the success or failure of the previous commands.
   
- **Redirection and Pipes** help you manipulate input and output by redirecting data to and from files, and passing data between commands in a pipeline.
   
- **Environment Variables** define settings and configurations for the system and applications, enabling flexibility and customization for various tasks and scripts.

<br>



## **Command Chaining: Use of `&&`, `||`, and `;` to Chain Commands**

#### **1. Command Chaining**

Command chaining allows you to execute multiple commands in a single line. Depending on the success or failure of previous commands, subsequent commands can be executed using operators like `&&`, `||`, and `;`.

| **Operator**   | **Description**                                                | **Example**                                             |
|----------------|----------------------------------------------------------------|---------------------------------------------------------|
| `&&`           | Executes the second command only if the first command succeeds. | `mkdir newdir && cd newdir`                             |
| `||`           | Executes the second command only if the first command fails.   | `ls non_existing_dir '||' echo "Directory not found"`    |
| `;`            | Executes the commands sequentially, regardless of success or failure. | `echo "Hello" ; ls`                                   |

#### **Use Case Examples:**
1. **`&&` Example**: `mkdir testdir && cd testdir`  
   Creates a directory (`mkdir`) and only navigates into it (`cd`) if the directory creation is successful.
   
2. **`||` Example**: `ping google.com || echo "Network not reachable"`  
   Attempts to ping Google's server and echoes a message if the ping fails.

3. **` ; ` Example**: `echo "First Command"; echo "Second Command"`  
   Runs both commands one after the other, without checking the success of the first.

---

### **Redirection and Pipes: Use of `>`, `<`, and `|` to Redirect Input/Output**

#### **2. Redirection and Pipes**

Redirection allows you to control where the output of a command goes (to a file, for example), and pipes allow you to send the output of one command as the input to another.

| **Operator**   | **Description**                                                 | **Example**                                                 |
|----------------|-----------------------------------------------------------------|-------------------------------------------------------------|
| `>`            | Redirects standard output to a file, overwriting the file.       | `echo "Hello World" > hello.txt`                            |
| `>>`           | Appends standard output to the end of a file.                   | `echo "Append this line" >> hello.txt`                      |
| `<`            | Redirects input from a file to a command.                       | `sort < unsorted.txt`                                       |
| `2>`           | Redirects standard error to a file.                             | `ls non_existing_file 2> error.log`                         |
| `&>`           | Redirects both standard output and error to the same file.      | `ls / > output.log 2>&1`                                    |
| `|`            | Sends the output of one command as input to another.            | `ls | grep "file"`                                          |

#### **Use Case Examples:**
1. **`>` Example**: `echo "Hello" > file.txt`  
   This command writes the text "Hello" to `file.txt`, overwriting any previous content.
   
2. **`>>` Example**: `echo "New entry" >> file.txt`  
   Appends the text "New entry" to `file.txt` without overwriting existing content.

3. **`|` Example**: `ps aux | grep apache`  
   This pipes the output of `ps aux` (process list) to `grep` to filter and show only processes related to "apache".

4. **`2>` Example**: `cat non_existent_file 2> error.log`  
   Redirects the error output of the `cat` command to `error.log` when the file doesn't exist.

---

### **Environment Variables: Overview and How to Set Them**

#### **3. Environment Variables**

Environment variables are used to store system-wide values that processes and commands can reference. These variables store information about the system environment, such as paths, user details, or configurations.

| **Command**            | **Description**                                                  | **Example**                                                  |
|------------------------|------------------------------------------------------------------|--------------------------------------------------------------|
| `echo $VARIABLE`       | Displays the value of an environment variable.                   | `echo $HOME`                                                 |
| `export VARIABLE=value`| Sets a new environment variable or updates an existing one.      | `export PATH=$PATH:/new/path`                                |
| `unset VARIABLE`       | Removes an environment variable.                                | `unset MY_VARIABLE`                                          |
| `env`                  | Lists all environment variables.                                | `env`                                                        |
| `printenv`             | Displays the value of a specific environment variable.           | `printenv HOME`                                              |

#### **Use Case Examples:**
1. **Setting an Environment Variable**: `export MY_VAR="value"`  
   This sets a new variable `MY_VAR` with the value "value". It's available for the current session.

2. **Viewing Environment Variables**: `echo $PATH`  
   This command displays the current `PATH` environment variable, which holds directories that the shell searches for executables.

3. **Unsetting a Variable**: `unset MY_VAR`  
   This removes the `MY_VAR` variable from the environment.

4. **Viewing All Environment Variables**: `env`  
   Lists all the environment variables currently available in the system.

---

