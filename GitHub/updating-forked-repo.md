# Updating a Forked Repo

In order to get the latest updates from a repo after forking it, add the original repo as a remote:

```
$ git remote add upstream https://github.com/username/original-repo.git
```

Fetch all of the branches of the original repo:

```
git fetch upstream
```

To rewrite any commits on top of the master branch:

```
git rebase upstream/master
```