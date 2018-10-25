# Git Working with remote repositories

## GitHub

### Adding a remote repository

```text
cd <Directory>
Example cd test_site

git remote add <alias> <url>
Example git remote add origin https://github.com/petervmercer/codetips.git

// Find your remote

git remote
returns > origin

// More information

git remote -v
returns > 
origin  https://github.com/petervmercer/codetips.git (fetch)
origin  https://github.com/petervmercer/codetips.git (push)

// Looking at the config

cat .git/config
returns >
[core]
        repositoryformatversion = 0
        filemode = false
        bare = false
        logallrefupdates = true
        symlinks = false
        ignorecase = true
[remote "origin"]
        url = https://github.com/petervmercer/codetips.git
        fetch = +refs/heads/*:refs/remotes/origin/*
[branch "master"]
        remote = origin
        merge = refs/heads/master



```
