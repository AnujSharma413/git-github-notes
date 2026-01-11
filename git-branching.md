# Git Branching & Merging – Complete Guide

This document explains how Git branches work,
why we use them, and how merging happens in real projects.

---

## 1. What is a Branch?

A branch is a separate line of development.

- `main` → stable production-ready code
- `feature` branches → new features or experiments

Purpose:
- Work independently
- Avoid breaking main code
- Easy collaboration

---

## 2. Default Branch (main / master)

Older Git versions used:
`master`

Now commonly used:
`main`

Rename master to main:
`git branch -m master main`

Set default branch:
`git config --global init.defaultBranch main`

---

## 3. View Branches

List local branches:
`git branch`

List remote branches:
`git branch -r`

List all branches:
`git branch -a`

Current branch is marked with `*`

---

## 4. Create a Branch

Create branch:
`git branch feature1`

Create & switch:
`git checkout -b feature1`or
`git switch -c feature1`

Purpose:
- Start working on a new feature

---

## 5. Switch Between Branches

Old command:
`git checkout branch-name`

New command:
`git switch branch-name`

Switch to previous branch:
`git switch -`

---

## 6. Why Files Are Not Visible in Other Branches?

Each branch has:
- Its own commits
- Its own file state

If a file is:
- Not committed → it may not appear in other branches

Rule:
👉 Always commit before switching branches

---

## 7. Delete a Branch

Delete safely:
`git branch -d feature1`

Force delete:
`git branch -D feature1`

Purpose:
- Remove unused branches after merge

---

## 8. Merging Branches

Steps:
1. Switch to target branch (main)
2. Merge feature branch

Commands:
`git switch main`,
`git merge feature1`

---

## 9. Fast-Forward Merge

Occurs when:
- main has no new commits
- feature branch is ahead

Result:
- main pointer moves forward
- No extra merge commit

---

## 10. Merge Commit (Basic Idea)

Occurs when:
- Both branches have new commits

Result:
- A new merge commit is created

Purpose:
- Keeps history clear

---

## 11. Important Rule Before Merge

Always pull latest code:
`git pull origin main`

Why:
- Avoid conflicts
- Ensure updated main branch

---

## 12. After Merge

Check status:
`git status`

Push changes:
`git push origin main`

---

## 13. Real-Life Workflow Example

1. Create feature branch
2. Make changes
3. Commit changes
4. Merge into main
5. Delete feature branch

---

## ✅ Summary

- Branch = independent work
- Merge = combine work
- main branch = stable code
- Feature branches = development

---

## End of Branching & Merging
