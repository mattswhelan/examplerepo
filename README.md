# Hello this is an example github repo

# New Heading
Can you see this change?

* Bullet point one
* bullet point two

1. list item
2. list item


This readme is written in Markdown.
For more information on Markdown, see:
* [The Github-Flavored Markdown Guide](https://guides.github.com/features/mastering-markdown/)
* [The Github-Flavored Markdown Spec](https://github.github.com/gfm/)

Content using &lt;these brackets> is variable.


## Getting Started with Git
### Configure Identity
`git config --global user.name <"John Doe">`

`git config --global user.email <johndoe@example.com>`

The name and email address you configure here is used with any commits you make.

### Git clone
The `git clone` command copies an existing Git repo into a local directory.

`git clone <repoURL>`

For example:

`git clone https://github.com/mattswhelan/examplerepo`

### Git pull
The `git pull` command updates your local directory with any changes to the repo, then attempts to merge those changes with your work. Git pull synchronizes everyone's work.

# Workflow
1. Edit files in a repo locally.
2. (Optional) `git status` to view the state of any local changes.
3. `git pull` to update your repo.
3. `git add <changedfile>` to select changes to stage.
4. (Optional) `git diff` to view a summary of any local changes.
5. `git commit -m` to commit your changes.
6. `git push` to push your local changes out to the current branch of your repo.


## What Has Changed/What is Happening/Help
### Git status
The `git status` command displays the state of any changes in your working directory. These states include:
* Changes made locally that are not staged
* Changes made locally that are staged
* Changes made locally that are committed
* Merge conflicts

The `git status` command is useful to run if you are confused.

### Git log
The `git log` command uses commits to display the history of your project.

>Press Shift+Q to exit the commit log.

### Git diff
The `git diff` command shows a summary of any local changes.
>Press Shift+Q to exit the diff log.

## Saving Changes
### Git add
The `git add` command locally stages and tracks changes made to the specified file(s). These changes could be edits to a file, a file getting deleted, or a file being added to a project. Use `git add` to prepare content for a `commit`. Anything that changed in your working directory can added.

* `git add <filename.extension>`

Stages and tracks the changes made to the specified file.

* `git add <filename.extension1> <filename.extension2> <filename.extension1>`

Stages and tracks the changes made to all of the specified files.

* `git add <directory>`

Stages and tracks all changes made in a specific directory.

* `git add .` or `git add *`

Stages and tracks all changes made.

>This command will only add content in the current working directory and any subdirectories below it. If you wish to add _all_ local changes, navigate to your root project directory before using `git add .`. Or you could just right click the root project directory and select git bash on windows. That also works.


### Git commit
The `git commit` command creates a "snapshot" of a staged change in your project history. When you `commit` a change, include a short message describing the change. You must `add` changes before you `commit` them.


* `git commit <file.extension> -m "<yourmessage>"`

Creates a commit for a specified file.


* `git commit <file.extension1> <file.extension2> <file.extension1> -m "<yourmessage>"`

Stages and tracks the changes made to all of the specified files.

* `git commit <directory> -m "<yourmessage>"`

Creates a checkpoint of a staged changes made in a specific directory.


* `git commit -m "<yourmessage>"`

Stages and tracks all changes made.

For example:

`git commit -m "this is a commit message"`

>If you forget to type -m as part of your commit then vi opens. To exit vi, type :q and press enter.

### Git push
The `git push` command pushes your local changes out to the repo.

## Branches
Use the `git checkout -b <branchname>` command to create a new branch and switch to it. Checking out a branch will change your current working directory to match the contents of that branch.

Follow up by using the `git push --set-upstream origin <branchname>` command to set your new branch to point to origin.


Use the `git checkout <branchname>` command to switch to an existing branch. Checking out a branch will change your current working directory to match the contents of that branch.

## Fixing Mistakes
### Git Checkout
You can also use the `git checkout` command to change your working directory to match an older version of your project.


`git checkout <file>`

Changes the contents a file in your working directory to match the last commit on that file for the branch you are currently working on.


`git checkout <commit_sha>`

Changes the contents of your current working directory to match the specified commit.


`git checkout <commit_sha> <file>`

Changes the contents of a specified file to match the specified commit.


`git revert <commit_sha>`

Git revert functions as an undo command. Git revert undos the changes made in a specific commit without deleting the project history.

### Fix Mistakes with add or commit
`git reset --soft HEAD^`

Resets a `commit` while preserving the status of your working directory.


`git reset HEAD <file>`

Resets an `added` change while preserving the status of your working directory.

### Resolving Merge Conflicts Locally

<<<<<<< HEAD
Differences in the head branch (active branch).
========


Differences in the destination branch (branch you are merging into).

&gt;&gt;&gt;&gt;&gt;&gt;&gt;&gt;&gt;



<!--Get to this later

git commit -am "<yourmessage>"
adds and commits all current local changes.

git reset --hard HEAD~1

git reset --hard <commit_sha>

git merge --abort

git cherry-pick <commit_sha>

Remotes
git remote add origin
git push -u origin master

-->
