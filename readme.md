# **Git Tutorial**

- [**Git Tutorial**](#git-tutorial)
  - [What is Git?](#what-is-git)
  - [Basic terms and defenition](#basic-terms-and-defenition)
  - [Installation of Git on local desktop](#installation-of-git-on-local-desktop)
  - [Configure the user information](#configure-the-user-information)
    - [Name of the user](#name-of-the-user)
    - [Email-ID of the user](#email-id-of-the-user)
  - [Install git in local repository](#install-git-in-local-repository)
    - [Intitialize git](#intitialize-git)
    - [Cloning the repository](#cloning-the-repository)
  - [.gitignore file](#gitignore-file)
  - [Sync changes](#sync-changes)
    - [**git status**](#git-status)
    - [**git add**](#git-add)
      - [Adding a single file](#adding-a-single-file)
      - [Adding all the files](#adding-all-the-files)
    - [**git mv**](#git-mv)
    - [**git rm**](#git-rm)
    - [**git restore**](#git-restore)
    - [**git commit**](#git-commit)
      - [Commit with a small description about it](#commit-with-a-small-description-about-it)
      - [Commit an unstaged or untracked file](#commit-an-unstaged-or-untracked-file)
    - [**git diff**](#git-diff)
    - [**git log**](#git-log)
      - [Provides all the commits in one line](#provides-all-the-commits-in-one-line)
      - [Provides all the commits in detail](#provides-all-the-commits-in-detail)
  - [Branches in git](#branches-in-git)
    - [Provides all the branches present in the repository](#provides-all-the-branches-present-in-the-repository)
    - [Switch from one branch to another](#switch-from-one-branch-to-another)
    - [Deleting the branch](#deleting-the-branch)
    - [Merging the branches](#merging-the-branches)
   

## What is Git?
>Git is a widely used modern version control system for tracking changes in computer files.Git is the open source distributed version control system that facilitates GitHub activities on your laptop or desktop


## Basic terms and defenition
>clone: a local version of a repository, including all commits and branches<br><br>
remote: a common repository on GitHub that all team member use to exchange their changes<br><br>
fork: a copy of a repository on GitHub owned by a different user<br><br>
pull request: a place to compare and discuss the differences introduced on a branch with reviews, comments, integrated
tests, and more<br>
 

## Installation of Git on local desktop
```
https://git-scm.com/downloads
```

## Configure the user information
### Name of the user
```
git config --global user.name "[name]"
```

### Email-ID of the user
```
git config --global user.email "[email-ID]"
```

## Install git in local repository
### Intitialize git 
This will initialize git on a local repository
```
git init
```

### Cloning the repository
This will clone all the files , branches , commits that already exists on github.
```
git clone [url]
```


## .gitignore file

Sometimes it may be a good idea to exclude files from being
tracked with Git. This is typically done in a special file named .gitignore 

## Sync changes
### **git status**
Provides the current status of the repository
``` 
 git status
```

### **git add**
Adds a file to the tracked or staged list
#### Adding a single file
```
git add filename 
```
#### Adding all the files
```
git add .
```
### **git mv**
Renaming the file
```
git mv "oldname" "newname"
```

### **git rm**
Removing the file
```
git rm filename
```

### **git restore**
Restores the file
```
git restore filename
```

### **git commit**
The commit command makes sure that the changes are saved to the local repository.
#### Commit with a small description about it
```
git commit -m "message"
```
#### Commit an unstaged or untracked file
```
git commit -a -m "message"
```

### **git diff**
The git diff command can be used to show differences between commits

```
git diff
```

### **git log**
The git log command is used to display the commit history of a Git repository

#### Provides all the commits in one line
```
git log --oneline
```

#### Provides all the commits in detail
```
git log -p
```

## Branches in git

### Provides all the branches present in the repository

```
git branch
```

### Switch from one branch to another

```
git switch branchname
```
or
```
git checkout branchname
```

### Deleting the branch 

```
git branch -d branchname
```

### Merging the branches

```
git merge -m "message" branchname 
```