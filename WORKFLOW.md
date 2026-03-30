# Supera Development Workflow

## Branch Setup

| Branch | Purpose | Auto-Deploys? |
|--------|---------|---------------|
| `main` | Production site | ✅ YES |
| `develop` | Work in progress | ❌ NO |

---

## Working on Big Changes

### Step 1: Switch to develop branch
```bash
cd /Users/camrom/Desktop/supera-github-repo
git checkout develop
```

### Step 2: Make your changes
```bash
# Edit files, experiment, test...
# Edit index.html
# Add new features
# Whatever you need
```

### Step 3: Commit and push (WON'T auto-deploy!)
```bash
git add .
git commit -m "Work in progress: [describe changes]"
git push origin develop
```

---

## Going Live (Deploy to Production)

### Option A: Merge to main (Recommended)
```bash
# Make sure you're on develop branch
git checkout develop
# Commit any final changes
git add .
git commit -m "Ready for production"

# Switch to main and merge
git checkout main
git merge develop
git push origin main

# → Auto-deploys to supera.school!
```

### Option B: Direct push to main (Quick fixes only)
```bash
git checkout main
# Make small fix
git add .
git commit -m "Quick fix: [description]"
git push origin main
# → Auto-deploys!
```

---

## Quick Reference

**Current branch:**
```bash
git branch
```

**Switch branches:**
```bash
git checkout main      # Production
git checkout develop   # Work in progress
```

**See what changed:**
```bash
git status
git diff
```

---

## Tips

- ✅ Small fixes → Push directly to `main`
- 🔧 Big changes → Work on `develop`, merge when ready
- 🚫 Never commit secrets to either branch
- 💡 Test locally before merging to main

---

*Last updated: March 28, 2026*
