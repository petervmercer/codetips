# Merge

## Check differences first

### Differences between two branches - all differences

```shell script
git diff master...branch_A
```

### Files changed only

```shell script
git diff --name-only master...branch_A
```

## Merge process

```shell script
$ git merge [branch] -m "Add message"
```