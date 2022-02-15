## Version control histories
Display the logs. To switch between screens, use space to move forward,
b to move backward, and q to quit.

```
git log 
```

Display the logs in a pretty way.  
Or use git reflog to see all the logs(past and future) with indexes.
```
git log --pretty=oneline
git log --oneline
git reflog
```

Go to a version
```
git reset --hard 42e7e84
```

Only change the header in the version history
```
git reset --soft 42e7e84
```

Only change the header in the version history and temp storage
```
git reset --mixed 42e7e84
```

## Check the difference between 2 files
Use git diff: the difference between the file and the "stage". If no file in the stage, then compare with the HEAD in the repository.
```
git diff
```

Use the following to compare between any version in the repository.
```
git diff HEAD apple.txt
```

## Branches
Check all branches
```
git branch
git branch -v
```

Create new branch
```
git branch hot_fix
```

Switch to a branch
```
git checkout hot_fix
```

Merge a branch (You need to be on the branch to be merged)
```
git merge hot_fix
```


