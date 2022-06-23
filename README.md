# Git/GitHub Cheatsheet

## **Create** 

|Functionality|Command|
|:-----------|:-----|
|New local repository|`$ git init`|
|New local repository in specific directory|`$ git init <directory>`|
|Clone an existing repository to local machine (HTTPS)|`$ git clone https://github.com/user/repo.git`|
|Clone an existing repository to local machine (SSH)|`$ git clone ssh://user@domain.com/repo.git`|

## **Local Changes**

|Functionality|Command|
|:-----------|:-----|
|Changed files in your working directory|`$ git status`|
|Changes to tracked files|`$ git diff`|
|Add all current changes to the next commit|`$ git add .`|
|Add some changes in <file> to the next commit|`$ git add -p <file>`|
|Commit all local changes in tracked files|`$ git commit -a`|
|Commit previously staged changes|`$ git add -p <file>`|
|Add some changes in to the next commit|`$ git commit`|
|Change the last commit|`$ git commit --amend`|

> OBS.: Don't ammend published commits.

## **Branching and Tags**

|Functionality|Command|
|:-----------|:-----|
|List all existing branches|`$ git branch`|
|Switch HEAD branch|`$ git checkout <branch>`|
|Create a new branch based on your current HEAD|`$ git branch <new-branch>`|
|Create a new tracking branch based on a remote branch|`$ git checkout --track <remote/branch>`|
|Delete a local branch|`$ git branch -d <branch>`|
|Mark the current commit with a tag|`$ git tag <tag-name>`|

## **Merge and Rebase**

|Functionality|Command|
|:-----------|:-----|
|Merge <branch> into your current HEAD|`$ git merge <branch>`|
|Rebase your current HEAD onto <branch>|`$ git rebase <branch>`|
|Abort a rebase|`$ git rebase --abort`|
|Continue a rebase after resolving conflicts|`$ git rebase --continue`|
|Use your configured merge tool to solve conflicts|`$ git mergetool`|
|Use your editor to manually solve conflicts|`$ git add <resolved-file>`|
|After resolving mark file as resolved|`$ git rm <resolved-file>`|

> OBS.: Don‘t rebase published commits.

## **Undo**

|Functionality|Command|
|:-----------|:-----|
|Discard all local changes in your working directory|`$ git reset --hard HEAD`|
|Discard local changes in a specific file|`$ git checkout <file>`|
|Revert a commit (by producing a new commit with contrary changes)|`$ git revert <commit>`|
|Reset your HEAD pointer to a previous commit & discard all changes since then|`$ git reset --hard <commit>`|
|Reset your HEAD pointer to a previous commit & preserve all changes as unstaged changes|`$ git reset <commit>`|
|Reset your HEAD pointer to a previous commit & preserve uncommitted local changes|`$ git reset --keep <commit>`|

## **Update and Publish**

|Functionality|Command|
|:-----------|:-----|
|List all currently configured remotes|`$ git remote -v`|
|Show information about a remote|`$ git remote show <remote>`|
|Add new remote repository, named <remote>|`$ git remote add <remote> <url>`|
|Download all changes from <remote>, but don‘t integrate into HEAD|`$ git fetch <remote>`|
|Download changes and directly merge/integrate into HEAD|`$ git pull <remote> <branch>`|
|Publish local changes on a remote|`$ git push <remote> <branch>`|
|Delete a branch on the remote|`$ git branch -dr <remote/branch>`|
|Publish your tags|`$ git push --tags`|
