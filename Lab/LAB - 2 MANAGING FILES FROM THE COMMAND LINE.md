# MANAGING FILES FROM THE COMMAND LINE #

***PERFORMANCE CHECKLIST***

In this lab, you will efficiently create, move, and remove files and directories by using 
the shell and a variety of file name matching techniques.
 
 **OUTCOMES**
 
  You should be able to:

    • Use wildcards to locate and manipulate files. 

**BEFORE YOU BEGIN** 

   Log in to workstation as student using student as the password.On workstation, run the lab files-review start command. 
    
   The command runs a start script that determines if the serverb machine is reachable on the network. 

*[student@workstation ~]$ lab files-review start*

1. Use the ssh command to log in to serverb as the student user. The systems are configured to use
    SSH keys for authentication, and therefore a password is not required.
    
*[student@workstation ~]$ ssh student@serverb* 

*[student@serverb ~]$*

2. Before you create project files, use the mkdir command with brace expansion to create empty project planning documents in the /home/student/Documents/project_plans directory. (Hint: if    ~/Documents does not exist, the -p option for the mkdir command will create it.)
Create two empty files in the ~/Documents/project_plans directory: season1_project_plan.odf and season2_project_plan.odf.

3. Create sets of empty practice files to use in this lab. If you do not immediately recognize the intended shell expansion shortcut, use the solution to learn and practice. Use shell tab completion to locate file path names easily.
Create a total of 12 files with names tv_seasonX_episodeY.ogg. Replace X with the season number and Y with that season's episode, for two seasons of six episodes each.

4. As the author of a successful series of mystery novels, your next bestseller's chapters are being edited for publishing. Create a total of eight files with names mystery_chapterX.odf. Replace X with the numbers 1 through 8. 

5. Use a single command to create two subdirectories named season1 and season2 under the Videos directory, to organize the TV episodes. 

6. Move the appropriate TV episodes into the season subdirectories. Use only two commands, specifying destinations using relative syntax.

7. Create a 2-level directory hierarchy with a single command to organize the mystery book chapters. Create my_bestseller under the Documents directory, and chapters under the new 
my_bestseller directory.

8. Create three more subdirectories directly under the my_bestseller directory using a single command. Name these subdirectories editor, changes, and vacation. The -p option (create parents) is not needed because the my_bestseller parent directory already exists.

9. Change to the chapters directory. Using the tilde (~) home directory shortcut to specify the source files, move all book chapters to the chapters directory, which is now your current directory. What is the simplest syntax to specify the destination directory?

10. You sent the first two chapters to the editor for review. Move only those two chapters to the editor directory to avoid modifying them during the review. Starting from the chapters subdirectory, use brace expansion with a range to specify the chapter file names to move and a relative path for the destination directory.

11. While on vacation you intend to write chapters 7 and 8. Use a single command to move the files from the chapters directory to the vacation directory. Specify the chapter file names using brace expansion with a list of strings and without using wildcard characters.

12. Change your working directory to ~/Videos/season2, and then copy the first episode of the season to the vacation directory.

13. Use a single cd command to change from your working directory to the ~/Documents/ my_bestseller/vacation directory. List its files. Use the previous working directory argument to return to the season2 directory. (This will succeed if the last directory change with the cd command was accomplished with one command rather than several cd commands.) From the season2 directory, copy the episode 2 file into the vacation directory. Use the shortcut again to return to the vacation directory.

14. The authors of chapters 5 and 6 want to experiment with possible changes. Copy both files from the ~/Documents/my_bestseller/chapters directory to the ~/Documents/ my_bestseller/changes directory to prevent these changes from modifying original files. Navigate to the ~/Documents/my_bestseller directory. Use square-bracket pattern matching to specify which chapter numbers to match in the filename argument of the cp command.

15. Change your current directory to the changes directory.
Use the date +%F command with command substitution to copy mystery_chapter5.odf to a new file which includes the full date. The name should have the form mystery_chapter5_YYYY-MM-DD.odf. 
Make another copy of mystery_chapter5.odf, appending the current time stamp (as the number of seconds since the epoch, 1970-01-01 00:00 UTC) to ensure a unique file name. Use command substitution with the date +%s command to accomplish this. 

16. After further review, you decide that the plot changes are not necessary. Delete the changes directory.
 If necessary, navigate to the changes directory and delete all the files within the directory. You cannot delete a directory while it is the current working directory. Change to the parent directory of the changes directory. Try to delete the empty directory using the rm command without the -r recursive option. This attempt should fail. Finally, use the rmdir command to delete the empty directory, which will succeed. 

17. When the vacation is over, the vacation directory is no longer needed. Delete it using the rm command with the recursive option.
When finished, return to the student user's home directory.

18. Create a hard link to the ~/Documents/project_plans/season2_project_plan.odf file named ~/Documents/backups/season2_project_plan.odf.back. A hard link will protect against accidental deletion of the original file and will keep the backup file updated as changes are made to the original.

19. Exit from serverb.

*[student@serverb ~]$ exit*

`logout Connection to serverb closed.`

*[student@workstation ~]$*

**Evaluation**

   On workstation, run the lab files-review grade script to confirm success on this lab. 

*[student@workstation ~]$ lab files-review grade* 

**Finish**

On workstation, run the lab files-review finish script to finish this lab. 
This script removes all files and directories created on serverb during the lab exercise. 

*[student@workstation ~]$ lab files-review finish*

    This concludes the lab. 
