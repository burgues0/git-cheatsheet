# Git/GitHub Cheatsheet

## Create

- New local repo


`$ git init`


- New local repo in directory

```txt
$ git init <directory>
```

- Clone existing repo

- HTTPS

```txt
$ git clone https://github.com/user/repo.git
```

- SSH

```txt
$ git clone ssh://user@domain.com/repo.git
```

## Local Changes

### Changed files in your working directory

```txt
$ git status
```

### Changes to tracked files

```txt
$ git diff
```

### Add all current changes to the next commit

```txt
$ git add .
```

### Add some changes in <file> to the next commit

```txt
$ git add -p <file>
```

### Commit all local changes in tracked files

```txt
$ git commit -a
```

### Commit previously staged changes

```txt
$ git add -p <file>
```

### Add some changes in to the next commit

```txt
$ git commit
```

### Change the last commit

```txt
$ git commit --amend
```

Don‘t amend published commits!
## Branching and Tags

## Update and Publish

## Merge and Rebase

## Undo
