# 🌈 VS CODE → GITHUB COMPLETE WORKFLOW NOTES

### VS CODE:-

VS Code is your **workplace**, Git is your **time machine**, and GitHub is your **online locker**.

### Hinglish:

VS Code me kaam hota hai, Git version sambhalta hai, GitHub online save karta hai.

---

## 🧩 COMPLETE FLOW DIAGRAM (IMPORTANT)

```text
🧑‍💻 Developer (You)
        ↓
📂 Open Folder in VS Code
        ↓
⚙️ git init
        ↓
📝 Create / Edit Files (.md)
        ↓
➕ git add
        ↓
💬 git commit
        ↓
🌐 Connect to GitHub (remote)
        ↓
🚀 git push
        ↓
📦 Code Visible on GitHub
```

---

## 1️⃣ OPEN PROJECT IN VS CODE

### ✅ Steps:

* Open **VS Code**
* Click **File → Open Folder**
* Select or create a folder (example: `git-notes`)

### Hinglish:

VS Code me pehle ek folder open karo, wahi tumhara project hoga.

---

## 2️⃣ OPEN TERMINAL IN VS CODE

### Shortcut:

```
Ctrl + `
```

### Hinglish:

Terminal se hi Git ke commands chalenge.

---

## 3️⃣ INITIALIZE GIT (Start Tracking)

```bash
git init
```

### 🧠 What happens?

* `.git` folder create hota hai (hidden)
* Git tracking start ho jata hai

### Hinglish:

Ab Git tumhare folder ko yaad rakhna start karega.

---

## 4️⃣ CREATE A COLORFUL `.md` NOTES FILE

### Steps:

* Left panel → Right click → **New File**
* File name:

```
01-vscode-to-github-notes.md
```

### Example Content:

```md
# 🚀 My GitHub Notes

## 🌟 What is Git?
Git is a version control system.
```

---

## 5️⃣ SAVE FILE 💾

```
Ctrl + S
```

### Hinglish:

Save karna mat bhoolna.

---

## 6️⃣ CHECK FILE STATUS 🔍

```bash
git status
```

### Meaning:

* 🔴 Red → New / Untracked file
* 🟢 Green → Staged file

---

## 7️⃣ ADD FILE TO STAGING AREA ➕

```bash
git add .
```

### Hinglish:

Staging matlab commit ke liye ready.

---

## 8️⃣ COMMIT YOUR WORK 💬

```bash
git commit -m "Add VS Code to GitHub notes"
```

### 🧠 Think of commit as:

"Save point" or "Snapshot"

---

## 9️⃣ CREATE REPOSITORY ON GITHUB 🌐

### Steps:

1. Go to **GitHub → New Repository**
2. Repo name: `git-learning-notes`
3. Public
4. ❌ Do NOT add README (first push)
5. Click **Create Repository**

---

## 🔟 CONNECT VS CODE TO GITHUB 🔗

### 👤 Repository Owner

**Owner Name:** Rahul Upadhyay
(This repository and notes are maintained by Rahul Upadhyay)

---

### 📋 How to Copy Repository URL from GitHub (FIRST TIME USER)

#### Step-by-Step (Very Clear):

1. Open your **GitHub repository page** in browser
2. Click green **Code** button
3. Make sure **HTTPS** tab is selected
4. Click **Copy icon (📋)** next to URL

### Diagram:

```text
GitHub Repo Page
     ↓
Green [ Code ] Button
     ↓
HTTPS URL
     ↓
