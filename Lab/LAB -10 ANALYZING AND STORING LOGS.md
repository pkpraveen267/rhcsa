ANALYZING AND STORING LOGS 
PERFORMANCE CHECKLIST 
In this lab, you will change the time zone on an existing server and configure a new log file for all events related to authentication failures. 
OUTCOMES 
You should be able to: 
• Update the time zone on an existing server. 
• Configure a new log file to store all messages related to authentication failures. 
BEFORE YOU BEGIN 
Log in to workstation as student using student as the password. 
On workstation, run lab log-review start to start the exercise. This script records the current time zone of the serverb system and ensures that the environment is setup correctly. 
[student@workstation ~]$ lab log-review start 
1. From workstation, open an SSH session to serverb as student.
2. For the sake of this activity, pretend that the serverb system has been relocated to Jamaica and you must update the time zone appropriately. Use sudo to elevate the privileges of the student user while running the timedatectl command to update the time zone. Use student as the password if asked.
3. Display all the log events recorded in the previous 30 minutes from the current time on serverb.
4. Create the /etc/rsyslog.d/auth-errors.conf file with the necessary lines to help the rsyslog service write messages related to authentication and security issues to the new /var/log/auth-errors file. Use the authpriv facility and the alert priority in the configuration file.
Evaluation 
On workstation, run the lab log-review grade command to confirm success of this exercise. 
[student@workstation ~]$ lab log-review grade 
Finish 
On workstation, run lab log-review finish to complete this lab. This script ensures that the original time zone is restored along with all the original time settings on serverb. 
[student@workstation ~]$ lab log-review finish 
This concludes the guided exercise. 
