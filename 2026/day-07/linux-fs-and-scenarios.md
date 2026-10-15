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
