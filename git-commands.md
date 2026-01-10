# Git & GitHub Commands – Complete List

This document contains all important Git and GitHub commands
from beginner to intermediate level, learned step by step.

---

## 1. Git Installation & Setup

Check Git version:
git --version

Set username and email:
git config --global user.name "Your Name"
git config --global user.email "youremail@gmail.com"

Check configuration:
git config --list

Purpose:
- Used to identify the author of commits

---

## 2. Initialize Repository

git init

Purpose:
- Creates a new Git repository in the project folder

---

## 3. Repository Status

git status

Purpose:
- Shows current branch
- Shows staged, unstaged, and untracked files

---

## 4. Staging Files

Stage single file:
git add file.txt

Stage all files:
git add .

Purpose:
- Moves changes to staging area

---

## 5. Commit Changes

git commit -m "commit message"

Purpose:
- Saves changes permanently in Git history

---

## 6. Commit History

git log
git log --oneline
git log --graph

Purpose:
- View project history
- Understand commits and branches

---

## 7. Branching

List branches:
git branch

Create branch:
git branch feature1

Switch branch:
git checkout feature1
git switch feature1

Create and switch:
git checkout -b feature1
git switch -c feature1

Purpose:
- Work on features separately without affecting main branch

---

## 8. Delete Branch

git branch -d feature1

Purpose:
- Remove unused branches safely

---

## 9. Merge Branch

git merge feature1

Purpose:
- Merge feature branch into current branch (usually main)

Important:
- Always pull latest code before merge

---

## 10. Rebase (Basic Idea)

git rebase main

Purpose:
- Keeps commit history clean and linear

---

## 11. Git Diff

git diff
git diff --staged

Purpose:
- See changes before committing

---

## 12. Git Stash

Save work temporarily:
git stash

List stashes:
git stash list

Apply stash:
git stash apply

Apply & remove stash:
git stash pop

Purpose:
- Temporarily save unfinished work without committing

---

## 13. Time Travel (Old Commits)

Go to old commit:
git checkout commit-id

Create branch from old commit:
git checkout -b lite-version

Purpose:
- Modify old code safely in a new branch

---

## 14. Remote Repository (GitHub)

Add remote:
git remote add origin repository-url

Check remote:
git remote -v

Purpose:
- Connect local repository to GitHub

---

## 15. Push & Pull

Push code:
git push origin main
git push origin branch-name

Pull code:
git pull origin main

Purpose:
- Sync local and remote repositories

---

## 16. Clone Repository

git clone repository-url

Purpose:
- Download repository from GitHub

---

## 17. Fork (GitHub Theory)

Steps:
- Fork repository on GitHub
- Clone forked repo
- Make changes
- Push changes

Purpose:
- Work on someone else’s project independently

---

## 18. Pull Request (PR)

Steps:
- Fork repository
- Make changes in fork
- Push changes
- Create Pull Request
- Owner reviews and merges

Purpose:
- Contribute to original repository

---

## ✅ End of Git Commands
