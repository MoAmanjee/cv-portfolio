# Setup Instructions for GitHub

## Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **+** icon in the top right → **New repository**
3. Repository name: `cv-portfolio` (or any name you prefer)
4. Description: "My professional CV and Portfolio website"
5. Make it **Public** (required for free GitHub Pages)
6. **DO NOT** initialize with README, .gitignore, or license (we already have these)
7. Click **Create repository**

## Step 2: Push Your Code to GitHub

Run these commands in your terminal (from the cv-portfolio directory):

```bash
cd /Users/mo.a/cv-portfolio

# Add your GitHub repository as remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/cv-portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Note:** You'll need to authenticate. GitHub may ask for:
- Username: Your GitHub username
- Password: Use a Personal Access Token (see Step 3 if needed)

## Step 3: Create Personal Access Token (if needed)

If GitHub asks for a password:

1. Go to GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Click **Generate new token (classic)**
3. Give it a name like "CV Portfolio"
4. Select scopes: **repo** (full control)
5. Click **Generate token**
6. **Copy the token** (you won't see it again!)
7. Use this token as your password when pushing

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under **Source**, select:
   - Branch: **main**
   - Folder: **/ (root)**
5. Click **Save**

## Step 5: Your Live Website

After a few minutes, your portfolio will be live at:
```
https://YOUR_USERNAME.github.io/cv-portfolio/
```

Or directly to portfolio:
```
https://YOUR_USERNAME.github.io/cv-portfolio/portfolio.html
```

## Step 6: Update CV Link

Once your site is live, update the portfolio link in your CV HTML file to point to your GitHub Pages URL, then commit and push again.

## Quick Commands Reference

```bash
# Navigate to repository
cd /Users/mo.a/cv-portfolio

# Make changes, then:
git add .
git commit -m "Your commit message"
git push

# Your changes will be live on GitHub Pages in 1-2 minutes
```

## Troubleshooting

- **404 Error**: Wait 1-2 minutes after enabling Pages, it takes time to deploy
- **Authentication Error**: Make sure you're using a Personal Access Token, not your password
- **Repository not found**: Check that the repository name matches exactly

---

**Your repository is ready!** Just follow the steps above to push it to GitHub and enable Pages.

