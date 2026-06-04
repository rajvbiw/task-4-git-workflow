# 🚀 DevOps Internship - Task 4

## Git Workflow Management Project

---

# 📌 Project Description

This project was completed as part of the DevOps Internship Task 4.
The objective of this task is to understand and implement Git best practices in a real DevOps project environment.

The project demonstrates:

* Git repository initialization
* GitHub integration
* Branch management
* Feature development workflow
* Pull Request workflow
* Merge operations
* Version tagging
* Documentation management

---

# 🛠️ Technologies Used

* Git
* GitHub
* Jenkins
* Docker
* Node.js

---

# 📂 Repository Workflow

The following Git workflow was implemented in this project:

```text
main → Production Branch
dev → Development Branch
feature/readme-update → Feature Branch
```

Workflow Process:

```text
Feature Branch → Dev Branch → Main Branch
```

---

# 🌿 Branches Created

| Branch Name           | Purpose                 |
| --------------------- | ----------------------- |
| main                  | Production-ready code   |
| dev                   | Development and testing |
| feature/readme-update | Feature implementation  |

---

# ⚙️ Git Commands Used

## Initialize Git Repository

```bash
git init
```

## Add Files

```bash
git add .
```

## Commit Changes

```bash
git commit -m "Initial commit"
```

## Create Branches

```bash
git checkout -b dev
git checkout -b feature/readme-update
```

## Push Code to GitHub

```bash
git push -u origin main
git push -u origin dev
```

## Merge Branches

```bash
git merge dev
```

## Create Git Tag

```bash
git tag v1.0
git push origin v1.0
```

---

# 🔀 Pull Request Workflow

A Pull Request (PR) workflow was followed to merge changes safely.

Steps:

1. Feature branch created
2. Changes committed
3. Feature branch pushed to GitHub
4. Pull Request created
5. Code merged into dev branch
6. Dev branch merged into main branch

---

# 🧾 .gitignore Usage

A `.gitignore` file was used to ignore unnecessary files such as:

```text
node_modules/
.env
*.log
dist/
```

---

# 🏷️ Git Tag

Git Tag created:

```text
v1.0
```

This tag represents the first stable version of the project.

---

# 📚 Learning Outcomes

Through this task, the following concepts were learned:

* Git version control
* Branching strategy
* Pull Request workflow
* Merge operations
* Git tags
* Documentation practices
* Collaboration workflow

---

# 👨‍💻 Author

Raj Birari

---

# ✅ Task Status

✔ Repository Created
✔ Branches Created
✔ Pull Request Used
✔ README Added
✔ Git Tag Added
✔ Documentation Completed
