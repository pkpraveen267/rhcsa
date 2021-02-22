MONITORING AND MANAGING LINUX PROCESSES 
PERFORMANCE CHECKLIST 
In this lab, you will locate and manage processes that are using the most resources on a system. 
OUTCOMES 
You should be able to manage processes using top as a process management tool.
 BEFORE YOU BEGIN 
Log in to workstation as student using student as the password. 
On workstation, run the lab processes-review start command. The command runs a start script to determine whether the host, serverb, is reachable on the network. 
[student@workstation ~]$ lab processes-review start 
1. On workstation, open two terminal windows side by side. In this section, these terminals are referred to as left and right. On each terminal window, log in to serverb as the student user.
Create a script called process101, which will generate artificial CPU load. Create the script in the /home/student/bin directory. 
#!/bin/bash 
while true; do 
var=1 
while [[ var -lt 50000 ]]; do var=$(($var+1)) 
done 
sleep 1 
done
2. In the right window, run the top utility.
3. In the left terminal shell, determine the number of logical CPUs on the virtual machine. Run the process101 script in the background.
4. In the right terminal shell, observe the top display. Toggle between load, threads and memory. Note the process ID (PID) for process101. View the CPU percentage. It should hover around 10% to 15%. Ensure that top is showing CPU usage once you have viewed load, threads, and memory.
5. Turn off the use of bold in the display. Save this configuration for reuse when top is restarted. Confirm that the changes are saved.

6. Copy the process101 script to a new file called process102. Edit the script to create more artificial CPU load. Increase the load from fifty thousand to one hundred thousand. Start the process102 process in the background.
7. In the right terminal shell, confirm that the process is running and using the most CPU resources. The load should be hovering between 25% and 35%.
8. The load average is still below 1. Copy process101 to a new script called process103. Increase the addition count to eight hundred thousand. Start process103 in the background. Confirm that the load average is above 1. It may take a few minutes for the load average to change.
9. In the left terminal shell, become root. Suspend the process101 process. List the remaining jobs. Observe that the process state for process101 is now T.
10. Resume the process101 process.
11. Terminate process101, process102, and process103 using the command line. Confirm that the processes no longer display in top.
12. In the left terminal shell, exit from the root user. In the right terminal shell stop the top command. Exit from serverb in both windows.
Evaluation 
On workstation, run the lab processes-review grade script to confirm success on this exercise.
 [student@workstation ~]$ lab processes-review grade 
Finish 
On workstation, run the lab processes-review finish script to complete the lab. 
[student@workstation ~]$ lab processes-review finish 

This concludes the lab.
