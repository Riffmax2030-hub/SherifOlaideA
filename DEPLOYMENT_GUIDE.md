# 🚀 Deployment Guide: Git & Vercel

Follow these step-by-step instructions to push your portfolio to GitHub and deploy it on Vercel.

---

## Part 1: Push to GitHub

### Step 1: Create a GitHub Repository

1. Go to [github.com](https://github.com) and log in
2. Click the **"+"** icon in the top right → **"New repository"**
3. Name your repository: `portfolio` (or your preferred name)
4. Add description: "My AI & Full-Stack Developer Portfolio"
5. Choose **"Public"** (so it's visible to employers)
6. **Do NOT** initialize with README, .gitignore, or license (we already have these)
7. Click **"Create repository"**

### Step 2: Get Your Repository URL

After creating, you'll see a screen with commands. Copy your repository URL. It should look like:
```
https://github.com/yourusername/portfolio.git
```

### Step 3: Initialize Git & Push Your Code

Open a terminal/command prompt in your project folder and run:

```bash
# Initialize git
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial commit: Portfolio website"

# Add remote (replace with YOUR repository URL)
git remote add origin https://github.com/yourusername/portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**That's it!** Your code is now on GitHub.

---

## Part 2: Deploy on Vercel

### Step 1: Sign Up for Vercel

1. Go to [vercel.com](https://vercel.com)
2. Click **"Sign Up"**
3. Choose **"Continue with GitHub"**
4. Authorize Vercel to access your GitHub account

### Step 2: Import Your GitHub Repository

1. After signing in, click **"New Project"**
2. Find your **`portfolio`** repository in the list
3. Click **"Import"**

### Step 3: Configure Your Project

Vercel will auto-detect this is a static site. Just click **"Deploy"** - no configuration needed!

### Step 4: Wait for Deployment

Vercel will:
- Build your project
- Deploy it to their servers
- Give you a live URL

You'll see a screen like:
```
✓ Deployed to vercel.com
Preview URL: https://portfolio-yourusername.vercel.app
```

**🎉 Your portfolio is live!**

---

## Part 3: Custom Domain (Optional)

Want to use your own domain? In Vercel:

1. Go to your project → **"Settings"**
2. Click **"Domains"**
3. Add your custom domain
4. Follow DNS instructions from your domain provider

---

## Making Updates

When you make changes locally:

```bash
# Make your changes, then:
git add .
git commit -m "Update: description of changes"
git push
```

Vercel automatically redeploys when you push to GitHub!

---

## Troubleshooting

### "Deploy failed"
- Check that all files are in the repository
- Make sure `index.html` exists in the root folder

### "Page shows 404"
- Verify `vercel.json` exists and is correct
- Check that all CSS and JS files are linked properly

### "Styles not loading"
- Ensure `styles.css` and `script.js` paths are correct in `index.html`
- Clear browser cache (Ctrl+Shift+Delete)

---

## Need Help?

- **Vercel Docs**: https://vercel.com/docs
- **GitHub Docs**: https://docs.github.com
- **Contact**: Reach out if you need assistance!

---

**Your portfolio is now live and automatically updates with every push to GitHub! 🚀**
