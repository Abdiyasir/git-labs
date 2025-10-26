# Git Stash (Temporary saving)
- When in the middle of a task Git Stash can be used to temporary save and switch branches if something else needs to be addressed immediately.
```
echo "incomplete work" > feature.txt
git add feature.txt

echo "More changes not staged" > feature.txt
git stash push -m "WIP :feature.txt changes"

echo "hotfix applied" > hotfix.txt
git add hotfix.txt
git commit -m "apply hotfix on main"
git push origin main

git stash list
git stash apply  #Re-applies stashed changes to working directory
git stash pop    #Re-applies stashed changes and deletes that stash entry
git commit -m "push feature changes"
git push
```
