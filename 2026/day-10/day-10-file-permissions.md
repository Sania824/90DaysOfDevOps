# Day 10 - File Permission Challenge

## Files Created

1. `devops.txt` through touch command
2. `notes.txt` through echo command
3. `scripts.txt` through vim

<img width="493" height="408" alt="image" src="https://github.com/user-attachments/assets/86d01227-a64b-415d-9aa8-345a06c81252" />

## Permission Changes

<img width="582" height="114" alt="image" src="https://github.com/user-attachments/assets/ac49ebb2-d9b9-4ee7-9830-110fd467dc90" />

### Before

- For all the 3 files:
  - owner has only read, write permission,
  - groups have only reach and write permission
  - others have only read permission

### After

- Modified the execute permission for scripts.sh and successfully ran the script

<img width="582" height="210" alt="image" src="https://github.com/user-attachments/assets/8940cdae-06c3-4e91-b998-9b5afe851363" />

- Modified permissions on devops.txt and made it read-only

<img width="441" height="93" alt="image" src="https://github.com/user-attachments/assets/42d93046-60e3-419d-985d-6b195e271506" />

- Modified permissions for notes.txt and set permissions to 640 (6=rw for owner, 4=r for groups, 0=no permissions for other users)

<img width="441" height="93" alt="image" src="https://github.com/user-attachments/assets/84049c96-dae9-4383-894b-b73175654ae2" />

## Commands Used

1. `touch devops.txt`
2. `echo "Hello" > notes.txt`
3. `vim scripts.sh`
4. `ls -l`
5. `cat notes.txt`
6. `head -5 /etc/passwd`
7. `tail -5 /etc/passwd`
8. `chmod 764 scripts.sh`
9. `./scripts.sh`
10. `chmod 444 devops.txt`
11. `chmod 640 notes.txt`
12. `mkdir projects`
13. `chmod 755 projects`
14. `ls -l devops.txt notes.txt scripts.txt`

## Testing Permissions

<img width="638" height="356" alt="image" src="https://github.com/user-attachments/assets/55486457-413c-4136-8e28-c0d7f8ad10d0" />

## What I learned

1. This exercise pushed me to understand and execute Linux permissions with more clarity and confidence.
2. I leanred modifying permissions
3. Understanding the error messages and taking proper actions
4. Understood that space in Linux commands is crucial
