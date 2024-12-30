
# Git Basics Workshop 🛠️

A comprehensive guide for beginners to practice Git commands and concepts, based on the workshop materials.

## **Table of Contents**
- [Setup Git](#setup-git)
- [Common Git Commands](#common-git-commands)
- [Working with Local Repositories](#working-with-local-repositories)
- [Remote Repositories](#remote-repositories)
- [Git Stash](#git-stash)
- [Branching and Merging](#branching-and-merging)
- [Git Ignore](#git-ignore)
- [References](#references)

---

## **Setup Git**

### Install Git
```bash
sudo apt update
sudo apt install git
```

### Configure Git
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

### Validate Configuration
```bash
git config --list
```

---

## **Common Git Commands**

### Initialize a Git Repository
```bash
git init
```

### Clone a Repository
```bash
git clone https://github.com/yourusername/repo.git
```

### Add Changes to Staging Area
```bash
git add <file_name>
```

### Commit Changes
```bash
git commit -m "Your commit message"
```

### Check Status
```bash
git status
```

### View Commit History
```bash
git log
```

---

## **Working with Local Repositories**

### Create a New Repository
```bash
mkdir git-demo && cd git-demo
git init
```

### Create and Track a File
```bash
echo "Hello, Git!" > hello.txt
git add hello.txt
git commit -m "Initial commit"
```

---

## **Remote Repositories**

### Link to Remote Repository
```bash
git remote add origin https://github.com/yourusername/repo.git
git branch -M main
git push -u origin main
```

### Push Changes
```bash
git push
```

### Pull Changes
```bash
git pull origin main
```

---

## **Git Stash**

### Save Uncommitted Changes
```bash
git stash
```

### View Stash List
```bash
git stash list
```

### Apply and Remove Stash
```bash
git stash pop
```

---

## **Branching and Merging**

### Create a New Branch
```bash
git branch feature-branch
```

### Switch Branches
```bash
git checkout feature-branch
```

### Merge a Branch
```bash
git checkout main
git merge feature-branch
```

---

## **Git Ignore**

### Create a `.gitignore` File
Add the following contents to `.gitignore`:
```
*.pyc
__pycache__/
venv/
*.log
.env
```

### Add and Commit `.gitignore`
```bash
git add .gitignore
git commit -m "Add .gitignore"
```

---

## **References**

For more detailed information, refer to the full Git documentation at [git-scm.com](https://git-scm.com/).

---
