# This is my Git and Github Courses
# Terminology
  - git --version

# Repository
  - git status 
  - git config --list
# Your config settings  
  - git config --global user.email"malikabdulsattar9947@gmail.com"
  - git congig --global user.name"AbdulSattar-07"
# Creating a repository 
## Stage 
  - git status
  - git init
  - git add <filename1><filename2> and up to so on 
  - git add . ---> for all files which are to be add
## Commit  
  - git commit -m "commit message"
  - git status
## Logs
  - git log 
  - git log --oneline 

## gitignore
  - add .gitignore

# Branches in Git
  - git branch
  - git branch bug-fix
  - git switch master
  - git log
  - git switch -c dark-mode    (not noly creat but also switch to that branch also) 
  - git checkout orange-mode   (check out either the branch exist or not if present then switch to that branch  )

## Merging branches
### 1. Fast-forward merge
  - git checkout master    ( now head at master branch )
  - git merge bug-fix      (merge the code of that branch to main branch)
### 2. Slow farward merge
  - git checkout master    (working in this brache at the same time)
  - git merge bug- fix     (working in this brache at the same time)

  - git config --global core.editor "code --wait" ---> Its a important file
## Rename a branch
  - git branch -m <old-branch-name> <new-branch-name>
## Delete a branch
  - git branch -d <branch-name>    
 
## Checkout a branch
  - git checkout <branch-name>
## List all branches
 - git branch  


# Git diff
  - git diff  
## Comparing Staging Area with Repository
  -  git diff --staged  
## Comparing Two Branches
  - git diff <branch-name-one> <branch-name-two> 
  - git diff branch-name-one..branch-name-two  
## Comparing Specific Commits:
  - git diff <commit-hash-one> <commit-hash-two>  

# Git Stash
  - git stash

## Naming the stash
  - git stash save "work in progress on X feature" 
## View the stash list
  - git stash list
## Apply the Most Recent Stash
  - git stash apply
## Apply Specific Stash
  - git stash apply stash@{0}
## Applying and Drop a Stash
  - git stash pop
## Drop the stash
  - git stash drop
## Applying stash to a specific branch
  - git stash apply stash@{0} <branch-name>
## Clearing the stash
  - git stash clear         

# Git Tags
## Creating a tag
  - git tag <tag-name>
## Create an annotated tag
  - git tag -a <tag-name> -m "Release 1.0"
## List all tags
  - git tag  
## Tagging a specific commit
  - git tag <tag-name> <commit-hash>

## Push tags to remote repository
  - git push origin <tag-name>

## Delete a tag
  - git tag -d <tag-name>
## Delete tag on remote repository
  - git push origin :<tag-name>  


# Managing History
## Rebase in git
  - git checkout feature-branch
  - git rebase main 
## Resolve any conflicts
  - git add <resolved-files>
  - git rebase --continue   
## Git reflog
### View the reflog:
  - git reflog
### Find specific commit
  - git reflog <commit-hash>
### Recover lost commits or changes
  - git reflog <commit-hash>
  - git reset --hard <commit-hash>
  - git reflog <commit-hash>
  - git reset --hard HEAD@{1}   


# Github  
## Configuring Git
  - git config --global user.email "1abdulsattar32304@gmail.com"
  - git config --global user.name "1abdulsattar32304-prog" 
  - git config --list  
## Setup SSH Key
  - ssh-keygen -t ed25519 -C "1abdulsattar32304@gmail.com"
                         Control Panel → Credential Manager → Windows Credentials


## Publish Code to Remote Repository
  - git init
  - git add <filesname>
  - git commit -m "commit message"
  - git branch -M main   (rename the master branch to main branch )
## Remote URL Setting
  - git remote -v
### Add Remote Repository
  - git remote add origin https://github.com/1abdulsattar32304-prog/first_github_course_repo.git  

## Pushing Code
  - git push origin main

### Setup an upstream remote
  - git remote add upstream <remote-url>
  - git remote add -u <remote-url>
  - git push -u origin main

### Fetch code
  - git fetch <remote-name>
## Pull code
  - git pull origin main  
  
   
  
