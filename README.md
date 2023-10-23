# Git Examples

## Branch

```BASH
# start git in this project
git init

# define origin of the project
git remote add origin git@github.com:OsmanKAYI/osmankayi.com.git

# create new branch called main
git branch -M main

# add all existing files and folders
git add .

# create the first commit as *site published*
git commit -m "first commit"

# push everything being in your local pc to github
git push -u origin main

# start a new $branchName
git checkout -b $branchName main

# edit some files
git add $file
git commit -m "Start a feature"

# edit some files
git add $file
git commit -m "Finish a feature"

# merge in the $branchName branch
git checkout main
git merge $branchName

# delete the merged branch
git branch -d $branchName

# previous command will delete a local copy of a branch. The branch may still exist in remote repos. To delete a remote branch execute the following
git push origin --delete $branchName
```

---

## Stash

```BASH
# stash your changes
git stash save "Your stash message"

# switch branches **_optional_**
# Using git stash in combination with branches can be a powerful way to manage your changes.
git checkout <branch-name>
# or
git switch <branch-name>

# apply the stash
git stash apply
```

### Managing Multiple Stashes

```BASH
# list all stashes
git stash list

# apply a Specific Stash
git stash apply stash@{n}

#delete a Stash
git stash drop stash@{n}
#This will remove the specified stash. Be careful, this action cannot be undone.
```
