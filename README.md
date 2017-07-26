# Hello this is the example github repo

This readme is written in markdown.
Content in <this tag> is variable.

## Getting Started with Git
### Configure Identify
$ git config --global user.name <"John Doe">
$ git config --global user.email <johndoe@example.com>

The name and email address you configure here is used with any commits you make.

### Git clone
The `git clone` command copies an existing Git repo into a local directory.
`git clone <repoURL>` for example, `git clone https://github.com/mattswhelan/examplerepo`

### Git pull
The `git pull` command updates your local directory with any changes to the repo, then attempts to merge those changes with your work.

## What Has Changed/What is Happening/Help
### Git status
The `git status` command displays the state of any changes in your working directory. These states are:
* Changes made locally that are not staged
* Changes made locally that are staged
* Changes made locally that are committed

The `git status` command is useful to run if you are confused.

### Git log

### Git add
The `git add` command locally stages and tracks changes made to the specified file(s). These changes could be edits to a file, a file getting deleted, or a file being added to a project. Use `git add` to prepare content for a `commit`. Anything that changed in your working directory can added.

`git add <filename.extension>`
Stages and tracks the changes made to the specified file.

`git add <filename.extension1> <filename.extension2> <filename.extension1>`
Stages and tracks the changes made to all of the specified files.

`git add .`
Stages and tracks all changes made.

>This command will only add content in the current working directory and any subdirectories below it. If you wish to add _all_ local changes, navigate to your root project directory before using `git add .`. Or you could just right click the root project directory and select git bash on windows. That also works.

## Branches
##

## Fixing mistakes

git reset --hard HEAD~1

git reset --hard <commit_sha>

git merge --abort
Reverts a mer

## Workflow
1. Edit files in a repo locally.
2. `git status` to view changes.
3. `git add` to select changes to stage.
4. `git commit` to
