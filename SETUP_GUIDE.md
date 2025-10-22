# GitHub Repository Setup Guide

This guide will help you set up the Agoraphobia repository on GitHub.

## Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the **"+"** icon in the top right → **"New repository"**
3. Fill in the details:
   - **Repository name**: `agoraphobia`
   - **Description**: `Free-to-play tower defense game serving as Gorbagana's universal onramp`
   - **Visibility**: Choose Public or Private
   - **DO NOT** initialize with README (you already have one)
4. Click **"Create repository"**

## Step 2: Prepare Your Local Files

Download all the files from the outputs folder, which includes:

```
agoraphobia/
├── assets/
│   └── images/
│       ├── poster.png
│       ├── wallet-interface.png
│       ├── gameplay.png
│       ├── shop-defenses.png
│       ├── shop-shooters.png
│       ├── enemy-character.png
│       └── README.md
├── docs/
├── .gitignore
├── CONTRIBUTING.md
├── LICENSE
├── README.md
└── WHITEPAPER.md
```

## Step 3: Initialize Git Repository

Open your terminal/command prompt in the folder where you downloaded the files, then run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Make your first commit
git commit -m "Initial commit: Agoraphobia whitepaper and concept art"

# Set your branch to main (GitHub's default)
git branch -M main

# Add your GitHub repository as remote
# Replace YOUR_USERNAME with your actual GitHub username
git remote add origin https://github.com/YOUR_USERNAME/agoraphobia.git

# Push to GitHub
git push -u origin main
```

## Step 4: Customize Your Repository

### Update README.md

Replace placeholder text in README.md:
- Change `yourusername` to your actual GitHub username
- Add your contact information
- Update social media links when available

### Update WHITEPAPER.md

Replace the GitHub repository link:
- Change `yourusername` to your actual GitHub username

### Configure Repository Settings

On GitHub, go to your repository → **Settings**:

1. **About** (top right):
   - Add description
   - Add topics: `tower-defense`, `blockchain`, `gaming`, `crypto`, `unity`
   - Add website (if you have one)

2. **Features**:
   - ✓ Issues (for bug reports and feature requests)
   - ✓ Projects (optional, for project management)
   - ✓ Wiki (optional, for additional documentation)

3. **Social Preview**:
   - Upload `assets/images/poster.png` as the social preview image

## Step 5: Create GitHub Pages (Optional)

To create a nice landing page:

1. Go to **Settings** → **Pages**
2. Under "Source", select `main` branch
3. Click **Save**
4. Your site will be live at `https://YOUR_USERNAME.github.io/agoraphobia/`

## Step 6: Set Up Issue Templates (Optional)

Create `.github/ISSUE_TEMPLATE/` directory and add templates for:
- Bug reports
- Feature requests
- Questions

## Quick Commands Reference

```bash
# Clone your repository
git clone https://github.com/YOUR_USERNAME/agoraphobia.git

# Check status
git status

# Add changes
git add .

# Commit changes
git commit -m "Description of changes"

# Push to GitHub
git push

# Pull latest changes
git pull

# Create new branch
git checkout -b feature-name

# Switch branches
git checkout main
```

## Troubleshooting

### "Permission denied" error
- Make sure you're authenticated with GitHub
- Use HTTPS or set up SSH keys
- See: https://docs.github.com/en/authentication

### Images not showing
- Make sure image paths in markdown use relative paths
- Check that images are committed to the repository
- Verify image filenames match exactly (case-sensitive)

### Large file issues
- Keep individual files under 50MB
- Use Git LFS for large assets if needed
- Optimize images before committing

## Next Steps

1. ✅ Repository is live!
2. Share the repository link with your team
3. Start accepting contributions via pull requests
4. Set up project boards for task management
5. Create additional documentation as development progresses

## Need Help?

- [GitHub Documentation](https://docs.github.com)
- [Git Documentation](https://git-scm.com/doc)
- [Markdown Guide](https://www.markdownguide.org)

---

**Remember**: Update `YOUR_USERNAME` with your actual GitHub username in all files!
