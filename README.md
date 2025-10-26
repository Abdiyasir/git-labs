<img width="840" height="726" alt="image" src="https://github.com/user-attachments/assets/f2021b83-1688-448a-962b-ac355d427605" /># Git for Devops

## What Is Git?
- Git is a version control system — a tool that tracks changes in your code and helps multiple people work on the same project safely.
- It’s not just for storing code — Git is the foundation of collaboration in software development. It lets teams build, test, ship, and recover code efficiently — even if something breaks.

## Git Labs — Practical Hands-On Exercises
- This repository includes a Git Labs folder containing practical exercises based on real-world developer and DevOps workflows.

### What They Cover:
- Initializing and setting up repositories
- Branching, merging, and resolving conflicts
- Rebasing and squashing commits
- Using stash, cherry-pick, and revert safely
- Configuring .gitignore and handling .env files securely
- Undoing mistakes
- Practicing clean commit messages and team-based collaboration

## Common Git Commands
| **Command** | **Description** |
|--------------|----------------|
| `git init` | Initialize a new Git repository. |
| `git clone <url>` | Clone a remote repository to your local machine. |
| `git config --global user.name "<NAME>"` | Set global username for commits. |
| `git config --global user.email "<EMAIL>"` | Set global email for commits. |
| `git status` | Display the current state of the repository (staged, unstaged, untracked files). |
| `git add <file>` | Stage file changes for the next commit. |
| `git commit -m "message"` | Save a snapshot of staged changes. |
| `git log` | Show commit history. |
| `git diff` | Display differences between file versions. |
| `git branch` | List all local branches. |
| `git branch <name>` | Create a new branch. |
| `git switch <name>` | Switch to another branch (modern command). |
| `git merge <name>` | Merge the specified branch into the current one. |
| `git branch -d <name>` | Delete a branch safely. |
| `git restore <file>` | Undo changes in a file. |
| `git reset --soft HEAD~1` | Undo the last commit but keep changes staged. |
| `git revert <commit>` | Create a new commit that safely undoes a previous one. |
| `git reflog` | Show the full movement history of HEAD (recover lost commits). |
| `git remote add origin <url>` | Link a local repository to a remote GitHub repository. |
| `git push origin main` | Upload local commits to the remote main branch. |
| `git pull origin main` | Fetch and merge updates from the remote main branch. |
| `git fetch` | Download remote changes without merging them. |
| `git rebase main` | Reapply commits from the current branch onto another base branch. |
| `git stash` | Temporarily save uncommitted changes for later use. |
| `git stash pop` | Reapply the most recent stash and remove it from the stash list. |
| `git cherry-pick <hash>` | Apply a specific commit from another branch. |
| `git commit --amend` | Modify the most recent commit (message or content). |
| `git log --oneline --graph --all` | View all branches and commits in a visual format. |
| `git rm --cached .env` | Stop tracking sensitive files already added to Git. |
| `echo ".env" >> .gitignore` | Add `.env` to `.gitignore` to prevent future tracking. |