Click Copy 📋
```

### Hinglish:

GitHub par apna repo kholo → Code button dabao → HTTPS URL copy karo.

---

### Run this command in VS Code terminal:

```bash
git remote add origin https://github.com/username/git-learning-notes.git
```

### Check connection:

```bash
git remote -v
```

---

## 1️⃣1️⃣ PUSH FILE TO GITHUB 🚀

```bash
git branch -M main
git push -u origin main
```

### 🎉 Result:

* File GitHub par dikhne lagegi
* Repo live ho jayega

---

## 🖱️ ALTERNATE: PUSH USING VS CODE BUTTONS

1. Click **Source Control (🔀)** icon
2. Click **Stage All (+)**
3. Write commit message
4. Click **✔ Commit**
5. Click **Publish Branch**

---

## 🔐 AUTHENTICATION (VERY IMPORTANT – FIRST TIME USER)

### ❓ Why Token Needed?

### English:

GitHub does NOT allow password for push. Token works like a **secure password**.

### Hinglish:

Ab GitHub password allow nahi karta, isliye **Token** use hota hai.

---

## 🪪 HOW TO CREATE GITHUB TOKEN (STEP-BY-STEP)

### Steps (Do Slowly):

1. Open **GitHub → Profile Icon (top right)**
2. Click **Settings**
3. Click **Developer settings** (left menu bottom)
4. Click **Personal access tokens**
5. Click **Tokens (classic)**
6. Click **Generate new token (classic)**
7. Enter Note: `VS Code Git Access`
8. Select Expiration: `30 days` or `No expiration`
9. ✅ Select scopes:

   * repo
   * workflow
10. Click **Generate token**

---

### ⚠️ VERY IMPORTANT WARNING

```text
Copy the token immediately.
You will NOT see it again.
```

### Hinglish:

Token ek baar hi dikhega — copy karke safe jagah rakh lo.

---

## 🔑 HOW TO USE TOKEN IN VS CODE

### When you run `git push`:

* Username → Your GitHub username
* Password → **Paste TOKEN (not password)**

### Diagram:

```text
git push
   ↓
Ask Username → GitHub Username
   ↓
Ask Password → Paste TOKEN
   ↓
Authentication Success ✅
```

---

### ❌ Password not allowed

### ✅ Use GitHub Token

GitHub → Settings → Developer Settings → Personal Access Token

---

## 🏢 COMPANY-LEVEL WORKFLOW (REAL LIFE)

```text
Developer writes code
        ↓
Commit locally
        ↓
Push to GitHub
        ↓
Team reviews code
        ↓
Merge to main branch
```

---

## 🎯 BEST PRACTICES 🌟 (FOR BEGINNERS)

* Always use **HTTPS** URL
* Never share your token
* One topic = one `.md` file
* Clear commit messages
* Push daily (even small notes)

---

* One topic = one `.md` file
* Clear commit messages
* Push daily
* Keep repo clean

---

## 🔁 HOW TO EDIT AGAIN & PUSH AGAIN (VERY IMPORTANT)

> This section explains **what to do AFTER first push**

---

## 🧠 Simple Concept (English)

After first push:

* You **edit file**
* You **add** changes
* You **commit** changes
* You **push** again

Git remembers previous history automatically.

## 🧠 Simple Concept (Hinglish)

Ek baar push karne ke baad:

* File edit karo
* Dubara add karo
* Dubara commit karo
* Dubara push karo

Git khud history sambhal leta hai.

---

## 📝 STEP 1: EDIT YOUR `.md` FILE

### Example:

* Open `01-vscode-to-github-notes.md`
* Add new lines or fix mistakes
* Save file (`Ctrl + S`)

### Hinglish:

Bas file kholo, likho, save karo.

---

## 🔍 STEP 2: CHECK STATUS

```bash
git status
```

### Output Meaning:

* Modified file → Git ne change detect kar liya

---

## ➕ STEP 3: ADD CHANGES TO STAGING

```bash
git add .
```

### Hinglish:

Iska matlab: "Is change ko commit ke liye ready karo"

---

## 💬 STEP 4: COMMIT UPDATED CHANGES

```bash
git commit -m "Update notes with new explanation"
```

### 🧠 Remember:

* Har commit = ek save point
* Message clear rakho

---

## 🚀 STEP 5: PUSH AGAIN TO GITHUB

```bash
git push
```

### Result:

* GitHub par file update ho jayegi
* Old version history me safe rahegi

---

## 🔄 COMPLETE REPEAT PUSH DIAGRAM

```text
Edit File ✏️
   ↓
Save File 💾
   ↓
git status 🔍
   ↓
git add ➕
   ↓
git commit 💬
   ↓
git push 🚀
   ↓
GitHub Updated ✅
```

---

## 🖱️ ALTERNATE: USING VS CODE BUTTONS

1. Open **Source Control (🔀)**
2. See modified files
3. Click **Stage (+)**
4. Write commit message
5. Click **Commit (✔)**
6. Click **Sync / Push**

---

## ❌ COMMON BEGINNER MISTAKES

* ❌ Forgetting `git add`
* ❌ Writing bad commit message
* ❌ Thinking repo will duplicate (it will NOT)

---

