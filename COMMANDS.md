# Quick Command Reference

## First Time Setup

```bash
# Navigate to your project folder
cd path/to/your/folder

# Initialize git
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit - PTCB Flashcards app"

# Add remote (replace YOUR-USERNAME and YOUR-REPO-NAME)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## After Setup - Making Updates

```bash
# Check what files changed
git status

# Add all changed files
git add .

# Commit with a message
git commit -m "Your update message here"

# Push to GitHub (automatically updates your site)
git push
```

## Useful Commands

```bash
# See commit history
git log

# See what branch you're on
git branch

# Undo changes to a file (before commit)
git checkout -- filename.html

# Remove file from git (but keep locally)
git rm --cached filename.html
```

## Quick Reference URLs

- Your Repository: `https://github.com/YOUR-USERNAME/YOUR-REPO-NAME`
- Your Live Site: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME`
- Settings > Pages: `https://github.com/YOUR-USERNAME/YOUR-REPO-NAME/settings/pages`
