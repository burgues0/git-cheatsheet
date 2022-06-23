# Git/GitHub Cheatsheet

## Create

New _local_ repository

`$ git init`


> New local repository in a specific directory

`$ git init <directory>`

> Clone an existing repository to local machine

|HTTPS          |SSH            |
|:-------------:|:-------------:|
|`$ git clone https://github.com/user/repo.git`| `$ git clone ssh://user@domain.com/repo.git` |


## Local Changes

> Changed files in your working directory

`$ git status`


> Changes to tracked files

`$ git diff`


> Add all current changes to the next commit

`$ git add .`


> Add some changes in <file> to the next commit

`$ git add -p <file>`


> Commit all local changes in tracked files

`$ git commit -a`


> Commit previously staged changes

`$ git add -p <file>`


> Add some changes in to the next commit

`$ git commit`


> Change the last commit

`$ git commit --amend`


## Branching and Tags

## Update and Publish

## Merge and Rebase

## Undo
