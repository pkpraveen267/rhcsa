CREATING, VIEWING, AND EDITING TEXT FILES 
PERFORMANCE CHECKLIST 
In this lab you will edit a text file, using the vim editor. 
OUTCOMES 
You should be able to: 
• Use Vim to perform file editing. 
• Use visual mode to simplify file editing. 
BEFORE YOU BEGIN 
Log in to workstation as student using student as the password. 
On workstation, run the lab edit-review start command. 
[student@workstation ~]$ lab edit-review start 
1. Redirect a long listing of all content in the student's home directory, including hidden directories and files, into a file named editing_final_lab.txt.
2. Edit the file using Vim.
3. Remove the first three lines. Enter line-based visual mode with uppercase V.
4. Remove columns on the first line. Enter visual mode with lowercase v. Lowercase v selects characters on a single line only. The columns after -rw- should be deleted.
5. Remove columns, and the subsequent dot (".") on the remaining lines. Use the visual block mode. Enter visual block with the control sequence Ctrl+V. Use this key sequence to select a block of characters on multiple lines. The columns after -rw- should be deleted.
6. Use visual block mode to remove the fourth column.
7. Use visual block mode to remove the time column, leaving the month and day on all lines.
8. Remove the Desktop and Public rows. Enter visual line mode with uppercase V.
9. Use the :wq command to save and exit the file. Make a backup, using the date (in seconds) to create a unique file name.
10. Append a dashed line to the file. The dashed line should contain at least 12 dashes.
11. Append a directory listing of the Documents directory. List the directory listing on the terminal and send it to the editing_final_lab.txt file with one command line.
12. Confirm that the directory listing is at the bottom of the lab file.
Evaluation 
On workstation, run the lab edit-review grade command to confirm success of this exercise. 
[student@workstation ~]$ lab edit-review grade 
Finish 
On workstation, run the lab edit-review finish script to complete this exercise. 
[student@workstation ~]$ lab edit-review finish 
This concludes the lab. 
