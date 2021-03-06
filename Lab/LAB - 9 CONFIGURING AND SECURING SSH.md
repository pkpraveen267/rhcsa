# CONFIGURING AND SECURING SSH #

***PERFORMANCE CHECKLIST***

In this lab, you will set up key-based authentication for users, and disable direct login as root and password authentication for all users for the 

OpenSSH service on one of your servers. 

**OUTCOMES**

You should be able to: 

    • Authenticate using SSH keys. 
    • Prevent users from directly logging in as root over ssh. 
    • Prevent users from logging in to the system using SSH password-based authentication. 

**BEFORE YOU BEGIN**

Log in to workstation as student using student as the password. 

On workstation, run lab ssh-review start to start the exercise. This script creates the necessary user accounts and files.

*[student@workstation ~]$ lab ssh-review start*

1. From workstation, open an SSH session to servera as student.

2. Use the su command to switch to production1 on servera.

3. Use the ssh-keygen command to generate passphrase-less SSH keys for production1 on servera.

4. Use the ssh-copy-id command to send the public key of the SSH key pair to production1 on serverb.

5. Confirm that production1 can successfully log in to serverb using the SSH keys.

6. Configure sshd on serverb to prevent users logging in as root. Use redhat as the password of the superuser.

7. Configure sshd on serverb to allow users to authenticate using SSH keys only, rather than their passwords.

**Evaluation** 

On workstation, run the lab ssh-review grade command to confirm success of this exercise.

*[student@workstation ~]$ lab ssh-review grade* 

**Finish**

On workstation, run lab ssh-review finish to complete this lab. 


*[student@workstation ~]$ lab ssh-review finish*

    This concludes the lab. 
