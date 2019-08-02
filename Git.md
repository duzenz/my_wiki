# Docker commands

##  Create patch and apply

```bash
git format-patch -1 <commit_sha> # create patch

git apply --stat file.patch # check applicability of patch

git am --signoff < file.patch # apply patch

```
