# GitHub
## GitHub configuration
One can add their name and email address and other configuration information using 

```
git config --global user.name "name"
git config --global user.email "emailID"
```

# To initiate the GitHub from scrach 
```
git init
```
With these the basic settings are done and git folders will be created.

# Git folder 
.git/ folder is created upon 'git init' and this stores all the configuration information of the repository.


# To check the status of the git 
```
git status
```
This shows the status of the repository. How many files are yet to be commited to the branch and how many files are in added tack.

# To add a file 
```
git add <filepath>
```
This command adds the file to the track but it doesn't commit it to the repository yet.

# To commit to the repository
```
git commit <filepath>
```
This command commits all the modified files, all the files in the ad track to the repository and stores in the database.

# To see the history of the repository
```
git log 
```
This command shows what all have happened in the repository with small messages.with the date and time when the commits were made.

# Writitng a commit message 
after you give the command 
```
git commit 
```
you will be directed to write a commit message.
A good commit message,
1st line should give a small context on the change, after a small gap. A paragraph with a comprehensive explanation would be a good commit message. The message should have 72 characters in length so that the message doesn't get hidden in the screen. # are used to moslty for the coder's own understanding and are often ignored by others. A commit is aborted without a commit message. So, a good commit message is always important.

# Skipping the stage step
Usually when you want to ccommit your new file to the repository you first stage them using 'git add' and then 'git commit' but if you want to commit a already existing modified file without stagign them first you can completely skip the 'git add' command and directly commit them using 
```
git commit -a
```
This command commits and tracks the modified file but we should note that this feature is used only to a modified file and not a new file. New files has to stagged first inorder for them to be tracked in the future.

If your commit is really a small modification and just doesn't have to be complex and if you are sure of the change then we can use both -a and -m flags like below
```
git commit -a -m "a short message on the change"
```
This helps to skip stagging and commit with a short message in same time, but this has to be done only when you are sure of the small change and it doesn't need any big explanation.

Once you do the commit check it with 'git log' command
you will see 
(HEAD->master)
this always indicates that the latest commit is done to the master branch of the repository. We will see how to modify just a branch and not the master later.

# To check the small modification 
After commiting the changes you can check what's changed using 
```
git log -p
```
This command will show the lines that were added or removed to the program.
This command is similar to 
```
diff -u
```
command used before to see the changes made in the program 
```
git show <commit ID>
```
this helps to check the changes as well by sepcifying the exact commit 

# To check all the changes and no of lines you can use
```
git log --stat
```

# To check the patch wile stagging 
```
git add -p 
```
asks you whether to commit the changes by showing the new patch that's modified.


