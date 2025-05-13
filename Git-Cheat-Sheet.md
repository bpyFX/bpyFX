# Git Cheat Sheet

## 🔄 INIT & CONFIG

Set up Git in your local environment.

```bash
git init                       # Start tracking this folder with Git
git config --global user.name "Your Name"   # Set your Git username
git config --global user.email "your@email.com"   # Set your Git email
```

## 🔍 STATUS & TRACKING

Check file states and stage changes for commit.

```bash
git status                    # Show changed files and what’s staged
git add .                     # Stage all changes
git add filename.py           # Stage a specific file
```

## 📸 COMMITTING CHANGES

Save a snapshot of staged changes to your local Git history.

```bash
git commit -m "Descriptive commit message"     # Commit staged changes with a message
git commit -am "Commit tracked files"          # Stage and commit in one step (only for modified files)
```

## ☁️ PUSH TO GITHUB

Upload your local commits to a GitHub repository.

```bash
git remote add origin https://github.com/youruser/repo.git   # Link local repo to remote GitHub repo
git branch -M main                                            # Rename current branch to main
git push -u origin main                                       # Push first commit and set upstream
git push                                                      # Push subsequent commits
```

## 🔄 PULL CHANGES FROM GITHUB

Get the latest updates from GitHub to your local repo.

```bash
git pull                     # Download and merge changes from GitHub
```

## 🧼 UNDO & CLEANUP

Reverse or clean up changes before committing.

```bash
git restore filename.py      # Undo local changes in a file
git reset HEAD filename.py   # Unstage a file (keep changes)
git checkout -- filename.py  # Revert file to last committed version
```

## 📚 BRANCHING

Create and manage branches for feature development.

```bash
git branch new-feature       # Create a new branch
git checkout new-feature     # Switch to that branch
git merge new-feature        # Merge changes into the current branch
```

## 🗑 IGNORING FILES

Prevent files/folders from being tracked by Git.
**.gitignore example:**

```
venv/
__pycache__/
*.pyc
.ipynb_checkpoints/
.env
```

## ✅ Typical Workflow

Your go-to sequence for making and pushing changes.

```bash
git status                   # Check what’s changed
git add .                    # Stage all changes
git commit -m "Your message"  # Commit changes with a message
git push                     # Push to GitHub
```
