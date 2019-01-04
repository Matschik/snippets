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
