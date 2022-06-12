# git-commands

# Git Configuration

## Git Global Setup
`Git` uses a hierarchical config approach in which settings of a broader scope are inherited if not overriden.

`Global configurations` are available for the current users for all the projects and stored in

```shell
$ ~/.gitconfig or ~/.config/git/config
```

```shell
$ git config --global user.name "MyKloudJourney"
$ git config --global user.email "mykloudjourney@gmail.com"
```


## Git Local Setup
`Local configs` are available for the current repository only. We can make `git` read and write from Local by passing `--local` option.

```shell
$ git config --local user.name "MyKloudJourney"
$ git config --local user.email "mykloudjourney@gmail.com"
```

## Git Local Setup
```shell
$ git config --list --show-origin
```

# Clone Remote Repository
```shell
$ git clone <git-url>
$ cd <cloned-repo-name>
$ git switch -c main
$ touch README.md
$ git add README.md
$ git commit -m "add README"
$ git push -u origin main
```

# Push to an existing folder
```shell
cd <repo-name>
git init --initial-branch=main
git remote add origin <repo-url>
git add .
git commit -m "Initial commit"
git push -u origin main
```

# Push an existing Git repository
```shell
cd <repo-name>
git remote rename origin old-origin
git remote add origin <repo-url>
git push -u origin --all
git push -u origin --tags
```
