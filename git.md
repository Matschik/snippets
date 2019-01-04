# Git snippets

## Get some files from a stash

```
# Copy all modifications from stash to WIP
$ git stash apply

# Remove added files
$ git rm -f newFileFromStash.md

# Remove modified files
$ git checkout fileModified.md

# Now you can check your files in WIP
$ git status
```
