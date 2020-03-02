# Some useful techniques for using git

## How to update the fork repo
It's super important to update the fork repo with the new commits of the 'upstream' repo.

### Set remote repo for the fork repo

#### Check status
``` 
git remote -v 
```

#### Add upstream repo
``` 
git remote add upstream
https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
```
After this has been set, check the status again.

### Synchronize fork
#### Fetch branchs and commits from upstream repo, commit to local master branch and this would be stored in the branch upstream/master
```
git fetch upstream
```
#### Checkout to local master
```
git checkout master
```
#### Merge upstream/master to local master, then synchronize is completed and local mudify on master wouldn't disappear
```
git merge upstream/master master
```
#### Update on remote repo
```
git push origin master
```
#### Done
