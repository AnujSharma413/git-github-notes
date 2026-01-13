# Git Tags

This document explains **Git Tags**, why they are used, and how to create, view, and push them properly.

---

## 1. What is a Git Tag?

A **Git Tag** is a label that points to a specific commit.

👉 Mostly used to mark:
- Releases
- Versions (v1.0, v1.1, v2.0, etc.)
- Stable points in the project

Example:
- `v1.0` → First stable release
- `v1.1` → Bug fixes / minor updates

---

## 2. Why Use Git Tags?

Git Tags help to:
- Identify release versions easily
- Go back to a specific stable code
- Track project history clearly
- Deploy a specific version

✅ Tags do NOT change  
❌ Tags are NOT branches

---

## 3. Types of Git Tags

### 1️⃣ Lightweight Tag
- Just a pointer to a commit
- No extra information

### 2️⃣ Annotated Tag (Recommended)
- Stores tagger name
- Email
- Date
- Message

👉 Used for releases

---

## 4. View Existing Tags


`git tag`

Lists all tags in the repository.

* * *

## 5\. Create an Annotated Tag

`git tag -a v1.0 -m "First release"`

*   `v1.0` → tag name
    
*   `-m` → message
    

* * *

## 6\. View Tag Details

`git show v1.0`

Shows:

*   Tag info
    
*   Commit details
    
*   Changes at that version
    

* * *

## 7\. Create Tag After New Changes

1.  Make changes
    
2.  Commit changes
    

`git commit -m "processing user data"`

3.  Create new tag
    

`git tag -a v1.1 -m "Second release"`

* * *

## 8\. Push Tags to Remote Repository

By default, tags are **NOT pushed automatically**.

### Push a single tag

`git push origin v1.0`

### Push all tags

`git push origin --tags`

* * *

## 9\. Tags vs Branches

| Tag | Branch |
| --- | --- |
| Fixed pointer | Moves with commits |
| Used for releases | Used for development |
| Cannot change | Continuously updated |

* * *

## 10\. When to Use Tags?

Use tags when:

*   Releasing a version
    
*   Creating production builds
    
*   Marking stable checkpoints
    

* * *

## 11\. Common Tag Naming Convention

`v1.0, v1.1, v2.0, v2.1-beta`

* * *

## 12\. Summary

*   Git Tags mark specific commits
    
*   Mostly used for versioning & releases
    
*   Annotated tags are preferred
    
*   Tags must be pushed manually
    
*   Very important for real-world projects
    

* * *

## End of Git Tags