# Git-Basic-Documentation-relate-to-use-and-it-s-commands
Git Basic Documentation relate to use and it's commands

#1 Open htdocs in cmd OR any can open your project folder [cmd C:\xampp\htdocs\Project_name]

#2 Download live code from GIT
-> git clone <GIT_URL>

#3 Create branch
-> Git checkout -b <Branch_name>

#4 Switch to other Branch
-> git checkout <Branch_name_where_to_switch>

#5 Upload the files manually at created branches

#6 Save file locally 
-> git add --all

#7 Ready to upload on live
-> git commit -m "Add_comment_about_changes"

#8 Upload all files on live repo
-> git push <USERNAME>::: <PASSWORD>

#9 Pull new changes from repo to local
-> git fetch 

#10 Pull new changes to local successfully
-> git pull

#11 Merge 2 Branches
-> goto parent branch (Whatever you have)
-> Use step #4
-> git merge <Branch_name> 


#Following are also some basic rules/command that really helpfull :
-----------------------------

#1. Fetch and pull first before starting any work

#2 Clone the branch
-> git clone -b <branchname> <git hublink>

#3 git init

#4 git add README.md // add specific file
or
git add . // add all files

#5 git commit -m "first commit"
#6 git remote add origin <repo>
#7 git push -u origin master

#8. Commit all files and it's change 
->git add --all
->git commit -m 'Initial Commit'
->git push
Vi editor (esc+shift+:)wq

#9 Commit specific/single file
->git commit -m 'your comment for comit' -- ‘your path’
->git commit -m 'update 1.php file by web8' -- 1.php

#10 How to ignore some files and folders?
 - #10.a For a File
   -> git add -u
   -> git reset -- main/dontcheckmein.txt
 - #10.b For a folder
   -> git add -u
   -> git reset -- main/*

#11 How to add new file in repo?
->git add ‘file_path_that_you_want_add’

#12 How to pull data from git to live server?
-> git fetch
-> git pull

#13 Commands for MergeTool and Merge file
-> https://stackoverflow.com/a/163659

#14 How to identify the current repo?
-> git remote -v
=========================================================================

Following is the reference document that also helpfull :
-----------------------------

#1 Git basic document for startup 

- https://docs.gitlab.com/ee/topics/git/numerous_undo_possibilities_in_git/

Issue that faced while working with GIT and also given solution too :
-----------------------------

- https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html

#1 Issue 

fatal: Unable to create '/var/www/html/jtdev/.git/index.lock': File exists.

Another git process seems to be running in this repository, e.g.
an editor opened by 'git commit'. Please make sure all processes
are terminated then try again. If it still fails, a git process
may have crashed in this repository earlier:
remove the file manually to continue.

#1 Solution

rm -rf .git/index.lock
