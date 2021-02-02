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
Ref: https://stackoverflow.com/questions/7244321/how-do-i-update-a-github-forked-repository
