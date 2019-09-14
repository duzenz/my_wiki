# Git commands


## CREATE
```bash
#Clone an existing repository
git clone ssh://user@domain.com/repo.git
#Create a new local repository
git init
```

##  Create patch and apply

```bash
git format-patch -1 <commit_sha> # create patch
git apply --stat file.patch # check applicability of patch
git am --signoff < file.patch # apply patch
```
