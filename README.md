# IS601 MINI PROJECT
By [Wenjie Zhang](), [Vito DePalo]()
## Table of Content
1. [What is a repository](#What-is-a-repository)
2. [Cloning  a respository](#How-to-clone-respository)
3. [Forking a repository](#fork)
4. [Branch](#branch)
5. [Commit](#Commit)
6. [Merge](#merge)
7. [Checkout](#checkout)
8. [Push](#push)
9. [Pull](#pull)
10. [Remote Add / Remove / Show](#remote)
11. [Status](#status)
12. [Master Branch](#master)

## What is a repository
A repository is like a folder for your project. Your project's repository contains all of your project's files and stores each file's revision history.
## How to clone respository
type the following command
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
```
git pull 
```
## How to push to a remote respository
```
git push
```
## Branch