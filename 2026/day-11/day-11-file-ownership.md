# Day 10 Challenges

## **Task 1**

### **Understanding Ownership**

- Owner: An owner is a specific account that is the sole master of the file or a directory, typically the one who created it (but ownership does not always lies with the logged in user but can be transferred.)

- Group: A group is a collection of user accounts that share specific permissions for a file or a directory.

## **Task 2**

### **Changing Ownershop**

- Created a file that was owned by a sania user and changed the ownership to a user 'tokyo'

<img width="484" height="679" alt="image" src="https://github.com/user-attachments/assets/5af76b42-67d5-4f02-bfe9-733508ac5af2" />

### **Commands Used**

1. sudo chown tokyo devops.txt

## **Task 3**

### **Basic chgrp Operations**

- Made a new group 'heist-team'
- Changed a file group

<img width="539" height="181" alt="image" src="https://github.com/user-attachments/assets/1135dbad-b6a9-4323-b384-74a57e59f77f" />

### **Commands Used**

1. ls -l notes.txt
2. sudo groupadd heist-team
3. sudo chgrp heist-team notes.txt
4. ls -l notes.txt

## **Task 4**

- Changing both ownership and group together with chown

<img width="688" height="444" alt="image" src="https://github.com/user-attachments/assets/68e997c7-1109-4914-adf0-a5af91080e0f" />

**For directory**

<img width="670" height="690" alt="image" src="https://github.com/user-attachments/assets/2172f0b2-792c-4968-b7cf-65c606a28eea" />


### **Commands Used:**

1. touch project-config.yaml
2. ls -l
3. sudo chown professor:heist-team project-config.yaml
4. ls -l project-Config.yaml

## **Task 5**

### **Recursive Ownership**

- Created a nested folder structure and then recursively changed the ownership and the group of the folder, subfolders and files.

<img width="635" height="552" alt="image" src="https://github.com/user-attachments/assets/267beb39-5795-471f-84f2-d4197add7cd8" />

<img width="635" height="150" alt="image" src="https://github.com/user-attachments/assets/870eef81-d96f-4ece-a878-a7498483b7a3" />

<img width="680" height="621" alt="image" src="https://github.com/user-attachments/assets/3c76fad1-76cd-4438-94f2-de0a9e4b3789" />

### **Commands Used**

1. mkdir -p heist-project/vault
2. mkdir -p heist-project/plans
3. touch heist-project/vault/gold.txt
4. touch heist-project/plans/strategy.conf
5. ls -l
6. ls -l heist-project
7. ls -l heist-project/vault
8. ls -l heist-project/plans
9. sudo chown -R professor:planners heist-project


