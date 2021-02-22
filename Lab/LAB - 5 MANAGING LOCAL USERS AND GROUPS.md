MANAGING LOCAL USERS AND GROUPS 
PERFORMANCE CHECKLIST 
In this lab you will set a default local password policy, create a supplementary group for three users, allow that group to use sudo to run commands as root, and modify the password policy for one user. 
OUTCOMES 
You should be able to: 
• Set a default password aging policy of the local user's password. 
• Create a group and use the group as a supplementary group for new users. 
• Create three new users with the new group as their supplementary group. 
• Configure the group members of the supplementary group to run any command as any user using sudo. 
• Set a user-specific password aging policy. 
BEFORE YOU BEGIN 
Log in to workstation as student using student as the password. 
On workstation, run lab users-review start to start the exercise. This script creates the necessary files to ensure that the environment is set up correctly. 
[student@workstation ~]$ lab users-review start 
1. From workstation, open an SSH session to serverb as student.
2. On serverb, ensure that newly created users have passwords that must be changed every 30 days.
3. Create the new group consultants with a GID of 40000.
4. Configure administrative rights for all members of consultants to be able to execute any command as any user.
5. Create the consultant1, consultant2, and consultant3 users with consultants as their supplementary group.
6. Set the consultant1, consultant2, and consultant3 accounts to expire in 90 days from the current day.
7. Change the password policy for the consultant2 account to require a new password every 15days.
8. Additionally, force the consultant1, consultant2, and consultant3 users to change their passwords on the first login. 
Evaluation 
On workstation, run the lab users-review grade command to confirm success of this exercise. 
[student@workstation ~]$ lab users-review grade 
Finish 
On workstation, run lab users-review finish to complete this lab. 
This script deletes the user accounts and files created throughout the lab to ensure that the environment is clean. 
[student@workstation ~]$ lab users-review finish 
This concludes the lab.
