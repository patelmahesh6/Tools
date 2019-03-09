
## Configure user information for all local repositories

```$ git config --global user.name "[name]"``` 
 Sets the name you want atached to your commit transactions

``` $ git config --global user.email "[email address]"``` 
 Sets the email you want atached to your commit transactions

``` $ git config --global color.ui auto ``` 
 Enables helpful colorization of command line output
 
 
## CREATE REPOSITORIES

```$ git init [project-name] ```
Creates a new local repository with the specified name

```$ git clone [url] ```
Downloads a project and its entire version history

## MAKE CHANGES

```$ git status```
Lists all new or modified files to be commited

```$ git add [file]```
Snapshots the file in preparation for versioning

```$ git reset [file]```
Unstages the file, but preserve its contents

```$ git diff```
Shows file differences not yet staged

```$ git diff --staged```
Shows file differences between staging and the last file version

```$ git commit -m "[descriptive message]"```
Records file snapshots permanently in version history

## GROUP CHANGES

```$ git branch```
Lists all local branches in the current repository

```$ git branch [branch-name]```
Creates a new branch

```$ git checkout [branch-name]```
Switches to the specified branch and updates the working directory

```$ git merge [branch]```
Combines the specified branch’s history into the current branch

```$ git branch -d [branch-name]```
Deletes the specified branch

## SYNCHRONIZE CHANGES

```$ git fetch [bookmark]```
Downloads all history from the repository bookmark

```$ git merge [bookmark]/[branch]```
Combines bookmark’s branch into current local branch

```$ git push [alias] [branch]```
Uploads all local branch commits to Git

```$ git pull```
Downloads bookmark history and incorporates changes


## SAVE FRAGMENTS

```$ git stash```
Temporarily stores all modified tracked files

```$ git stash list```
Lists all stashed changesets

```$ git stash pop```
Restores the most recently stashed files

```$ git stash drop```
Discards the most recently stashed changeset

## REDO COMMITS

```$ git reset [commit]```
Undoes all commits afer [commit], preserving changes locally

```$ git reset --hard [commit]```
Discards all history and changes back to the specified commit


```$ git log```
Lists version history for the current branch
