# Git Config tips

## Location of configuration files

### System wide configuration

Generally not used - user based config is most common

*Linux*

```text
/etc/gitconfig
```

*Windows*

```text
Program Files/Git/etc/gitconfig
```


### logged in user based configuration

*Linux*

in Home directory

```text
 HOME\.gitconfig
```

*Windows*

```text
cd users/petervmercer/

ls -la

> -rw-r--r-- 1 Peter 197609       99 Nov  6 18:03 .gitconfig

```


### Local project configuration

In .git

```text
myProject/.git/config
```

## Configuration

*System*

```text
$ git config --system
```

*User*

```text
git config --global
```

*Local project*

```text
$ git config
```

## Changing configuration

### Add user name and email
```text
$ git config --global user.name "Peter Mercer"

$ git config --global user.email "myemail@test.com"
```

### Show config

```text
$ git config --list

> user.name=Peter Mercer
> user.email=myemail@test.com

$ git config user.name
> user.name=Peter Mercer


$ cat .gitconfig
[user]
        name = Peter Mercer
        email = peter@vizipix.com
[color]
        ui = true
[core]
        editor = notepad


```


### Edit config file

```text
$ git config --global core.editor "vim"   // notepad++.exe, wordpad, Vim, mate

$ git config --global color.ui true //outputs coloured config text

$ git config --global --edit

```
