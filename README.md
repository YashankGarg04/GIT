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
`git commit` is used to commit the files its like a save point or a check point which saves the files which could be recovered even if it is removed, `-a` if we use with our commit Staging step is not required it is done only if small changes are done to some files and `-m`is used to give a message it is recommended because it could be helpful while looking into Logs 
> Use of `git log` is done to check logs within the git project

## GIT and GITHUB
Once a local GIT repo is created we can then push it to GitHub , First we need to create repository inside our Github and then copy the URl to the repository 
```
git remote add origin <URL>
git push --set-upstream origin master
```
> **Note:** If connecting first time Git to GitHub it will require authentication 
### Pull Changes
This is combination of `fetch` and `merge`. It is used in Git to update your local repo if any change is made via GitHub
```
\\Fetching
git fetch origin
\\merge
git merge origin/master
\\here master is the local branch and origin is the branch on GitHub
\\We can also directly use pull to reduce efforts
git pull origin
```
**We can also Pull from a branch on Github**
```
git branch -a
\\Using this command we can check all remote and local branches
git checkout <branch-name>
\\ This to change to the remote branch
git pull
```
> **Note:** `branch -r` is used to only check remote branches

### Push Changes
Similar to Pull if changes are made in Local Repo we can directly commit and push to GitHub
```
git commit -a -m "Message"
git push origin
```
**We can also Push local branches**
```
git checkout -b <branch-name>
git commit -m "Message"
git push origin <branch-name>
\\In github once pushing branches we can check the changes made and create the pull request and then we can merge
```
