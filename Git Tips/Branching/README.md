# Branching Tips

## General notes

Branch only gets a new head SHA after commiting changes in the branch

### Example to see heads ref

```text
$ git init

// CREATE A FILE and commit

$ git branch new_branch
$ git checkout new_branch
$ $ ls -la .git/refs/heads
> total 2
> drwxr-xr-x 1 Peter 197609  0 Nov 12 17:38 ./
> drwxr-xr-x 1 Peter 197609  0 Nov 12 17:35 ../
> -rw-r--r-- 1 Peter 197609 41 Nov 12 17:37 master
> -rw-r--r-- 1 Peter 197609 41 Nov 12 17:38 new_branch

$ cat .git/refs/heads/master
> e222972e125377368208badd19f958a9d1080778

$ cat .git/refs/heads/new_branch
> e222972e125377368208badd19f958a9d1080778
```

Note the HEAD is the same.

Now change a file in the branch

```text
// After commkit check the refs
$ cat .git/refs/heads/new_branch
> 4d5bfabc0bffe8938e1377c2714e158d16ecff7d

```

### Show Commit

```text
git show HEAD

// OR

git show efghij93 //SHA value for HEAD

```

## Looking at available branches 

```text
$ git branch
``` 

## Adding a branch

no spaces or symbols allowed

```text
$ git branch new_branch
```

### Fast way to add and switch to a branch

```text
$ git checkout -b new_checkout_b_branch
> Switched to a new branch 'new_checkout_b_branch'

// Make a change and commit

// Send to remote
git push -u origin new_checkout_b_branch

```

### Switching to a branch

```text
$ git checkout branch_name
```


## Which HEAD id git pointing to?

```text
$ cat .git/HEAD
```

## Difference between Branches

Use spread operator [..]

```text
$ git diff master..new_branch

//Use color words on one line

$ git diff --color-words master..new_branch
```

## What branches code is included in your branch

Useful to know where the branch was derived from.
```text
$ git branch --merged
```

## Renaming branches

```text
$ git branch -m old_branch new_branch
```

## Deleting a branch

Can not delete branch you are on.  You will get a warning of there are chnges that have not been merged.
```text
$ git branch -d old_branch
```
