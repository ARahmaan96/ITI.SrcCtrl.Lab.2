# ITI.SrcCtrl.Lab.2"

## commands:

`mkdir ITI.SrcCtrl.Lab.2`

`cd ITI.SrcCtrl.Lab.2`

---

`git init`

`git add *`

`git commit -m "init commit."`

`git branch -M main`

`git remote add origin https://github.com/ARahmaan96/ITI.SrcCtrl.Lab.2.git`

`git push -u origin main`

## Create two branches (dev & test) and create one file on each branch:

```bash
git checkout -b dev
echo "# Development Branch" > dev_log.md
echo "## author: A.Rahman Khallaf" >> dev_log.md
echo "## Created at: 4/18/2024" >> dev_log.md
git add dev_file.md
git commit -m "Added dev file"

git checkout -b test
echo "# Test Branch" > test_log.md
git add test_file.md
git commit -m "Added test file"
```

## Push these branches to the remote repository:

```bash
git push origin dev
git push origin test
```

## Merge these changes on the Main branch locally:

```bash
git checkout main
git merge dev
git merge test
```

## Push changes to your remote main branch:

```bash
git push origin main
```

## Create an annotated tag with tagname (v1.7):

```bash
git tag -a v1.7 -m "Version 1.7"
```

## Push the tag to the remote repository:

```bash
git push origin v1.7
```
