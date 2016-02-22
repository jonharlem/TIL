# Clone all remote branches

When you clone a Git repo, `$ cd` into it, and look at the local branches (`$ git branch`), you won't see all of the other branches on the project. To see the other branches on the Git repo, you have to use the `-a` flag.

First you will want to fetch all the branches:

```
$ git fetch -a
```

Then you will want to see all branches:

```
$ git branch -a
```

To switch to a branch:

```
$ git checkout branchName
```
