# Git Time Travel – Go Back to Any Commit

This document explains Git Time Travel,
how to move to old commits, create a new branch from past,
and safely work without breaking main code.

---

## 1. What is Git Time Travel?

Git Time Travel means:
- Going back to any previous commit
- Viewing or modifying old code
- Creating a new branch from old history

Git allows you to move freely across commits.

---

## 2. View Commit History

To see all commits:
`git log`

Short version:
`git log --oneline`

This shows commit hashes needed for time travel.

---

## 3. Checkout Old Commit

Command:
`git checkout <commit-hash>`

Example:
`git checkout fb8af3f`

Result:
- HEAD becomes detached
- You are NOT on any branch

---

## 4. Detached HEAD State

Detached HEAD means:
- You are viewing a commit directly
- Any new commit can be lost

`Git Warning:
Changes are not saved in any branch`

---

## 5. Create Branch from Old Commit (Important)

To safely work from old commit:

`git checkout -b lite-version`

OR (modern):

`git switch -c lite-version`

Now:
- A new branch is created
- Changes are safe

---

## 6. Make Changes in Old Version

1. Modify files
2. Stage changes
3. Commit changes

Commands:
`git add .`,
`git commit -m "lite version is ready"`

---

## 7. Push Time-Travel Branch to Remote

Command:
`git push origin lite-version`

Result:
- New branch appears on GitHub
- Independent from main branch

---

## 8. Switch Back to Latest Code

To return to main:
`git switch main`

OR:
`git checkout main`

---

## 9. Why Git Time Travel is Useful?

- Create lite version of product
- Fix bugs in old release
- Experiment safely
- Release hotfix from old commit

---

## 10. Important Rules

✅ Always create a branch from old commit  
❌ Do not work directly in detached HEAD  
✅ Push new branch separately  
❌ Do not modify history of main blindly

---

## ✅ Summary

- git log → find commit
- git checkout <hash> → time travel
- Detached HEAD → unsafe
- Create branch → safe
- Push branch → save work

---

## End of Git Time Travel
