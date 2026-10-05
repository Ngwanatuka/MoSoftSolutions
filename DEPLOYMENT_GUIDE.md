# Mo Soft Solutions - GitHub Deployment Guide

## Issue: Git Push Authentication

The `git push` command is hanging because it needs GitHub authentication. Here are your options:

## ✅ **Option 1: Use GitHub CLI (Recommended)**

You already have `gh` installing. Once it completes:

```bash
# Authenticate with GitHub
gh auth login

# Follow the prompts:
# - Choose: GitHub.com
# - Choose: HTTPS
# - Authenticate via web browser

# Then push your code
cd /home/ngwanatuka/Portfolio/MoSoftSolutions
git push -u origin main --force
```

## ✅ **Option 2: Use Personal Access Token**

1. **Create a Personal Access Token**:
   - Go to: https://github.com/settings/tokens
   - Click **"Generate new token"** → **"Generate new token (classic)"**
   - Name: `MoSoftSolutions Deploy`
   - Expiration: Choose duration
   - Scopes: Check **`repo`** (full control of private repositories)
   - Click **"Generate token"**
   - **COPY THE TOKEN** (you won't see it again!)

2. **Push with Token**:
   ```bash
   cd /home/ngwanatuka/Portfolio/MoSoftSolutions
   git remote set-url origin https://YOUR_TOKEN@github.com/ngwanatuka/MoSoftSolutions.git
   git push -u origin main --force
   ```

## ✅ **Option 3: Use SSH (Most Secure)**

1. **Generate SSH Key** (if you don't have one):
   ```bash
   ssh-keygen -t ed25519 -C "ngwanatuka@gmail.com"
   # Press Enter to accept default location
   # Press Enter for no passphrase (or set one)
   ```

2. **Add SSH Key to GitHub**:
   ```bash
   cat ~/.ssh/id_ed25519.pub
   # Copy the output
   ```
   - Go to: https://github.com/settings/keys
   - Click **"New SSH key"**
   - Title: `MoSoftSolutions`
   - Paste the key
   - Click **"Add SSH key"**

3. **Change Remote to SSH**:
   ```bash
   cd /home/ngwanatuka/Portfolio/MoSoftSolutions
   git remote set-url origin git@github.com:ngwanatuka/MoSoftSolutions.git
   git push -u origin main --force
   ```

## ✅ **Option 4: Upload via GitHub Web Interface**

If the above don't work, you can manually upload:

1. Go to: https://github.com/ngwanatuka/MoSoftSolutions
2. Click **"Add file"** → **"Upload files"**
3. Drag and drop all files from `/home/ngwanatuka/Portfolio/MoSoftSolutions/`
4. Commit message: "Initial commit: Mo Soft Solutions website"
5. Click **"Commit changes"**

## 🚀 After Successful Push

Once your files are on GitHub:

1. **Enable GitHub Pages**:
   - Go to: https://github.com/ngwanatuka/MoSoftSolutions/settings/pages
   - Source: **main** branch
   - Folder: **/ (root)**
   - Click **Save**

2. **Wait 1-2 minutes** for deployment

3. **Visit your site**: https://ngwanatuka.github.io/MoSoftSolutions/

## 🔍 Verify Deployment

Check deployment status:
- Go to: https://github.com/ngwanatuka/MoSoftSolutions/deployments
- You should see a "github-pages" deployment

## 📝 Current Status

Your local repository is ready with all files:
- ✅ HTML, CSS, JavaScript files
- ✅ Logo and service icons
- ✅ README documentation
- ✅ Git repository initialized
- ⏳ Waiting for authentication to push

## 💡 Recommended Next Step

**Use GitHub CLI** (Option 1) - it's the easiest and most secure method for future deployments.

Once `gh` finishes installing, run:
```bash
gh auth login
cd /home/ngwanatuka/Portfolio/MoSoftSolutions
git push -u origin main --force
```

---

**Need help?** Let me know which option you'd like to use!
