# SUBMODULES
## SETUP

### IMPORTANT

Update the submodule first and then commit the change in the main repository.  This will make sure that the HEAD of the main repository is pointing to the correct submodule HEAD

### Adding a submodule

If you want to add the submodule to a specific directory like plugins 

```text
$ cd plugins/
```

```text
$ git submodule add -b https://github.com/petervmercer/submodule

```
Using the -b argument means we want to follow the master branch of the submodule repository, and after running this command we'll have an empty submodule directory.

### Removing a submodule - that you added and want to remove from core

1. Delete the relevant line from the .gitmodules file.
2. Delete the relevant section from .git/config.
3. Add the changes - git add .
4. Run git rm –cached path_to_submodule # Note: a/submodule (no trailing slash).
5. Commit
6. delete the now untracked submodule files.
