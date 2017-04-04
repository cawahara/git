# Try Git


## Scinario 2: 2 different branch from same master

1. Working in `current` branch. (updating file_a)
2. in `another` branch, file_a has been update and merge to `master`
3. Want to continue working in `current` after merge latest `master`

## Scinario 1: 2 different branch from same master

When you want to develop function A and function B separately, you need 2 different branch from same master.
After creating branch for A, how to create branch B with original status.

### How to manage

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
