# Git Rebase – Clean Commit History

This document explains what Git rebase is,
why we use it, and how it is different from merge.

---

## 1. What is Git Rebase?

`Rebase`means:
Move your branch commits on top of another branch

Simple words:
- Rebase rewrites commit history
- Makes history clean and straight

---

## 2. Merge vs Rebase (Quick Difference)

### Merge
- Creates a merge commit
- History becomes complex (graph-like)
- Safe and non-destructive

### Rebase
- No merge commit
- History becomes linear (straight line)
- Rewrites commit history

---

## 3. When to Use Rebase?

Use rebase when:
- You want clean commit history
- You are working alone on a feature branch
- Branch is NOT pushed yet

⚠️ Do NOT rebase public/shared branches

---

## 4. Basic Rebase Workflow

You are on `main`
You want latest changes from `feature3`

Command:
`git rebase feature3`

Meaning:
- main commits are replayed on top of feature3

---

## 5. Real Example Flow

1. Create a feature branch
2. Make commits
3. main branch also gets new commits
4. Rebase feature branch on main

Commands:
`git switch feature3`,
`git rebase main`

---

## 6. Result of Rebase

- Old commits are replaced
- New commit hashes are generated
- History looks straight

Example:

- Before:
`feature → main → feature`

- After:
`main → feature → feature`

---

## 7. Check History Graph

Command:
`git log --graph --oneline`

Rebase result:
- No merge commit
- Straight commit line

---

## 8. Conflict During Rebase

If conflict occurs:
1. Fix the conflict
2. Add resolved files
3. Continue rebase

Commands:
`git add .`,
`git rebase --continue`

Abort rebase:
`git rebase --abort`

---

## 9. Rebase vs Pull

Default pull:
- `git pull`
= fetch + merge

Rebase pull:
- `git pull --rebase`
= fetch + rebase

Purpose:
- Avoid unnecessary merge commits

---

## 10. Golden Rules

✅ Use rebase for local branches  
❌ Never rebase pushed branches  
✅ Rebase before final merge  
❌ Rebase shared history

---

## ✅ Summary

- Rebase = clean history
- Merge = safe history
- Rebase rewrites commits
- Merge keeps original commits

---

## End of Git Rebase
