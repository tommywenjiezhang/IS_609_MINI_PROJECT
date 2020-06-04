# IS601 MINI PROJECT
By [Wenjie Zhang](), [Vito DePalo]()

This projects explains how the usage of Git, Docker, automated testing, and continuous integration can improve the productivity and competitiveness of a company.
## gitFlow, git commands and terminology
The gitFlow Workflow is a lightweight branch based workflow built around the core Git commands used by teams around the globe. There are six steps to the Workflow. 
1. Create a branch, 
2. Add commits 
3. open a pull request 
4.  Discuss and review code, 
5.  Merge 
6.  Deploy.

## gitflow illustration ##
![GitFlow Diagram](https://datasift.github.io/gitflow/GitFlowFeatureBranches.png)

## Table of Content
1. [What is a repository](#What-is-a-repository)
2. [Cloning  a respository](#How-to-clone-respository)
3. [Forking a repository](#fork)
4. [Branch](#branch)
5. [Commit](#Commit)
6. [Merge](#merge)
7. [Checkout](#Checkout)
8. [Push](#Push)
9. [Pull](#pull)
10. [Remote Add / Remove / Show](#remote)
11. [Status](#status)
12. [Master Branch](#master)


## What is a repository
A repository is like a folder for your project. Your project's repository contains all of your project's files and stores each file's revision history.
## How to clone respository
git clone - creates a local copy or Clone of a project that already exists remotely.
```
git clone https://github.com/tommywenjiezhang/IS_609_MINI_PROJECT.git
```
##Fork
A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.
###Steps to Fork:
- Fork the repository.
- Make the fix.
- Submit a pull request to the project owner.
##Branch
Branch allows for parallel work. New development (such as features and non-emergency bug fixes) is done in feature branches, and is only merged back into main body of code when the developer(s) is happy that the code is ready for release.

**git branch** - shows the branches being worked on locally.
```
git branch 
git branch -a // "-a" flag will make sure remote branches are also included in the list.
git branch -d <branch> //Deletes a specified branch.
```
###How to create a new Branch 
To create a new branch and switch to it at the same time, you can run the git checkout command with the -b switch:
```
$ git checkout -b new
Switched to a new branch "new"
```
Once you are comfortable with development in the new branch you merge it back into master by
```
git commit -a -m 'new change'
git checkout master
git merge new
```
##Commit
The git commit command captures a snapshot of the project's currently staged changes. 
```
git commit -m"new Commit"
```
## How to fetch your respository
git pull- updates the local line of development with updates from ts remote counterpart.
```
git pull
```
## Merge
Incorporates changes from the named commits (since the time their histories diverged from the current branch) into the current branch. 
```
 A---B---C feature
	 /         \
    D---E---F---G---H master
```
### How to merge
```
 git merge fixes enhancements
```
## Checkout
The git checkout command lets you navigate between the branches created by git branch. Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch. 
```
git branch
master
another_branch
feature_inprogress_branch
git checkout feature_inprogress_branch
```
## Push
The git push command is used to upload local repository content to a remote repository. 
```
git push <remote> <branch>
```
## How to push to a remote respository
git push - updates the remote repository with any commits made locally to a branch.
```
git push
```



