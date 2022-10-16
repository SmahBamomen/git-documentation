# Git Documentation

## Table Of Content 
- [Structure](#Structure)
  * [1.1 Purpose](#11-purpose)
  * [1.2 Scope](#12-scope)
  * [1.3 Acronyms](#13-acronyms)
  * [1.4 References](#14-references)
    + [1.4.1 Internal References](#141-internal-references)
    + [1.4.2 External References](#142-external-references)
  * [1.5 Overview](#15-overview)
 - [Git Commands](#GitCommands)

<a name="Structure"/>
<a name="GitCommands"/>


## Structure


## Git Commands

![Git Command Flow](https://miro.medium.com/max/1400/1*69prApOy8_cZPnmRHGHQZg.png  "Git Command Flow")

Git is an important part of daily programming and is commonly used in the software industry. Here are listed commands that are commenly used that every developer should know.



#### Git Init
The `git init` command creates a new Git repository. Executing `git init` creates a `.git` subdirectory in the current working directory, which contains all of the necessary Git metadata for the new repository.

#### Git Status

The `git status`command  lets you see which changes have been staged, which haven’t, and which files aren’t being tracked by Git. Status output does not show you any information regarding the committed project history. For this, you need to use `git log`.

We can gather information like:

- Whether the current branch is up to date
- Whether there is anything to commit, push or pull
- Whether there are files staged, unstaged or untracked
- Whether there are files created, modified or deleted

#### Git Add
Adding changes from "Working Directory" to Git's "Staging Area".

- To Add a single file:
```
git add <file name>
```

- To add everything in once :
```
git add .
```

**Important: The git add command doesn't change the repository and the changes are not saved until we use git commit.**

#### Git Commit
Taking snapshots to your work and moving it from the "Staging Area" to Git's "Repository"
When Commiting, you need to write a message to explain what you did or developed

```
git commit -m "commit message"
```


#### Git Branch 
Branches are highly important in the git world. By using branches, several developers are able to work in parallel on the same project simultaneously.
We explained **here** in details about `git branch` including how to create, delete, and merging them.

#### Git Push

After committing your changes, the next thing you want to do is send your changes to the remote server. Git push uploads your commits to the remote repository.

```
git push <remote> <branch-name>
```

**However**, if your branch is newly created, then you also need to upload the branch with the following command:

```
git push -u origin <branch_name>
```

**Important: Git push only uploads changes that are committed.**

#### Git Pull
`git pull`is  a command used to update the local version of a repository from a remote. It does two thing:
does two things.
- Updates the current local working branch (currently checked out branch)
- Updates the remote tracking branches for all other branches.

``` 
# General format
git pull

# Pull from specific branch
git pull REMOTE-NAME BRANCH-NAME
```

#### Git Clone
The `git clone` command is used to create a copy of a specific repository or branch within a repository.
```
git clone <Repository URL>  

```

## Branches



