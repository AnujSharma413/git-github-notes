# Git Stash – Save Work Temporarily

This document explains Git Stash,
why it is used, and how to safely switch branches
without losing unfinished work.

---

## 1. What is Git Stash?

Git Stash is used to:
- Temporarily save uncommitted changes  
-  Switch branches safely  
- Resume work later

It works like a temporary locker for code.

---

## 2. When Do We Use Git Stash?

Use git stash when:
- You are working on a branch
- Changes are NOT ready to commit
- You urgently need to switch branch

Example:
Working on feature1 but need to fix issue in main.

---

## 3. Save Changes Using Stash

Command:
`git stash`

What happens:
- Working directory becomes clean
- Changes are stored safely
- You can switch branches

---

## 4. View Stashed Changes

Command:
`git stash list`

Output example:
`stash@{0}: WIP on feature1: Adding admin service`

---

## 5. Switch Branch After Stash

Command:
`git switch main`

Now you can:
- Fix bugs
- Commit changes
- Push code

---

## 6. Apply Stash Back

After finishing work, return to original branch:

`git switch feature1`

Apply stash:
`git stash apply`

Result:
- Changes come back
- Stash remains saved

---

## 7. Apply and Remove Stash (Optional)

Command:
`git stash pop`

This:
- Applies changes
- Deletes stash entry

---

## 8. Commit Stashed Changes

After applying stash:

`git add .`,
`git commit -m "ai enabled"`

Now changes are permanently saved.

---

## 9. Important Rules

✅ Stash only uncommitted work  
✅ Always check stash list  
❌ Do not forget applied stash  
❌ Avoid too many stashes

---

## 10. Why Git Stash is Useful?

- Emergency bug fixes
- Multitasking safely
- Clean working directory
- No code loss

---

## ✅ Summary

- git stash → save work
- git stash list → view stash
- git stash apply → restore work
- git stash pop → restore + delete
- Commit after applying

---

## End of Git Stash
