# 🚀 SariKo Deployment - Quick Command Guide

Just copy-paste these commands in order. Don't overthink it.

---

## **BEFORE YOU START**

✅ GitHub account created (github.com)  
✅ Vercel account created (vercel.com)  
✅ Terminal/Command Prompt open  
✅ Navigate to your sariko-website folder  

---

## **COMMAND BLOCK 1: Git Setup (One-time)**

Run this once to tell Git who you are:

```bash
git config --global user.email "poppet@sariko.app"
git config --global user.name "Poppet Celdran"
```

---

## **COMMAND BLOCK 2: Initialize & Commit**

Run these commands in order:

```bash
git init
```

```bash
git add .
```

```bash
git commit -m "Initial SariKo website - Phase 1"
```

```bash
git branch -M main
```

---

## **COMMAND BLOCK 3: Connect to GitHub**

**FIRST:** Go to github.com → Create new repository → Name: `sariko-website`

**THEN:** Run this command (replace `YOUR_USERNAME`):

```bash
git remote add origin https://github.com/YOUR_USERNAME/sariko-website.git
git push -u origin main
```

**EXAMPLE:** If your GitHub username is `poppet-celdran`:

```bash
git remote add origin https://github.com/poppet-celdran/sariko-website.git
git push -u origin main
```

---

## **What You Should See**

After `git push`, you should see something like:

```
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Delta compression using up to 8 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (15/15), 150.00 KiB | 1.50 MiB/s, done.
Total 15 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/YOUR_USERNAME/sariko-website.git
 * [new branch]      main -> main
Branch 'main' is set to track remote branch 'main' from 'origin'.
```

✅ **If you see this, code is on GitHub!**

---

## **DEPLOY TO VERCEL (Web Only)**

1. Go to **vercel.com** (logged in with GitHub)
2. Click **"Add New"** → **"Project"**
3. Select **`sariko-website`** from the list
4. Click **"Deploy"**
5. Wait ~60 seconds
6. You see: ✓ Deployed!
7. Click the link → Your site is LIVE

---

## **FUTURE UPDATES (After You Add Community Links)**

When you want to update the site:

```bash
git add .
```

```bash
git commit -m "Description of what changed"
```

```bash
git push origin main
```

Vercel auto-deploys. Done in ~60 seconds.

---

## **IF SOMETHING GOES WRONG**

### **"git command not found"**
```bash
git --version
```

If error: Install Git
- Mac: `brew install git`
- Windows: Download from git-scm.com
- Linux: `sudo apt install git`

### **"Repository not found"**

Check your GitHub username:
```bash
git remote -v
```

Should show:
```
origin  https://github.com/YOUR_USERNAME/sariko-website.git (fetch)
origin  https://github.com/YOUR_USERNAME/sariko-website.git (push)
```

If wrong, fix it:
```bash
git remote set-url origin https://github.com/YOUR_USERNAME/sariko-website.git
```

### **Push fails with "everything up-to-date"**

That's okay! Your code is already on GitHub.

---

## **VERIFY EVERYTHING WORKED**

✅ Go to `github.com/YOUR_USERNAME/sariko-website` → See your files? SUCCESS!  
✅ Go to `vercel.com` → See deployment logs? SUCCESS!  
✅ Visit your Vercel URL → See your website? **LAUNCH SUCCESSFUL!**  

---

## **Share Your Live URL**

Send this to Poppet and early community:

```
https://sariko-website.vercel.app
```

---

## **Cheat Sheet (Copy These)**

**Git Setup (one-time):**
```bash
git config --global user.email "poppet@sariko.app"
git config --global user.name "Poppet Celdran"
```

**First Deploy:**
```bash
git init
git add .
git commit -m "Initial SariKo website - Phase 1"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/sariko-website.git
git push -u origin main
```

**Future Updates:**
```bash
git add .
git commit -m "Your message here"
git push origin main
```

---

**That's it. You got this.** 🚀

Just run the commands. Don't overthink. If stuck, read DEPLOYMENT_STEPS.md for full explanation.
