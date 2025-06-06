# Git-Intro
# 🌱 Git & GitHub Complete Guide

A beginner-friendly guide to using Git and GitHub for version control and collaboration.

---

## 📘 What is Git?

**Git** is a **distributed version control system** used to track changes in source code during software development.

- 🧠 **Version Control**: Save multiple versions of your code.
- 👥 **Collaboration**: Work with others without conflict.
- 🧳 **Local & Remote**: Work offline, sync changes online.

---

## 🌐 What is GitHub?

**GitHub** is a cloud-based hosting service for Git repositories. It adds features like:
- Pull Requests
- Issues & Discussions
- Team Collaboration
- CI/CD Integration

---

## 🛠️ Git Setup

```bash
# Install Git (if not installed)
# https://git-scm.com/downloads

# Check Git version
git --version

# Set Git global config
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# View config
git config --list

# Git Project Workflow
# Step-by-step
git init                      # Initialize local repo
git add .                     # Stage changes
git commit -m "Initial commit" # Commit changes
git remote add origin https://github.com/username/repo.git
git push -u origin main       # Push code to GitHub


# 📦 Common Git Commands
#  Status & Logs
git status          # View changes
git log             # View commit history
git diff            # Show file changes
git show <commit>   # Show a specific commit

# ➕ Adding Files
git add filename    # Stage one file
git add .           # Stage all changes

# ✅ Committing Changes
git commit -m "Your message"       # Commit staged changes
git commit --amend                 # Edit last commit

# 🔗 Remote Repositories
git remote add origin <url>       # Add remote repo
git remote -v                     # View remotes
git push -u origin main           # Push for the first time
git push                          # Push changes
git pull                          # Pull latest changes

# 📄 Cloning Repositories
git clone <repo-url>              # Clone a repo

# 🌿 Branching in Git
git branch                        # List branches
git branch new-feature            # Create branch
git checkout new-feature          # Switch branch
git checkout -b new-feature       # Create + switch
git merge new-feature             # Merge branch into current
git branch -d new-feature         # Delete branch

# ⚠️ Merge Conflicts
# Resolve manually
# Remove >>>>, ====, <<<< in code
git add conflicted-file
git commit

# 🔄 Undo & Reset
git restore filename              # Discard local changes
git reset HEAD filename           # Unstage a file
git reset --hard HEAD             # Reset all to last commit

# ❓ Git Ignore
Create a .gitignore to exclude files:
# Example
node_modules/
.env
build/
.DS_Store

# 🧹 Cleaning Up
git clean -f                     # Remove untracked files
git clean -fd                    # Remove untracked files and dirs
