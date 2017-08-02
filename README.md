# Hello this is the example github repo

This readme is written in markdown.
Content using <these brackets> is variable.

## Getting Started with Git
### Configure Identify
`git config --global user.name <"John Doe">`
`git config --global user.email <johndoe@example.com>`

The name and email address you configure here is used with any commits you make.

### Git clone
The `git clone` command copies an existing Git repo into a local directory.
`git clone <repoURL>` for example, `git clone https://github.com/mattswhelan/examplerepo`

### Git pull
The `git pull` command updates your local directory with any changes to the repo, then attempts to merge those changes with your work. Git pull synchronizes everyone's work.

# Workflow
1. Edit files in a repo locally.
2. (Optional) `git status` to view the state of any local changes.
3. `git pull` to update your repo.
3. `git add <changedcontent>` to select changes to stage.
4. (Optional) `git diff` to view a summary of any local changes.
5. `git commit -m` to commit your changes.
6. `git push` to push your local changes out to the current branch of your repoThe Customer Context gadget now supports dropdowns. In the customer record, you can use dropdowns to select a customer's preferred language if you are using the cisco.base.customer fieldset..


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

### Git add
The `git add` command locally stages and tracks changes made to the specified file(s). These changes could be edits to a file, a file getting deleted, or a file being added to a project. Use `git add` to prepare content for a `commit`. Anything that changed in your working directory can added.

`git add <filename.extension>`
Stages and tracks the changes made to the specified file.

`git add <filename.extension1> <filename.extension2> <filename.extension1>`
Stages and tracks the changes made to all of the specified files.

`git add <directory>`
Stages and tracks all changes made in a specific directory.

`git add .`
Stages and tracks all changes made.

>This command will only add content in the current working directory and any subdirectories below it. If you wish to add _all_ local changes, navigate to your root project directory before using `git add .`. Or you could just right click the root project directory and select git bash on windows. That also works.


### Git commit
The `git commit` command creates a "checkpoint" of all changes committed. You must `add` changes before you `commit` them.

`git commit <filename.extension> -m "<yourmessage>"`
Stages and tracks the changes made to the specified file.

`git commit <filename.extension1> <filename.extension2> <filename.extension1> -m "<yourmessage>"`
Stages and tracks the changes made to all of the specified files.

`git commit <directory> -m "<yourmessage>"`
Stages and tracks all changes made in a specific directory.

`git commit -m "<yourmessage>"`
Stages and tracks all changes made.

For example, git commit -m "this is a commit message"

>If you forget to type -m as part of your commit then vi opens. To exit vi, type :q.

### Git push
The `git push` command

## Branches
Use the `git checkout -b <branchname>` to create a new branch and switch to it. Checking out a branch will change your current working directory to match the contents of that branch.

Use the `git checkout <branchname>` to switch to an existing branch. Checking out a branch will change your current working directory to match the contents of that branch.

## Fixing mistakes
### Git Checkout
The `git checkout` command can be used to change your working directory to match an older version of your project.

`git checkout <currentbranchname>`
Changes the contents of your current working directory to match the branch you are currently working on.

`git checkout <commit_sha>`
Changes the contents of your current working directory to match the specified commit.

`git checkout <commit_sha> <file>`
Changes the contents of a specified file to match the specified commit.

<!--Get to this later
`git revert <commit_sha>
`Git revert functions as an undo command. Git revert undos the changes made in a specific commit without deleting the project history.


git reset --hard HEAD~1

git reset --hard <commit_sha>

git merge --abort
--->
