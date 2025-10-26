# Git amend
- This allows you edit your most recent commit, either the message, contents or both.

```
echo "line 1" > notes.txt
git add notes.txt
git commit -m "feat: add note file"

echo "metadata" > meta.txt
git add meta.txt

git commit --amend   #Update the commit or include changes
git log --oneline    #Verify the update has gone through
git push
```
