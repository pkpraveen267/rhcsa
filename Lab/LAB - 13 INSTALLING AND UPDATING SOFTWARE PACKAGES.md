# INSTALLING AND UPDATING SOFTWARE PACKAGES #

***PERFORMANCE CHECKLIST***

 In this lab, you will manage software repositories and module streams, and install and upgrade packages from those repositories and streams. 

**OUTCOMES**

You should be able to: 

    • Manage software repositories and module streams.
    • Install and upgrade packages from repositories and streams.
    • Install an RPM package. 

**BEFORE YOU BEGIN**


Log in to workstation as student using student as the password. 

On workstation, run the lab software-review start command. This script ensures that serverb is available. It also downloads any packages required for the lab exercise. 

*[student@workstation ~]$ lab software-review start* 

1. On serverb configure a software repository to obtain updates. The repository should be called /etc/yum.repos.d/errata.repo. It should access http:// content.example.com/rhel8.0/x86_64/rhcsa-practice/errata. Do not check GPG signatures.

2. On serverb, install new package xsane-gimp and the Apache HTTP Server module from the 2.4 stream and the common profile.

3. For security reasons, serverb should not be able to send anything to print. Achieve this by removing the cups package. Exit from the root account.

4. Confirm that the package rhcsa-script-1.0.0-1.noarch.rpm is available on serverb. Install the package. You will need to gain superuser privileges to install the package. Verify that the package is installed. Exit from serverb.

**Evaluation**

On workstation, run the lab software-review grade script to confirm success on this lab.

*[student@workstation ~]$ lab software-review grade* 

**Finish**

On workstation, run the lab software-review finish script to complete this exercise. This script removes the repository and packages created during this exercise.

*[student@workstation ~]$ lab software-review finish* 

    This concludes the lab. 
