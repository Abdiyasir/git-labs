# Git Ignore
- This tells Git which files or folders to ignore when tracking changes. 
- Useful for protecting sensitive info in order to avoid getting hacked.

```
touch .env
vi .env   #Open .env and add passwords
```

```
git pull
git add .gitignore
git commit -m "don't track env files"
git push
```
