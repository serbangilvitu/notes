## add
Update the index by adding all files in the working directory (`-n` for dry-run)
```
git add -A
```
## branch
Show all branches
```
git branch -a
```
Show remote branches
```
git branch -r
```
## checkout
Create a new branch
```
git checkout -b <branch>
```
Switch to an existing branch
```
git checkout <branch>
```
Revert uncommited changes to a file
```
git checkout HEAD -- <path>
```

## cleanup
Remove untracked files from the working tree (`-n` for dry-run)
```
git clean -df
```

## diff
View the changes you staged for the next commit
```
git diff --cached
```
Diff between local and remote branch
```
git diff <branch>..origin/<branch>
```
## fetch
Download objects and refs from a remote and remove any remote-tracking references that no longer exist on the remote.
```
git fetch -p
```
## merge
Create a single commit instead of doing a merge
```
git merge --squash <branch>
```
## push
Use `-n` for dry-run
```
git push -u origin <branch>
```
Delete a remote branch
```
git push -d origin <branch>
```
Push tags
```
git push --tags
```
## reset
Resets the index but not the working tree (i.e., the changed files are preserved but not marked for commit)
```
git reset --mixed
```
Resets the index and working tree
```
git reset --hard
```
Discard latest commit
```
git reset --hard HEAD^
```
## stash 
Save your local modifications to a new stash entry and roll them back to HEAD
```
git stash
```
Apply changes and remove the latest stash entry
```
git stash pop
```
## status 
List of modified files (using `-vv` will also list contents)
```
git status -v
```

## tag
Tag current commit
```
git tag -a -m <message> <tag>
```
Delete a tag
```
git tag -d <tag>
```
