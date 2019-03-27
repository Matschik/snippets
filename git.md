# Git snippets

## Useful aliases

```sh
$ vi ~/.gitconfig
```

```
# .gitconfig

[alias]
  # pretty logs
  lg = log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --branches
```

## Clean commits in a branch
To clean up commits (squash, edit commit,  remove commit), use the start point (hash from the oldest commit) to edit newer commits.
```sh
$ git rebase -i 9a7f06b
```

## Add file modifications to last commit
```sh
$ git add my-forgotten-file.md
$ git commit --amend
```

## Split last commit into many commits
```sh
$ git reset HEAD~

$ git add first-commit.md
$ git commit -m "First commit"

$ git add second-commit.md
$ git commit -m "Second commit"
```

## Store locally WIP changes
```sh
$ git stash # store all changes in the current branch
$ git stash list # show all stashes stored
$ git stash pop # unwrap all stashes
$ git stash apply # apply all stashes without removing stashes
```
