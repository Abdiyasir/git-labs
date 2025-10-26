# Branching & Merging
- Branching allows you to work in different features without changing the main code.
- Once the changes are ready Merging allows you to bring the changes over to the main branch.
- Merge conflicts can occur when the same file is changed differently in both the new feature branch and main branch.

### Making a change to the Main branch & adding a feature branch
```
echo "Hello from main" > app.txt
git add app.txt
git commit -m "Initial commit on main"

git checkout -b feature-1
echo "Feature branch change" > app.txt
git add app.txt
git commit -m "update from feature-1"

git checkout main
echo "Main branch change" > app.txt
git add app.txt
git commit -m "Conflicting update from main"
git merge feature-1   #This creates a conflict as there's different changes on the same file

cat app.txt
echo -e "Hello from main\nMain branch change\nFeature branch change" > app.txt #This overrides the merge conflict and keeps all changes

git add app.txt
git commit -m "resolve merge conflict between main and feature-1 branch"
git branch
git branch -d feature-1
```
