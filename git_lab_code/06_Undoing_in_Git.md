# Undoing in Git
- You can undo mistakes on git to restore your workflow.

## Undo before staging
```
git checkout main
git pull

echo "Original line" > undo.txt
git add undo.txt
git commit -m "Test commit"

echo "bad change" > undo.txt
cat undo.txt
git restore undo.txt
cat undo.txt
git push
```

## Undo after staging
```
echo "Another bad line" > undo.txt
git add undo.txt
git status

git restore --staged undo.txt
git status

git add undo.txt
git commit -m "Move to main"
git push
```

## Undo a Commit
```
echo "Commit error" > undo.txt
git add undo.txt
git commit -m "Wrong commit"

git reset --mixed HEAD~1
```

## Undo from main branch safely

echo "main branch mistake" > undo.txt
git add undo.txt
git commit -m "main branch mistake"
git push

git revert HEAD   #Creates a new commit that undoes the last one
git status
git push









