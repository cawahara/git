Git
---
Basic
```
$ git status                 # show status of branch
$ git config --list          # show config of git
$ git log                    # show commit message, quit with ‘q’
$ git clone <url of repository>
$ git clone <repocitory> [path]
```

Branch
```
$ git branch -a              # show branch list
$ git branch <branchname>
$ git co <branchname>
```


Scinerio: 2 different branch from same master
---
When you want to develop function A and function B separately, you need 2 different branch from same master.
After creating branch for A, how to create branch B with original status.

# How to manage

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
