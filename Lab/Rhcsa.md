**CONTROLLING SERVICES AND DAEMONS**

**PERFORMANCE CHECKLIST**

    In this lab, you will configure several services to be enabled or disabled, running or stopped, based on a specification that is provided to you. 
**OUTCOMES**

    You should be able to enable, disable, start, and stop services. 
**BEFORE YOU BEGIN**

     Log in as the student user on workstation using student as the password. 
     From workstation, run the lab services-review start command. 
     The command runs a start script that determines whether the host, serverb, is reachable on the network. 
     The script also ensures that the psacct and rsyslog services are configured appropriately on serverb. 
**[student@workstation ~]$ lab services-review start**

1. On serverb, start the psacct service.
2. Configure the psacct service to start at system boot.
3. Stop the rsyslog service.
4. Configure the rsyslog service so that it does not start at system boot.
5. Reboot serverb before evaluating the lab.

**Evaluation**

     On workstation, run the lab services-review grade script to confirm success on this lab.
     
 **[student@workstation ~]$ lab services-review grade**
 
**Finish**

       On workstation, run the lab services-review finish script to complete this lab.
 **[student@workstation ~]$ lab services-review finish** 

   This concludes the lab. 
