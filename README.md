# Git Commands Cheatsheet

## 1. Navigate to your Git project folder

use `cd` to move between folders, for example 

```
cd workspce
cd bdl02 haidar_git_cheatsheet
```

## 2. check the status of the project

I can use these commands **anytime** to inspect my project.

- `git status` to see changes added to the file, and if some files are ready to be committed. 
It gives me an overview of the project at that specific moment of time.

  Messages given by `git status`:
    - > working tree clean

This means that no change has happened in our project since our last `git commit`

    - > nothing to commit
    
This means that no `git add .` has happened yet, so there is no change to commit

    - > changes to be committed

This means that we have staged some changes with `git add .`, and we now need to commit 

    - > changes not staged for commit

This means that we need to use `git add .` to prepare some changes to be committed.

- `git log` 

This command shows the commit logs.

- `git diff`

    Shows what changes have happened in our project since the last `git add .`.
    - Lines marked in **red** are lines that were removed.
    - Lines marked in **green** are lines that were added.
## 3. initializing a git project
if any `git` command that we run  gives the following output:
> fatal: not a git repository (or any of the parent directories): .git

it means **we are not inside a git project**. in such case we can:

1.  make sure that we are inside the right folder and navigate to it if needed.
2. initialize git

To initialize git run

```
git init
``` 

This command creates an empty Git repository.
from now on we can make changes to our files and permanently save those changes.

## 4. save changes to files

1. `git add .` or `git add -A`

`git add` tells Git that you want to include the latest changes in the next commit. However, changes are not actually recorded until you run `git commit`.

2. `git commit -m "reference to the changes"`
Commits can be thought of as snapshots or milestones along the timeline of a Git project.

You can also *quick commit* by running `git commit -am "reference message"`

3. `git push` this command sends the committed changes to the server. It is used to upload local repository content to a remote repository. 


New changes added to test

