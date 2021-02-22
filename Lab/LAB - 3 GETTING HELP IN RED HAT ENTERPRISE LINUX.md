**GETTING HELP IN RED HAT ENTERPRISE LINUX** 

**PERFORMANCE CHECKLIST** 

In this lab, you will look up information to help you complete tasks in man pages and GNU Info documents. 

**OUTCOMES** 

You should be able to:
   
    • Locate relevant commands by searching man pages and Info nodes. 
    • Learn new options for commonly used documentation commands. 
    • Use appropriate tools to view and print documentation and other non-text formatted files. 

**BEFORE YOU BEGIN**

Log in to workstation as student using student as the password. 
On workstation, run the lab help-review start command. 

*[student@workstation ~]$ lab help-review start* 

1. On workstation, determine how to prepare a man page for printing. Specifically, find what format or rendering language is used for printing.

2. Create a formatted output file of the passwd man page. Call the file passwd.ps. Determine the file content format. Inspect the contents of the passwd.ps file.

NOTE :-
Create formatted output of the passwd man page using the following command: 

*[student@workstation $]$ man -t passwd > passwd.ps*

     The > symbol redirects the contents of the man page to the passwd.ps file. 
     This command is taught in more detail in a following chapter.

3. Using man, learn the commands used for viewing and printing PostScript files.

4. Learn how to use the evince(1) viewer in preview mode. Also, determine how to open a document starting on a specific page.

5. View your PostScript file using the various evince options you researched. Close your document file when you are finished.

6. Using the man command, research lp(1) to determine how to print any document starting on a specific page. Without actually entering any commands (because there are no printers), learn the syntax, in one command, to print only pages 2 and 3 of your PostScript file.

7. Using pinfo, look for GNU Info documentation about the evince viewer.

8. Using Firefox, open the system's package documentation directory and browse into the mandb package subdirectory. View the provided manuals.

9. Using the Firefox browser, locate and browse to the initscripts package subdirectory. View the sysconfig.txt file, which describes important system configuration options stored in the /etc/sysconfig directory.

**Evaluation**

On workstation, run lab help-review grade to confirm success of this exercise. 

*[student@workstation ~]$ lab help-review grade* 

**Finish**

On workstation, run the lab help-review finish script to complete this exercise. 

*[student@workstation ~]$ lab help-review finish* 

    This concludes the lab.
