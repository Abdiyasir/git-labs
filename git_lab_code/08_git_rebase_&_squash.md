# Git Rebase & Squash

- Git rebase & git squash work together to combine multiple small commits into one, so you would have one clear commit representing your whole feature.

```
git checkout -b feature-rebase
echo "line 1" > changes.txt
git add changes.txt
git commit -m "feat: add first line"

echo "line 2" >> changes.txt
git add changes.txt
git commit -m "feat: add second line"

echo "line 3" >> changes.txt
git add changes.txt
git commit -m "feat: add third line"

git log --oneline      #shows recent logs as 3 different commits
git rebase -i HEAD~3   #change last two commits from pick to squash to change this to one commit
git push
```










