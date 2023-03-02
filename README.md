
Personal library aliases for git defined

##  👀 View current aliases

```
git config --global -l
```

</br>
</br>

## 📚 Alias Library:


- `git current`: Query the name of the current branch
- `git last`: Query info of the last commit
- `git undo`: Rollback last changes
- `git done`: Push to non-remoted branch
- `git history`: Display all branches like graph

</br>
</br>

##  ⚙️  Bulk installation:

First step, open editor:
```
git config --global -e
```
Second step, paste next lines:
```
[alias]
	current = rev-parse --abbrev-ref HEAD
	last = log -1 HEAD --stat
	undo = reset HEAD~1 --mixed
	done = !git push origin HEAD
	history = log --all --graph --decorate --oneline --simplify-by-decoration
```


</br>
</br>

##  ⚒️  Cherry-pick Installation:

#### Query the name of the current branch  

```
git config --global alias.current 'rev-parse --abbrev-ref HEAD'
```


#### Query info of the last commit

```
git config --global alias.last 'log -1 HEAD --stat'
```


####  Rollback last changes

```
git config --global alias.undo 'reset HEAD~1 --mixed'
```

####  Push to non-remoted branch

```
git config --global alias.done '!git push origin HEAD'
```

####  Display all branches like graph

```
git config --global alias.history 'log --all --graph --decorate --oneline --simplify-by-decoration'
```


