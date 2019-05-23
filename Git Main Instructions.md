# Git Main Instructions

Git has tree main states that our files can reside in: _committed, modified_, and _staged_.

+ **Committed** means that the data is safely stored in our local database.
+ **Modified** means that you have changed the file but have not committed it to our database yet.
+ **Staged** means that you have marked a modified file in its current version to go into our next commit snapshot.

Three locals areas:
+ **Working tree**: where are the files where you are working actually.
+ **Index**: is the staging area where the validations are ready to be committed.
+ **Head**: the repository.

And one remote repository, where you can share the changes you do.

![Git working](https://i1.wp.com/foxutech.com/wp-content/uploads/2018/02/GIT-interview-Question-and-Answers.png?fit=1100%2C481&ssl=1&resize=350%2C200)

-----

## Git Basics

| Git basics | |
|:----- | :----- |
| `git init`| Creates a new local repository (/.git) |
| `git clone <url>` | Creates a copy of a remot repository |
| `git status` | List all files news and modified compared with the head |
| `git add [-u] [filename.pattern]` | Makes a snapshot of the files to add them to the staged area. The parameter -u adds the files that must be erased | 
| `git commit [-m "Message"]` | Saves the snapshots of the files permanently to the Head |
| `git push origin master` | Charge all the validated files of the local branch to the remot repository |
| `git pull origin master` | Download and incorporates the changes from the remot repository |

------

You typically obtain a Git repository in one of two ways:

1. You can take a local directory that is currently not under version control, and turn it into a Git repository.
2. You can _clone_ an existing repository from elsewhere.

In both cases, you end up with a Git repository on our local machine ready to work.

-----

### Git init

If you have a project directory that is currently not under version control and you want to start controlling it with Git, you first need to do to that project's directory and type:

`git init`

This command creates a new subdirectory named `.git` that contains all of our necessary repository file.

If you want to start version-controlling existing files, you should probably begin tracking those files and do an initial commit. You can accomplish that with a few `git add` commands that specify the files you want to track, followed by a `git commit`:

```
$ git add *.c
$ git add LICENSE
$ git commit -m 'initial project version'
```

At this point, you have a Git repository with tracked files and an initial commit.

-----

### Git clone

If you want to get a copy of an existing Git repository, the command you need is:

```
git clone http://github.com/user_organization/github_repository
```

That creates a directorty named `github_repository`, initializes a .git directory inside it, pulls down all the data for that repository and checks out a working copy of the latest version.

------

### Recording changes to the repository

When you clone a repository, all of our files will be tracked and unmodified because Git just checked them out and you haven't edited anything.

As you edit files, Git sees them as modified, because you've changed them since our last commit. As you work, you selectively stage these modified files and then commit all those staged changes, and the cycle repeats.

The main tool you use to determine which files are in which state is the `git status` command. If you run this command direcly after a clone, you should see something like this:

```
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean
```

This means you have a clean working directory. If you add a new file to our project, if the file didn't exist before and you run `git status`, you see our untrascked file like so:

```
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
    (use 'git add <file>...' to include in what will be committed)

    FILE

nothing added to commmit but untracked files present (se 'git add' to track)
```

### Tracking New Files

In order to begin tracking a new file, you use the command `git add`. To begin tracking the `FILE`, you can run this:

```
$ git add FILE
```

If you run `git status` command again, you can see that FILE is now tracked and staged to be commited.

-----

## Git Fast Cheat Sheet

| Create & Clone | |
| :-----: | :-----|
| __Create new__ repository | `git init` |
| __Clone local__ repositor | `git clone /path/to/repository` |
| __Clone remote__ repository | `git clone username@host:/path/to/repository` | 

-----

| Add & Remove | |
| :-----: | :-----|
| __Add__ changes to INDEX | `git add <filename>` |
| __Add all__ changes to INDEX | `git add *` |
| __Remove/delete__ | `git rm <filename>` |

------

| Commit & Synchronize | |
| :-----: | :-----|
| Commit changes | `git commit -m "Commit message"`|
| Push changes to remote repository | `git push origin master` |
| __Connect__ local repository to remote repository | `git remote add origin <server>` |
| __Update__ local repository with remote changes | `git pull` |

------

| Branches| |
| :-----: | :-----|
| __Create__ new branch | `git checkout -b <branch>` |
| __Switch to__ master branch | `git checkour master` |
| __Delete__ branch | `git branch -d <branch>` |
| __Push branch__ to remote repository | `git push origin <branch>` |

-------

| Merge| |
| :-----: | :-----|
| __Merge changes__ from another branch | `git merge <branch>`|
| __View changes__ between two branches | `git diff <source_branch> <target_branch>` |