# New Repository
- This creates a new repository and adds a file to Github.
```
mkdir git-lab
cd git-lab
git init
touch README.md
echo "# Git Lab" > README.md
git add README.md
git commit -m "init commit"
git remote add origin https://github.com/<USERNAME>/git-labs.git
```
