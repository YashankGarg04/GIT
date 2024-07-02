# GIT
It is a popular version control system , Used to perform Coding Collaboration and to track Changes

## What does git do?
* Manage projects with Repositories
* Clone a project to work on a local copy
* Control and track changes with Staging and Committing
* Branch and Merge to allow for work on different parts and versions of a project
* Pull the latest version of the project to a local copy
* Push local updates to the main project

## Some Coding Examples 
```
mkdir myproject
cd myproject
git init
```
This would Initiallize git into **myproject** folder
```
git status
```
It is used to Find status of the folder and check for Commits or untracked files 
```
git add <file-name>
git add --all
```
These Functions are used to update or add any new file to the Project
> Note: git add -A can also be used as an alternative of git add --all

```
git commit -a -m "Hey there this is my Commit"
```
`git commit` is used to commit the files its like a save point or a check point which saves the files which could be recovered even if it is removed, `-a` if we use with oour commit Staging step is not required it is done only if small changes are done to some files and `-m`is used to give a message it is recommended because it could be helpful while looking into Logs 
> Use of `git log` is done to check logs within the git project


