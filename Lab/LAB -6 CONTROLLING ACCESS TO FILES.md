# CONTROLLING ACCESS TO FILES #


***PERFORMANCE CHECKLIST*** 

In this lab, you will configure permissions on files and set up a directory that users in a particular group can use to conveniently share files on the local file system. 

**OUTCOMES** 

You should be able to: 

    • Create a directory where users can work collaboratively on files. 
    • Create files that are automatically assigned group ownership. 
    • Create files that are not accessible outside of the group. 

**BEFORE YOU BEGIN**

Log in to workstation as student using student as the password. 

On workstation, run the lab perms-review start command. The command runs a start script that determines if serverb is reachable on the network. The script also creates the techdocs group and three users named tech1, tech2, and database1. 

*[student@workstation ~]$ lab perms-review start*

1. Use the ssh command to log in to serverb as the student user. Switch to root on serverb using redhat as the password.

2. Create a directory called /home/techdocs.

3. Change the group ownership of the /home/techdocs directory to the techdocs group.

4. Verify that users in the techdocs group can create and edit files in the /home/techdocs directory.

5. Set permissions on the /home/techdocs directory. On the /home/techdocs directory, configure setgid (2), read/write/execute permissions (7) for the owner/user and group, and no permissions (0) for other users.

6. Verify that the permissions are set properly.

7. Confirm that users in the techdocs group can now create and edit files in the /home/ techdocs directory. Users not in the techdocs group cannot edit or create files in the /home/techdocs directory. Users tech1 and tech2 are in the techdocs group. User database1 is not in that group.

8. Modify the global login scripts. Normal users should have a umask setting that prevents others from viewing or modifying new files and directories.

9. Log off from serverb.

*[student@serverb ~]$ exit logout Connection to serverb closed.* 

**Evaluation**

On workstation, run the lab perms-review grade script to confirm success on this exercise. 

*[student@workstation ~]$ lab perms-review grade* 

**Finish**

On workstation, run the lab perms-review finish script to complete the lab. 

*[student@workstation ~]$ lab perms-review finish* 

    This concludes the lab. 
