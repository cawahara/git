# Try Git


## Scinario 2: 2 different branch from same master

1. Working in `current` branch. (updating file_a)
2. in `another` branch, file_a has been update and merge to `master`
3. Want to continue working in `current` after merge latest `master`

### Steps
```
2-1
$ git checkout -b current
# update file_a
$ git cm -a -m "Update file A in current branch"
2-2
$ git checkout -b another
# update file_a
$ git add file_a
$ git cm -m "Update file A in another branch"
```

## Scinario 1: 2 different branch from same master

When you want to develop function A and function B separately, you need 2 different branch from same master.
After creating branch for A, how to create branch B with original status.

### Steps

What you need to do is just checkout master and create second branch.

```
$ git branch branch_2_1
$ git checkout branch_2_1
# add file for function A
$ git add .
$ git commit -m "Add function A"
$ git checkout master
$ git branch branch_2_2
```
