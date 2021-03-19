# Totorial-of-basic-git-commands
Commonly used commands for managing a git repository.


## Clone
Clone the repo to your local folder.
```git
git clone <url>
```

## Check remote repo
```git
git remote -v
```

## Check status
Check the status of your local branch.
```git
git status
```

## Pull
Pull changes from remote repo.
```git
git pull
```

## Add
Updated changes of a file / add a file in your local branch.
```git
git add <file>
```
Update all changes in your local branch, including changes of files/directories and addition of files/directories.
```git
git add --all
```

## Commit
Commit all changes in your local branch with a message.
```git
git commit -am "<message>"
```

## Push
Push your changes to remote master.
```git
git push origin master
```

## Remove
Remove some files / directories from your local branch
```git
git rm <file>
```
```git
git rm -r <dir>
```

## Synchronize forked repo
Add the remote, call it "upstream":
```git
git remote add upstream https://github.com/whoever/whatever.git
```
Fetch all the branches of that remote into remote-tracking branches
```git
git fetch upstream
```
Make sure that you're on your master branch:
```git
git checkout master
```
Rewrite your master branch so that any commits of yours that
aren't already in upstream/master are replayed on top of that
other branch:
```git
git rebase upstream/master
```
Push / force push
```git
 git push -f origin master
```

Ref: https://stackoverflow.com/questions/7244321/how-do-i-update-a-github-forked-repository

## Cleanup a forked branch
```git
git remote add upstream /url/to/original/repo
git fetch upstream
git checkout master
git reset --hard upstream/master  
git push origin master --force 
```
Ref: https://stackoverflow.com/questions/9646167/clean-up-a-fork-and-restart-it-from-the-upstream

## Manipulating a branch
Clone only a branch
```git
git clone --single-branch --branch <branchname> <remote-repo>
```
Or clone the whole repo
```git
git clone <url>
```
List branches
```git
git branch -a 
```
Checkout the branch
```git
git checkout <branchname>
```

## Revert a commit
https://opensource.com/article/18/6/git-reset-revert-rebase-commands
