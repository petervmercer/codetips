# STASH

## When to use?

You need to save your work and create a new branch to add the saved work to

Document is based on https://www.atlassian.com/git/tutorials/saving-changes/git-stash

### Process of saving

```shell script
$ git stash
```
### Process of re-applying your changes

#### POP

Popping your stash removes the changes from your stash and reapplies them to your working copy.

```shell script
$ git stash pop
```

#### Apply

Alternatively, you can reapply the changes to your working copy and keep them in your stash with git stash apply. This is useful if you want to apply the same stashed changes to multiple branches. 

```shell script
git stash apply
```

## Stashing untracked

Add -u option (or --include-untracked)

```shell script
$git stash -u
```

## Stashing ignored files

Add -a (or --all) 

