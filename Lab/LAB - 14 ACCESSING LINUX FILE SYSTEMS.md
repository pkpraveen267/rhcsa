ACCESSING LINUX FILE SYSTEMS 
PERFORMANCE CHECKLIST 
In this lab, you will mount a local file system and locate specific files on that file system. 
OUTCOMES 
You should be able to:
 • Mount a file system. 
• Generate a disk usage report. 
• Search files in the local file system. 
BEFORE YOU BEGIN 
Log in as the student user on workstation using student as the password. 
From workstation, run the lab fs-review start command. The command runs a start script that determines if the host, serverb, is reachable on the network. The script also creates a partition on the second disk attached to serverb. 
[student@workstation ~]$ lab fs-review start 
1. On serverb as root, identify the UUID for /dev/vdb1 and mount /dev/vdb1 by its UUID on the /mnt/freespace directory.
2. Generate a disk usage report of the /usr/share directory, and save the result in the /mnt/ freespace/results.txt file.
3. Use the locate command to find all rsyslog.conf configuration files and store the result in the /mnt/freespace/search1.txt file.
4. Store the search result of all files in the /usr/share directory that is greater than 50 MB and less than 100 MB in the /mnt/freespace/search2.txt file.
5. Exit from serverb.
Evaluation 
On workstation, run the lab fs-review grade script to confirm success on this lab.
[student@workstation ~]$ lab fs-review grade
 Finish 
On workstation, run the lab fs-review finish script to complete this exercise. 
[student@workstation ~]$ lab fs-review finish 
This concludes the lab. 
