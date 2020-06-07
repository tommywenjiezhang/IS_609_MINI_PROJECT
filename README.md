# IS601 MINI PROJECT
By [Wenjie Zhang](), [Vito DePalo]()
### [link to our documentation](https://tommywenjiezhang.github.io/IS_609_MINI_PROJECT)

This project explains how the usage of Git, Docker, automated testing, and continuous integration can improve the productivity and competitiveness of a company.
1. GIT is a source code management tool, basically software that manages changes or a type of verison control. GIT is distributed Linux operating system software developed by the founder of Linux Linus Torvalds. GIT allowas developers to collaborate in software teams, revert changes and keep track of code, like an index through comments. Because GIT is a open collaborative tool it allows alot more flwxibility to the team that increases productivity and competitiveness as you can see changes and make comments dynamically tha also allows to adapt to changes more effectively and more efficiently.
2. Docker is a software containerization platform, meaning you can build your application, package them along with their dependencies into a container and then these containers can be easily shipped to run on other machines. As stated by Vineet Chaturvedi in the Docker Tutorial.The biggest advantage for productivity is that developers or other team members like testers can use docker without installing a special software application and using Docker on an open platform, and once again it is more effective and efficient to develop and modify code and get it into prodcuction.
3. Automated testing that can be acheived by using both Git and Docker can expand your testing capacity, the number of test cases, get faster feedback as the results are readily avaialble to the interested parties, and improve quality through more substantial testing opposed to manual testing.
4. Continuous Integration allows the developer to continuously integrate code into a single shared and easy to access repository. This leads to smaller code changes, faster times to debug, more test reliability, faster release dates and usually better customer satisfactiom which is key for better productivity and effective competitiveness in a company.

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
10. [Remote Add / Remove / Show](#Remote)
11. [Status](#Status)
12. [Master Branch](#master)
13. [Changelog](changlog.md)


## What is a repository
A repository is like a folder for your project. Your project's repository contains all of your project's files and stores each file's revision history.
## How to clone respository
git clone - creates a local copy or Clone of a project that already exists remotely.
```
git clone https://github.com/tommywenjiezhang/IS_609_MINI_PROJECT.git
```
## Fork
A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.
### Steps to Fork:
- Fork the repository.
- Make the fix.
- Submit a pull request to the project owner.
## Branch
Branch allows for parallel work. New development (such as features and non-emergency bug fixes) is done in feature branches, and is only merged back into main body of code when the developer(s) is happy that the code is ready for release.

**git branch** - shows the branches being worked on locally.
```
git branch 
git branch -a // "-a" flag will make sure remote branches are also included in the list.
git branch -d <branch> //Deletes a specified branch.
```
### How to create a new Branch 
To create a new branch and switch to it at the same time, you can run the git checkout command with the -b switch:
```
$ git checkout -b new
Switched to a new branch "new"
```
## Commit
The git commit command captures a snapshot of the project's currently staged changes. 
```
git commit -m"new Commit"
```
## Merge
The git merge command merges lines of development together. This command is typically used to combine changes made on two distinct branches.
Once you are comfortable with development in the new branch you merge it back into master by
```
git commit -a -m 'new change'
git checkout master
git merge new
```
## Checkout
git checkout - allows you to navigate between the branches created by git branch. Checking out a branch updates the files in the working directory to match the version stored in that branch.
```
git checkout master
```
## How to push to a remote respository
git push - updates the remote repository with any commits made locally to a branch.
```
git push <remote> <branch>
```
## How to fetch your respository
git pull- updates the local line of development with updates from ts remote counterpart.
```
git pull <remote-name> <branch-name>
```

## How to Add/Remove/Show Remote
To add a new remote, use the git remote add command in the directory where your repository is stored.
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
## Remote
The git remote command lets you create, view, and delete connections to other repositories.
Remote connections are more like bookmarks rather than direct links into other repositories.
### Creating  remote configurations
```
git remote add <name> <url>
```
### Removing a remote
The command git remote rm will remove the connection to the remote repository specified by the <name> parameter. 
```
git remote rm <name>
```
### Show
The show subcommand can be appended to git remote to give detailed output on the configuration of a remote. 
```
git remote show origin
```

## Status
Displays paths that have differences between the index file and the current HEAD commit, paths that have differences between the working tree and the index file, and paths in the working tree that are not tracked by Git 
###  usage
```
git status
```
## How to push to a remote respository
git push - updates the remote repository with any commits made locally to a branch.

```
git remote add origin https://github.com/user/repo.git
```
To remove a remote use the git remote rm command to remove a remote URL from your repository.
```
git remote rm <destination>
```
To see more information about a particular remote, you can use the git remote show <remote> command.
```
git remote show <origin>
```
## Status
You can use git status to check if your local branch is up-to-date with the original one.
```
git status
```
## Master Branch
```
The default branch name in Git is master . As you start making commits, you're given a master branch that points to the last commit you made. Every time you commit, the master branch pointer moves forward automatically.
```
## Sources ##
1. https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html
2. https://datasift.github.io/gitflow/IntroducingGitFlow.html
3. https://www.git-tower.com/learn/git/glossary
4. https://guides.github.com/features/mastering-markdown
