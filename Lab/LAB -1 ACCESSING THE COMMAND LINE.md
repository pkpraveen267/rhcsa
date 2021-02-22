# ACCESSING THE COMMAND LINE #

**PERFORMANCE CHECKLIST**

In this lab, you will use the Bash shell to execute commands. 

**OUTCOMES**

    • Successfully run simple programs using the Bash shell command line. 
    • Execute commands used to identify file types and display parts of text files. s
    • Practice using some Bash command history "shortcuts" to more efficiently repeat commands or parts of commands.
    
 **BEFORE YOU BEGIN**
 
    Log in to workstation as student using student as the password. 
    On workstation, run the lab cli-review start script to set up a clean lab environment. 
    The script also copies the zcat file to student's home directory. 
1. Use the date command to display the current time and date.
2. Display the current time in 12-hour clock time (for example, 11:42:11 AM). Hint: The format string that displays that output is %r.
3. What kind of file is /home/student/zcat? Is it readable by humans?
4. Use the wc command and Bash shortcuts to display the size of zcat.
5. Display the first 10 lines of zcat.
6. Display the last 10 lines of the zcat file.
7. Repeat the previous command exactly with three or fewer keystrokes.
8. Repeat the previous command, but use the -n 20 option to display the last 20 lines in the file.
   Use command-line editing to accomplish this with a minimal number of keystrokes.
9. Use the shell history to run the date +%r command again.
   
 **Evaluation**
   
     On workstation, run the lab cli-review grade script to confirm success on this exercise.
 
 *[student@workstation ~]$ lab cli-review grade*
 
 **Finish**
 
   On workstation, run the lab cli-review finish script to complete the lab.
 
 *[student@workstation ~]$ lab cli-review finish* 
      
      This concludes the lab.
