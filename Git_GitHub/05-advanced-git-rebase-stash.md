# ⚡ 05 – Advanced Git (Rebase, Stash, Cherry-Pick & More)

> **Owner:** Rahul Upadhyay  


---

## 🧠 Why Advanced Git Exists

### English
In real companies:
- You get urgent tasks
- You make mistakes
- Your branch becomes messy
- You need clean history

Advanced Git helps you **fix, clean, and manage work safely**.

### Hinglish
Company me:
- Kabhi urgent bug aa jata hai
- Kabhi galti ho jati hai
- Kabhi branch messy ho jata hai

Advanced Git se tum **sab clean aur safe** bana sakte ho.

---

# 🧰 1️⃣ git stash – Save Work Without Commit

### English
`git stash` temporarily saves your unfinished work.

### Hinglish
`git stash` matlab:
> "Abhi ka kaam side me rakh do, baad me wapas le aunga."

---

### Real-Life Example

You are working on:
> feature-login

Suddenly boss says:
> "Fix production bug NOW!"

You don’t want to commit half work.

So you do:
```bash

>Diagram
git stash

Working on feature
      ↓
git stash
      ↓
Work saved safely
      ↓
Working directory clean
---------------------------------------------------
>See all stashesgit 
git stash list
