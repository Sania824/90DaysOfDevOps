<img width="1302" height="674" alt="image" src="https://github.com/user-attachments/assets/1ef2dbf6-054f-46e9-94a3-fda14e108be9" />The following task focuses on making a troubleshooting runbook to get equipped with Linux adminstration. 

Below is the process that I followed, their respective steps and commands.

**Step 1: Chose a service to explore**

Command Used: systemctl list-units --type=service
<img width="1294" height="682" alt="image" src="https://github.com/user-attachments/assets/bd342db0-d79d-4938-abea-889f5da1ab04" />

**Step 2: I found the PID of the service that I chose: cron.service**

Command Used: systemctl status cron.service
<img width="1092" height="449" alt="image" src="https://github.com/user-attachments/assets/47a3f45a-0fb2-4b3c-91ac-0071c1adf33b" />

**Environment Basics**

Checking the environemt basics like the machine details we're working on and kernel version we're debugging.

<img width="995" height="366" alt="image" src="https://github.com/user-attachments/assets/ad79e1be-3a6e-44b2-9910-d95be5fd4a1f" />

**Filesystem Sanity**

Created a throwaway directory
<img width="1139" height="438" alt="image" src="https://github.com/user-attachments/assets/bed34f7c-6d82-4626-b64e-679084cf41ed" />

Copied a text file
<img width="734" height="656" alt="image" src="https://github.com/user-attachments/assets/0193d96e-a96a-43ae-a19e-6c8c004fb259" />

**CPU, Memory Utilization**

I checked the memory utilization across the system and then checked cpu utilization for the cron.service that I am inspecting

**Lesson Learned**
While typing the ps command with commas in it, my command was not getting executed but I cam to learn that ps command is highly strict about spacing between the columns. Hence, when using commas it is imp to not leave space after.

<img width="692" height="416" alt="image" src="https://github.com/user-attachments/assets/40bec9a0-458b-43eb-9b35-ddc73ce729da" />

**Disk Management**

<img width="952" height="471" alt="image" src="https://github.com/user-attachments/assets/8c8fe367-710f-4c8c-b64b-c573b7f6b0aa" />

**Networking Connectivity**

<img width="1302" height="462" alt="image" src="https://github.com/user-attachments/assets/69b95c22-373e-4363-ab07-06415e8f2569" />

**Log Inspection**

Service Specific Logs: 

<img width="1302" height="674" alt="image" src="https://github.com/user-attachments/assets/f397cbe6-0efd-4f47-a7ff-ac56de673c21" />

Standard system log file check:


<img width="1302" height="674" alt="image" src="https://github.com/user-attachments/assets/04e3c7c9-217c-4c9f-b2a9-abbff9a66e63" />






