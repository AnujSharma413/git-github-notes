# Git Pull Request (PR)

This document explains the complete concept of Git Pull Request,
how it works, and how it is used in real projects.

---

## 1. What is a Pull Request?

A Pull Request (PR) is a request used to Merge your changes into another repository or branch.

It is commonly used when:
- Working on open-source projects
- Contributing to someone else’s repository
- Team collaboration

---

## 2. Why Pull Request is Needed?

Direct push is NOT allowed when:
- You don’t own the repository
- You are working on a forked project

So Pull Request helps to:
- Review code before merge
- Discuss changes
- Maintain code quality

---

## 3. Pull Request Real-Life Flow

1. Fork a repository
2. Clone forked repo
3. Create a new branch
4. Make changes
5. Commit changes
6. Push branch to your fork
7. Create Pull Request
8. Owner reviews & merges

---

## 4. Fork the Repository

Fork means:

Create a copy of someone else’s repository into your own GitHub account.

Example:
- Original repo: `microsoft/vscode`
- Forked repo: `your-username/vscode`

Fork is done using the **Fork button** on GitHub UI.

---

## 5. Clone Forked Repository

`
git clone https://github.com/your-username/repo-name.git
`

This creates a **local copy** of the forked repository on your system.

* * *

## 6. Create a New Branch

`git switch -c feature-branch`

### Why create a branch?

*   ❌ Never work directly on `main`

*   ✅ Pull Requests should always come from a **feature branch**

*   Helps keep changes isolated and clean


* * *

## 7. Make Changes & Commit

After editing files:

- `git add .`

- `git commit -m "Added new feature"`

This saves your changes in the feature branch.

* * *

## 8. Push Branch to Your Fork

`git push origin feature-branch`

👉 This pushes changes to **your GitHub repository**,  
👉 NOT to the original repository.

* * *

## 9. Create Pull Request (PR)

Steps on GitHub:

1.  Go to your forked repository

2.  Click **Compare & pull request**

3.  Add a clear **title** and **description**

4.  Click **Create pull request**


* * *

## 10. What Happens After PR?

*   Repository owner reviews the code

*   Comments or change requests may be added

*   If approved → PR is merged

*   Your changes become part of the original repository


* * *

## 11. After PR is Merged

You can:

*   🗑️ Delete your feature branch

*   🔄 Sync your fork with the original repository


* * *

## 12. Important PR Terms

| Term | Meaning |
| --- | --- |
| Fork | Copy of repository |
| PR | Request to merge code |
| Reviewer | Person who checks PR |
| Merge | Add changes to main repo |

* * *

## 13. PR Best Practices

✅ Create small and focused PRs  
✅ Write clear commit messages  
✅ Add proper PR description

❌ Never push directly to `main`  
❌ Don’t mix multiple features in one PR

* * *

## 14. PR Example Flow (Short)

`Fork → Clone → Branch → Change → Commit → Push → PR → Merge`

* * *

## 15\. Summary

*   Pull Request is used to contribute code

*   Mostly used with forked repositories

*   PR allows review before merging

*   Core concept of GitHub collaboration


***

## End of Git Pull Request