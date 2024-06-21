# Git Cheat Sheet

These are some useful commands.

## Starting Project
1) `git init` - Create a new local Git repository.
2) `git clone [repo]` - Clone a project from a remote repository.

## Day to Day
1) `git status` - Show the status of the repo.
2) `git add [fileName]` - Add a file to the staging area.
3) `git diff [fileName]` - Show changes made to the file.
4) `git checkout -- [fileName]` - Discard changes in the working directory for the specified file.
5) `git commit -m "[message]"` - Commit the staged files with a message.
6) `git rm [fileName]` - Remove a file from the working directory and staging area.

## Inspect History
1) `git log` - List all the commit history for the current branch.
2) `git reflog` - List all the operations (commits, checkouts, etc.) done in the local repository.

## Tagging
Tagging is mostly used for versions and releases.
1) `git tag` - List all the tags.
2) `git tag [name] [commit sha]` - Create a new tag with the provided name and commit id.
3) `git tag -d [name]` - Delete a tag.

## Storing Work
1) `git stash` - Put current changes in your working directory into stash for later use.
2) `git stash pop` - Apply and remove the stored stash.
3) `git stash drop [stash]` - Delete a specific stash (if not specified, deletes the latest one).

## Git Branching
1) `git branch -a` - List all the branches in the repository, including remote branches.
2) `git branch [name]` - Create a new branch with the provided name.
3) `git rebase [branch name]` - Reapply commits of the current branch on top of the specified branch.
4) `git checkout [branch name]` - Switch to the specified branch.
5) `git merge [branch name]` - Merge the specified branch into the current branch.
6) `git branch -d [branch name]` - Delete a local branch with the provided name.

## Remote Git
1) `git fetch` - Fetch changes from remote to local without merging.
2) `git pull` - Fetch changes from remote and merge them into the current branch.
3) `git push` - Push local commits to the remote repository.

## .gitignore
Files and directories listed in this file will be ignored by Git.
- This is mainly used to ignore large unnecessary files, to avoid storing secrets in the remote repository, etc.

