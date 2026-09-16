For today's task, I'll be making my own Linux commands cheatsheet that will be focused on: Process Management, File System and Networking commands.

**Process Management**

Process management commands in Linux are used monitor, control and manage running processes on the system. These are crucial to troublesheet system behaviour effectively.

Following are some management commands:

1. accton: This is an administrative level command used for process accounting/auditing
2. bg: It is used to resume a stopped job in the background
3. chrt: chrt is used to set or view real-time scheduling priority of a process
4. fg: Brings a background job to foreground
5. kill: This command is essential for process control and is used to send signal to the process. It terminates a unresponsive process
6. mpstat: Used to monitor system performance. This shows the CPU usage statistics for **processors**.
7. pidof: Used for getting the process ID of a running program (process)
8. pmap: Shows memory usage of a process. Useful for monitoring memory consumption
9. ps aux: Lists all active processes. Comes with different [options] to use for process monitoring
10. top: This shows live process activity, real-time view of running processes. It shows CPU and monitoring usage dynamically.
11. htop: Upgraded version of 'top' command with a more user-friendly interactive interface
12. strace: Traces system calls made by process, used for debugging applications
13. time: Shows time taken by a command to get executed. Displays execution time and resource usage
14. watch: The watch command runs a commands repeatedly on fixed intervals. Used for monitoring and live updates
15. vmstat: It gives an overview of system performance, displays memory, CPU and I/O statistics
16. uptime: This command shows fpr how long the system has been running. It also shows system load-average
17. w: Display information about logged-in users and their running processes. Combines user and process details

**File Management**

Everything in Linux is treated as a file. File Management in Linux includes handling files and directories through various commands such as remove, move, creation, modification and access control within the file system.
There are General files, Directory files (Folders) and Device Files. 

Following are some of the commonly used File Management Commands
1. ls: List all files in the current directory
2. pwd: Displays the present working directory
3. cd: Changes directory
4. touch: Creates a new file. If the file does not exists then an empty new file is created otherwise the already existing file's content remains same but the timestamp gets updated.
5. cat: Displays the content inside the file
6. cp: Used to copy a file and paste it in the given destination
7. mv: Moves a file from one location to another in Linux. mv can also be used to **rename** and file in destination (mv filename new_filename)
8. rm: Used to remove/delete a file in Linux file system

**Network Management**

1. ping: sends ICMP ECHO_REQUEST to host
2. ip: shows/manipulates routing, network devices, interfaces and tunnels
3. netstat: Stands for networking statistics. Shows various network related information such as listening ports, active connections, routing tables, and interface statistics. 
