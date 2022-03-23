# Linux Systems Administration

*Step 1: Ensure/Double Check Permissions on Sensitive Files*

*Permissions on /etc/shadow should allow only root read and write access.*

1. Command to inspect permissions:
- Ls -l /etc/shadow

2. Command to set permissions (if needed):
- Chmod 600 shadow
 
*Permissions on /etc/gshadow should allow only root read and write access.*

3. Command to inspect permissions:
- Ls -l /etc/gshadow

4. Command to set permissions (if needed):
- Chmod 600 gshadow

*Permissions on /etc/group should allow root read and write access, and allow everyone else read access only.*

5. Command to inspect permissions:
- Ls -l /etc/group

6. Command to set permissions (if needed):
- Didn’t need to set permissions for group

*Permissions on /etc/passwd should allow root read and write access, and allow everyone else read access only.*

7. Command to inspect permissions:
- Ls -l /etc/passwd

8. Command to set permissions (if needed):
- Didn’t need to set permissions for passwd

*Step 2: Create User Accounts*

9. Add user accounts for sam, joe, amy, sara, and admin.
Command to add each user account (include all five users):
- Sudo adduser “sam”
- Sudo adduser “joe”
- Sudo adduser “amy”
- Sudo adduser “sara”
- Sudo adduser “admin”

10. Ensure that only the admin has general sudo access. Command to add admin to the sudo group:
- Sudo usermod -aG sudo admin

*Step 3: Create User Group and Collaborative Folder*

11. Add an engineers group to the system. Command to add group:
- Sudo addgroup engineers

12. Add users sam, joe, amy, and sara to the managed group. Command to add users to engineers group (include all four users):
- Sudo usermod -a -G engineers sam
- Sudo usermod -a -G engineers joe
- Sudo usermod -a -G engineers amy
- Sudo usermod -a -G engineers sara

13. Create a shared folder for this group at /home/engineers. Command to create the shared folder:
- Sudo mkdir /home/engineers

14. Change ownership on the new engineers' shared folder to the engineers group. Command to change ownership of engineer's shared folder to engineer group:
- Sudo chgrp engineers /home/engineers/

*Step 4: Lynis Auditing*

Command to install Lynis:

Command to see documentation and instructions:

Command to run an audit:

Provide a report from the Lynis output on what can be done to harden the system.

Screenshot of report output:

![Capture 1](https://user-images.githubusercontent.com/94030092/159806020-9156d2bc-787f-4f35-9d53-45c8d61fdad7.PNG)
