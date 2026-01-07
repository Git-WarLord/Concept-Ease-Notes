# 🚀 02 – Git Daily Workflow & Commands

> **Owner:** Rahul Upadhyay


Every day, a developer **edits files → saves changes → commits → pushes**.

### Hinglish:

Roz ka Git ka kaam bas itna hi hota hai:
**edit → add → commit → push**.

---

## 🔁 DAILY GIT WORKFLOW (VISUAL DIAGRAM)

```text
🧑‍💻 You (Developer)
   ↓
✏️ Edit File
   ↓
💾 Save File
   ↓
🔍 git status
   ↓
➕ git add
   ↓
💬 git commit
   ↓
🚀 git push
   ↓
🌐 GitHub Updated
```

---

## 1️⃣ git status — CHECK CURRENT STATE

```bash
git status
```

### English:

Shows which files are:

* New
* Modified
* Staged

### Hinglish:

Batata hai kaun si file new hai, kaun si change hui hai.

### Tip:

👉 **Always run `git status` before and after every step**.

---

## 2️⃣ git add — STAGE YOUR CHANGES

### Add single file:

```bash
git add file.md
```

### Add all files:

```bash
git add .
```

### English:

Moves changes to **staging area** (ready for commit).

### Hinglish:

Commit ke liye file ready karta hai.

---

## 3️⃣ git commit — SAVE SNAPSHOT

```bash
git commit -m "Write clear message"
```

### English:

Creates a **save point** with message.

### Hinglish:

Ek safe save bana deta hai.

### Good Commit Message Examples:

* Add Git daily workflow notes
* Fix spelling errors
* Update README

---

## 4️⃣ git push — SEND TO GITHUB

```bash
git push
```

### English:

Uploads commits to GitHub.

### Hinglish:

Local changes GitHub par bhej deta hai.

---

## 🔄 FULL FILE LIFECYCLE (VERY IMPORTANT)

```text
Untracked File (Red)
      ↓ git add
Staged File (Green)
      ↓ git commit
Committed
      ↓ git push
On GitHub
```

---

## 5️⃣ git log — VIEW HISTORY

```bash
git log
```

### English:

Shows all previous commits.

### Hinglish:

Pehle ke sab saves dikha deta hai.

---

## 6️⃣ git diff — SEE WHAT CHANGED

```bash
git diff
```

### English:

Shows line-by-line changes.

### Hinglish:

Batata hai file me kya badla.

---

## 7️⃣ git pull — GET LATEST CODE

```bash
git pull
```

### English:

Downloads latest code from GitHub.

### Hinglish:

GitHub se latest update laata hai.

---

## 🏢 REAL COMPANY DAILY FLOW

```text
Morning:
- git pull

Work:
- Edit files
- git add
- git commit

End of day:
- git push
```

---

## ❌ COMMON BEGINNER MISTAKES

* ❌ Forgetting `git add`
* ❌ Big unclear commit messages
* ❌ Editing without pulling latest code



---

## ✅ FINAL SUMMARY

✔ git status → check
✔ git add → stage
✔ git commit → save
✔ git push → upload
✔ git pull → update

---
