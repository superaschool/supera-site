# Supera Website - GitHub + Porkbun Integration

This repository contains the Supera Learning LLC website (supera.school).

## 🚀 Auto-Deploy Setup

### Step 1: Create GitHub Repository
1. Go to https://github.com/new
2. Repository name: `supera-site`
3. Make it **Public** (required for free hosting)
4. **DO NOT** initialize with README
5. Click "Create repository"

### Step 2: Push This Code to GitHub

```bash
cd /Users/camrom/Desktop/supera-github-repo

git remote add origin https://github.com/YOUR_USERNAME/supera-site.git

git add .
git commit -m "Initial Supera website"
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

### Step 3: Connect GitHub to Porkbun

1. Log into **Porkbun** → Domain Management
2. Find **supera.school** → Click house icon (Website)
3. Go to **Static Hosting** settings
4. Look for **"Connect GitHub Repository"**
5. Authorize Porkbun to access your GitHub
6. Select repository: `supera-site`
7. Branch: `main`
8. Directory: `/` (root)
9. Click **Connect**

### Step 4: Auto-Deploy is Live! 🎉

Now every `git push` automatically deploys to supera.school in ~30 seconds.

---

## 📝 Making Updates

### Quick Update Workflow:

```bash
# 1. Edit files in /Users/camrom/Desktop/supera-github-repo/
cd /Users/camrom/Desktop/supera-github-repo

# 2. Make your changes (edit index.html, etc.)

# 3. Commit and push
git add .
git commit -m "Update: [describe what changed]"
git push

# 4. Done! Porkbun auto-deploys in ~30 seconds
# Check: https://supera.school
```

---

## 📁 Repository Structure

```
supera-site/
├── index.html          # Main Supera landing page
├── icon_color.png      # Favicon (browser tab icon)
└── README.md           # This file
```

---

## 🎨 Design System

**Colors:**
- Primary: #0D0C0B (dark background)
- Accent: #F08C39 (orange)
- Secondary: #139294 (teal)
- Text: #F4F1ED (off-white)

**Typography:**
- Font: Outfit (Google Fonts)
- Weights: 300, 400, 500, 600, 700

**Branding:**
- Logo: Supera<span style="color: #F08C39;">.</span>
- Tagline: "Automate the boring, live the fun"

---

## 🔗 Quick Links

- **Live Site:** https://supera.school
- **Porkbun Dashboard:** https://porkbun.com/account/
- **GitHub Repo:** https://github.com/YOUR_USERNAME/supera-site

---

## 💡 Tips

- Keep changes small and frequent
- Test locally before pushing
- Use meaningful commit messages
- Site auto-deploys on every push to `main`

---

*Last updated: March 28, 2026*
*Supera Learning LLC*
