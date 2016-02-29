# learning-git
These are notes into learning how to git.


# Git merge:

``` javascript
git checkout test
git pull origin master
git checkout master
git merge test
```


# Git rename branch:

Taken from [here](https://multiplestates.wordpress.com/2015/02/05/rename-a-local-and-remote-branch-in-git/).

1. Rename your local branch.
If you are on the branch you want to rename:

``` javascript
git branch -m new-name
```
If you are on a different branch:

``` javascript
git branch -m old-name new-name
```
2. Delete the old-name remote branch and push the new-name local branch.

``` javascript
git push origin :old-name new-name
```
3. Reset the upstream branch for the new-name local branch.
Switch to the branch and then:

``` javascript
git push origin -u new-name
```

# Git rebasing:

* http://gitready.com/intermediate/2009/01/31/intro-to-rebase.html
