# Branch Deneme

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
```
