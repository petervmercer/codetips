# Git Working with remote repositories

## GitHub

### Different git Push & Pull(fetch) URLs

Start with standard set up

```text
git remote -v
returns > 
origin  https://github.com/petervmercer/codetips.git (fetch)
origin  https://github.com/petervmercer/codetips.git (push)

// Change to Master
git remote set-url origin https://github.com/petervmercer/mastertips.git

// Weird change - to set push
git remote set-url --push origin https://github.com/petervmercer/codetips.git

git remote -v
returns > 
origin  https://github.com/petervmercer/mastertips.git (fetch)
origin  https://github.com/petervmercer/codetips.git (push)
```

Another way edit .git/config and add 

```text
...
PRE CHANGE
[remote "origin"]
        url = https://github.com/petervmercer/codetips.git
        fetch = +refs/heads/*:refs/remotes/origin/*

POST CHANGE
...
[remote "origin"]
    fetch = +refs/heads/*:refs/remotes/origin/*
    url = https://github.com/petervmercer/mastertips.git
    pushurl = https://github.com/petervmercer/codetips.git
...
```


