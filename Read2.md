

1. Version Control: is a system that allows you to re-visit various versions of a file or set files by recording changes.VCS can solve mistakes easily and correctly.
CVCS  includes a single server storing all file versions, which can be accessed by various clients.this sysytem allowed programmers to have more knowledge of team members’ activities, and gave administrators much more control over dividing a revision privileges.

2. (DVCS): If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions. DVCS allows clients to create mirrored repositories( like copy) because of that programmers working in teams can collaborate with each other in various ways to complete a joint project.

3. Git is a DVCS that stores data in a file system made up Each time you save a changed version of your project (called commit) Git creates a snapshot of the file and stores a reference to it. If the file does not changed, Git only stores a reference to the already-stored identical version of it.

4. Every single change applied to any file or directory is tracked by Git. 
5. git config ---> to set configuration variables.
6. after installing git set username and email
7. to verify correct setting re-write set instruction for email and username.you should recieve the same thing you entered
8. to check settings write git config --list. the setting you enterer will appear
9. to access manual git help *command* 
10. to import an existing project first: you have yo switch to the project that you want second:write git initial command third:start tracking
11. to make a copy of an existing project $git clone (repository url)
12. The local Git repository has three components:
      1. Working Directory: The actual files reside here.
      2. Index: The area used for staging
      3. Index: The area used for staging
13. Tracked files can be modified, unmodified, or staged
14. Untracked files were not in the last snapshot 
15. to check files write git status
16. git add filename to track single file
17. git add * to track all files
18. commit the changes and record what you did $ git commit -m “made change x,y,z”
19. if you want to commit all records $ git commit -a
20. to push changes to a remote repository $ git push origin master
21. git stash This command temporarily removes changes and hides them, giving you a clean working directory.





