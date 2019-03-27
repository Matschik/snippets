# Git snippets

## Get some files from a stash

```sh
# Copy all modifications from stash to WIP without removing the stash
$ git stash apply

# Remove added files
$ git rm -f newFileFromStash.md

# Remove modifications from modified files
$ git checkout fileModified.md

# Now you can check your files in WIP
$ git status
```

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
