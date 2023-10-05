## Open Sourse Lecture Week 5 HomeWork

Introduction: This document is a lecture note about Shell command  
Please skip this file if this is not your interest.  

---
**1. I/O Redirection: Standard Output**  
the screen we see == default standard output  
If we want, we can change the output into something else rather than just screen.  
One way to do so is using **">"**
By putting **">"** after the command, we can redriect output.  
After putting **">"**, we should add file that will save the output, and the file can be new one.

Additionally, **">>"** means appends output to an exsiting file or create and write to a new file if it does not exist.  
Command **"cat"** means showing the content of a text file.


*Usage Example*
![output picture 1](https://github.com/kda5337/lecture_note_5-2/assets/144139251/7ec49e0a-1cdf-407e-a08f-4d7334b2cc13)

![output picture 2](https://github.com/kda5337/lecture_note_5-2/assets/144139251/b3d6e30d-74ef-44eb-8a08-4b67cd50c8a6)
  
  
**2. I/O Redirection: Standard Input**  
keyboard == default standard input  
**"<"** == Redirecting input  
We can mix **"<"** and **">"** in a single line

**3. Pipelines "|"**  
Funtion: give output of previous command to input of next command.  
For example, if there is any command like "command 1 | command 2 | command 3 | ...", this means that the output of command 1 goes to command 2 input.
Output of command 2, which input is output of command 1, becomes the input of command 3.

**4. Expansion**  
Some special characters expand its meaning when given to shell commands.
command 'echo' == print out the text  
'echo *' == print out the file in the current directory  
'echo ~' == the home directory of current user  
'echo ~(user name)' == you can check the home firectory of (user name)  
***TIPS: Use backslash(/) to ignore the line change in command when enter the long command.***  

**5. Permissions**  
Permission of files and directories assigned to owner / group / others is different since Linux is a multi-user system.  

Permission could be identify through follow code.  
![permission picture 1](https://github.com/kda5337/lecture_note_5-2/assets/144139251/1b49402b-12cf-49e7-b2af-e3e5a5d284fd)  
  

![permission picture 2](https://github.com/kda5337/lecture_note_5-2/assets/144139251/7bc3ba87-c788-4c13-bafc-53b3a1c0383a)  
The code in this picture means that file owner has permission to read, write, and execute.  
While the group owner only have permission to read and execute, not write.  
Finally, all other users can read and execute the files, not write.  



