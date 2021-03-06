# ARCHIVING AND TRANSFERRING FILES #

***PERFORMANCE CHECKLIST***

In this lab, you will use tar, rsync, and scp to archive and back up the contents of directories. 

**OUTCOMES**

You should be able to: 

    • Synchronize a remote directory to a local directory. 
    • Create an archive of the contents of a synchronized directory. 
    • Securely copy an archive to a remote host. 
    • Extract an archive. 

**BEFORE YOU BEGIN** 

Log in as the student user on workstation using student as the password.

From workstation, run the lab archive-review start command. The command runs a start script that determines whether hosts servera and serverb are reachable on the network.

The script also ensures that the files and directories to be created in the lab do not exist on serverb, and workstation. 

*[student@workstation ~]$ lab archive-review start*

1. On serverb, synchronize the /etc directory tree from servera to the /configsync directory.

2. Use gzip compression to create an archive named configfile-backupservera.tar.gz with the contents of the /configsync directory.

3. Securely copy the /root/configfile-backup-servera.tar.gz archive file from serverb to the /home/student directory on workstation as the student user using student as the password.

4. On workstation, extract the contents of the /home/student/configfile-backupservera.tar.gz archive to the /tmp/savedconfig/ directory.

5. On workstation return to the student home directory.

*[student@workstation savedconfig]$ cd*

**Evaluation**

On workstation, run the lab archive-review grade script to confirm success on this lab. 

*[student@workstation ~]$ lab archive-review grade*

**Finish**

On workstation, run the lab archive-review finish script to complete this exercise. 

*[student@workstation ~]$ lab archive-review finish* 

    This concludes the lab. 
