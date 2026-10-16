**Linux File System Heirarchy**

Everything in Linux is either a file or a folder hence as a Linux user one must know the file structure of Linux to navigate and troubleshoot the system.

**Understanding the components of a Command Prompt**

root@ubuntu-dev:/#

- root: The logged in user's username
- ubuntu-dev: The hostname (computer/server)
- : separator
- /: Shows the current working directory (here it is '/' that is the start of the file system, root directory)
- #: The Prompt Symbol, tells two things:
  - That the shell is ready to accept the next command
  - The current privileges that your current session has. (# is superuser, $ is standard user)

**The main directories of the file system**

<img width="563" height="455" alt="image" src="https://github.com/user-attachments/assets/6888ccf9-84e0-4962-906d-2f5c0aba1451" />


1. **sbin**: This directory contains the system binaries.It contains administrative commands.
  - useradd and userdel are the 2 commands that I would use as an administrator to add and delete users.

2. **lib** **-> usr/lib**: This directory is used by the Kernel for making system calls with the hardware, executing commands
  - Not used by the users

3. **boot**: Used by Linux machine to start or restart the machine

4. **bin** -> **usr/bin**: It contains user binaries. Non-administrative commands to be used by standard users.

5. **srv**: Has info about webservers

7. **opt**: While working in an organization, to install any third party dependencies, we install them in /opt directory so that everyone can access the files.

8. **mnt**: Used when more volume/storage has to be added to the filesystem.

9. **media**: For keeping mp3, mp4 files

10. **var**: Used to store the log files or to store third party libraries.

11. **home**: The home directory of the logged in user.

12. **data**: Any data to be shared with other teams members or admin is put in the data directory.

13. **proc****, dev, sys, tmp**: Temporay/volatile directories/folders

14. **root**: Home directory of the root user

16. **run**: Stores the run-time data of a process

17. **etc**: Contains system configuration files. By using these files we can modify the system. Like Settings on a mobile/laptop.
   - shadow: I would use this file to see the encrypted passwords of the users.
   - passwd: I would use this file to check the user info.

**Scenario Based Practice**

**Scenario 1: Service Not Starting**

A web application service called 'myapp' failed to start after a server reboot.
What commands would you run to diagnose the issue?
Write at least 4 commands in order.

Step 1: systemctl status myapp
Why: Firstly I'll check if the service is running or not.

Step 2: systemctl is-enabled myapp
Why: I'll check is the service is enabled or not (to be started on boot/reboot)

Step 3: journalctl -u myapp -n 50 
Why: I'll check what does the log says.

Step 4: systemctl cat myapp
Why: To inspect if the file exists or not.

**Scenario 2: High CPU Usage**

Your manager reports that the application server is slow.
You SSH into the server. What commands would you run to identify
which process is using high CPU?

Step 1: top
Why: To see real-time data on which process has the higest CPU usage.

Step 2: ps aux --sort=%cpu | head -n 5
Why: To get a detail view of the process, which is user is running it and what command is being executed.

Step 3: sudo journalctl _PID=<PID> -n 20
Why: Checking the logs to check whether there is an infinite loop, database lock, etc. 

Step 4: kill -15 <PID>
Why: Gracefully kill process otherwise use kill -9 <PID>

**Scenario 3: Finding Service Logs**

A developer asks: "Where are the logs for the 'docker' service?"
The service is managed by systemd.
What commands would you use?

Step 1: systemctl status <service_name>
Why: To check the service status

Step 2: journalctl -u <service_name> -n 50
Why: Check the last 50 log messages

Step 3: journalctl -u <service_name> -f
Why: Follow log messages in real-time

**Scenario 4: File Permissions Issue**

A script at /home/user/backup.sh is not executing.
When you run it: ./backup.sh
You get: "Permission denied"

Step 1: cd /home/user
Why: Change path to where the file is present

Step 2:ls -l backup.sh
Why: See all the files and folders and what permissions does each file has

Step 3: chmod 764 backup.sh
Why: To give execute permission to the logged in user keeping the group and other users permissions non-executable

Step 4: ./backup.sh
Why: Verify if the script ran successfully
