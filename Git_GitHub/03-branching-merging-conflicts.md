# 🌿 03 – Branching, Merging & Conflicts 

> **Owner:** Rahul Upadhyay


### English:

Branching allows multiple developers to work **independently** without breaking the main code.

### Hinglish:

Branch ka matlab: **alag-alag kaam, bina main code kharab kiye**.

---

## 🌳 WHAT IS A BRANCH?

### English:

A branch is a **separate line of development**.

### Hinglish:

Branch ek **copy jaisa** hota hai jisme tum apna kaam safely karte ho.

### Real-Life Example:

Think of Google Docs:

* Original document = `main` branch
* You click "Make a copy" = new branch

---

## 🌲 BRANCH VISUAL DIAGRAM

```text
main
 |
 |--- feature-login
 |
 |--- feature-profile
```

---

## 🏗️ WHY BRANCHING IS IMPORTANT (COMPANY VIEW)

* Multiple people work at same time
* Bugs don’t affect production
* Easy testing

### Hinglish:

Company me bina branch ke kaam karna **dangerous** hota hai.

---

## 1️⃣ CHECK CURRENT BRANCH

```bash
git branch
```

### Output:

`* main` → you are on main branch

---

## 2️⃣ CREATE A NEW BRANCH

```bash
git branch feature-notes
```

### Hinglish:

Naya branch bana diya, par abhi use kar nahi rahe.

---

## 3️⃣ SWITCH TO NEW BRANCH

```bash
git checkout feature-notes
```

### OR (modern way):

```bash
git switch feature-notes
```

---

## 4️⃣ CREATE + SWITCH (ONE COMMAND)

```bash
git checkout -b feature-notes
```

### Hinglish:

Ek command me branch banana + use karna.

---

## 🔁 BRANCH WORKFLOW DIAGRAM

```text
main branch
     ↓
create branch
     ↓
work safely
     ↓
commit changes
     ↓
merge back
```

---

## 5️⃣ MERGING A BRANCH

### Step-by-Step:

1. Go to main branch

```bash
git checkout main
```

2. Merge feature branch

```bash
git merge feature-notes
```

### Hinglish:

Feature ka kaam main branch me add ho jayega.

---

## 🔀 MERGE DIAGRAM

```text
Before Merge:
main -----o
            \
             o--- feature

After Merge:
main -----o-----o
```

---

## ⚠️ WHAT IS A MERGE CONFLICT?

### English:

When Git cannot decide which change to keep.

### Hinglish:

Jab same line ko 2 jagah se change kar diya jata hai.

---

## 💥 CONFLICT REAL-LIFE EXAMPLE

* You change line 5
* Your teammate also changes line 5
* Git gets confused 😕

---

## 🧨 CONFLICT DIAGRAM

```text
main:    Hello World
branch:  Hello Rahul
         ↑ same line
```

---

## 🛠️ HOW TO RESOLVE CONFLICT (STEP-BY-STEP)

### Step 1: Git shows conflict

```text
<<<<<<< HEAD
Hello World
=======
Hello Rahul
>>>>>>> feature
```

### Step 2: Choose correct code

```text
Hello Rahul
```

### Step 3: Save file

### Step 4: Add & commit

```bash
git add .
git commit -m "Resolve merge conflict"
```

---

## 🖱️ RESOLVE CONFLICT USING VS CODE UI

* VS Code shows buttons:

  * Accept Current
  * Accept Incoming
  * Accept Both

### Hinglish:

Button click karke easily conflict solve hota hai.

---

## 🏢 COMPANY-LEVEL BRANCH STRATEGY

```text
main  → Production code
 |
 |--- develop
 |       |
 |       |--- feature branches
```

### Rules:

* Never work directly on `main`
* Always create feature branch

---

## ❌ COMMON BEGINNER MISTAKES

* ❌ Working directly on main
* ❌ Forgetting to pull before merge
* ❌ Panic during conflict

---

## 🌟 BEST PRACTICES

* Small branches
* One feature per branch
* Delete branch after merge

---

## ✅ FINAL SUMMARY

✔ Branch = safe workspace
✔ Merge = bring work together
✔ Conflict = same line changed
✔ VS Code makes conflicts easy

