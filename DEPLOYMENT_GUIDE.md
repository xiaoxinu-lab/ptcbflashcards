# GitHub Pages Deployment Guide

Follow these steps to publish your PTCB Flashcards app to GitHub Pages.

## Prerequisites

1. A GitHub account (create one at https://github.com if you don't have one)
2. Git installed on your computer (download from https://git-scm.com if needed)

## Step-by-Step Instructions

### Step 1: Create a New GitHub Repository

1. Go to https://github.com and log in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Fill in the details:
   - **Repository name**: `ptcb-flashcards` (or any name you prefer)
   - **Description**: "PTCB Top 200 Drugs Flashcard Study App"
   - **Visibility**: Choose "Public" (required for free GitHub Pages)
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)
5. Click "Create repository"

### Step 2: Initialize Git Locally

Open your terminal/command prompt and navigate to the folder containing your files, then run:

```bash
# Initialize a git repository
git init

# Add all files to git
git add .

# Create your first commit
git commit -m "Initial commit - PTCB Flashcards app"

# Add your GitHub repository as the remote origin
# Replace YOUR-USERNAME and YOUR-REPO-NAME with your actual values
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Rename the default branch to main (if needed)
git branch -M main

# Push your code to GitHub
git push -u origin main
```

**Note**: Replace `YOUR-USERNAME` with your GitHub username and `YOUR-REPO-NAME` with your repository name.

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" (top menu bar)
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click "Save"

### Step 4: Wait for Deployment

1. GitHub will now build and deploy your site (usually takes 1-3 minutes)
2. Refresh the Settings > Pages page
3. You'll see a message: "Your site is live at https://YOUR-USERNAME.github.io/ptcb-flashcards/"

### Step 5: Visit Your Live Site

Click the link or visit: `https://YOUR-USERNAME.github.io/ptcb-flashcards/`

Your flashcard app is now live! 🎉

## Alternative: Using GitHub Desktop (Easier for Beginners)

If you prefer a graphical interface:

1. Download and install GitHub Desktop from https://desktop.github.com
2. Open GitHub Desktop
3. Click "File" > "Add Local Repository"
4. Select the folder containing your flashcard files
5. Click "Publish repository" in the top menu
6. Fill in the repository name and click "Publish Repository"
7. Then follow Step 3 above to enable GitHub Pages

## Updating Your Site

Whenever you make changes:

```bash
git add .
git commit -m "Description of your changes"
git push
```

GitHub Pages will automatically update your site in 1-3 minutes.

## Troubleshooting

### Issue: Site shows 404 error
- **Solution**: Make sure you have an `index.html` file in the root directory
- Wait a few more minutes for deployment to complete

### Issue: Git command not found
- **Solution**: Install Git from https://git-scm.com

### Issue: Permission denied when pushing
- **Solution**: You may need to set up authentication:
  - Use GitHub Desktop (easier), or
  - Set up SSH keys: https://docs.github.com/en/authentication/connecting-to-github-with-ssh
  - Or use a Personal Access Token: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

### Issue: Changes not appearing
- **Solution**: 
  - Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
  - Wait 2-3 minutes for GitHub Pages to rebuild
  - Check if your commit was pushed successfully on GitHub.com

## Custom Domain (Optional)

If you want to use your own domain name:

1. Buy a domain from any domain registrar (GoDaddy, Namecheap, etc.)
2. In your repository, create a file named `CNAME` with your domain name
3. Configure your domain's DNS settings to point to GitHub Pages
4. See full instructions: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## Need Help?

- GitHub Pages Documentation: https://docs.github.com/en/pages
- Git Documentation: https://git-scm.com/doc
- GitHub Community: https://github.community
