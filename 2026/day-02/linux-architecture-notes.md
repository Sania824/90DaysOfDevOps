**Today's Learning Points**
**Linux Fundamentals**
  - Linus Trovalds created linux in 1991, kept it free and opensource.
  - Linux serves as the go to OS for about 90% of the applications in production.
  - It is highly secure and supports multi-users.
 
**How Linux Works**
  - Learned the Onion model on which Linux works.
  - Gained in depth knowledge of the three layers of the model that are Application, Shell, Kernel
  - Kernel has the code necessary to carry out the instructions. Linux code was orginally written in C language but each time command had to be executed and the intructions were passed on from the Shell to Kernel, the code had to compiled to binaries so that the hardware can actually execute the instructions. Hence, the Kernel contains already executed Machine code that can easily be executed without compiling. We can find these binaries in the root directory of the system.
  - Applications are the utilities like VS Code IDE, Docker, Kubernetes, etc.
  - Applications tell the shell to execute commands and shell communicates with the kernel to execute out the binaries associated with the shell commands.

**Process States**
  - There are five process states primarily that includes:
  - New -> Ready -> Running -> Waiting -> Terminated
  - A program is a dormant software sitting on your hard drive that when to be ran becomes a process.
  - When a process starts it first gets initialized with the New State, then gets ilined up in queue to be given the CPU for processing and gets in the Ready State. Once the CPU has been assigned the process gets in Running State and if in between the execution there is a need for I/O from any device then the process lands in the Waiting State, waiting for the necessary information to be given so that it can get back to the Ready state from where when the CPU assigned the process gets back in the Running state. There could be an Interrupt as well if the execution times out. Once the process is completed the process finally reaches the Terminated State.

**How the Computer Starts and What is systemd**
  - I also understood the behind the scenes of how the computer works.
  - Once we turn our system On, it first starts the BIOS (a firmware -> connect hardware and software) that starts the Bootloader.
  - The bootloader knows where the kernel code lives. The Kernel then starts a process and the first process to be started is init/systemd it has the Process ID 1, since it is the first process to be ran. Systemd then further starts more processes that starts the utilities.

**5 Commands for daily use**
  - pwd -> to check the present working directory
  - cd -> to change the directory 
  - cd .. -> to get back to tilde (~)
  - mkdir -> to make a new directory
  - touch -> to create a single empty file
