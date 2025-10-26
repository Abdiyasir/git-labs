# Git cherry-pick: Commit from one brach to another
- This allows you to copy a commmit from one branch and apply it to another.

```
git checkout -b feature-cherry
echo "hotfix config for prod" > hotfix.txt
git add hotfix.txt
git commit -m "hotfix: add config fix"
git push

git log --oneline     #copy the commit hash number e.g. c5fb550

git checkout main
git pull
git cherry-pick c5fb550
git push origin main
```
