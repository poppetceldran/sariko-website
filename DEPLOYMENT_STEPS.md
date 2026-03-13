# 🚀 SariKo Website - Complete Deployment Guide

## **Overview**

You're going to deploy to **Vercel** (fastest, free, auto-deploys from GitHub).

**Timeline:** 30 minutes total  
**Cost:** $0 (free tier)  
**Difficulty:** Easy (copy-paste commands)  

---

## **PART 1: Prerequisites (5 minutes)**

### **Step 1.1: Create GitHub Account (if you don't have one)**

1. Go to **github.com**
2. Click **"Sign up"**
3. Use your email (e.g., poppet@sariko.app)
4. Create password
5. Verify email
6. Done

### **Step 1.2: Create Vercel Account**

1. Go to **vercel.com**
2. Click **"Sign Up"**
3. Click **"Continue with GitHub"**
4. Authorize GitHub
5. Done (Vercel now linked to your GitHub)

---

## **PART 2: Upload Code to GitHub (10 minutes)**

### **Step 2.1: Open Terminal/Command Prompt**

**On Mac:** Applications → Utilities → Terminal  
**On Windows:** Press `Win + R` → type `cmd` → Enter  
**On Linux:** Open terminal  

### **Step 2.2: Navigate to Your Project**

```bash
cd /path/to/sariko-website
```

**Example for Mac/Linux:**
```bash
cd ~/Desktop/sariko-website
```

**Example for Windows:**
```bash
cd C:\Users\YourName\Desktop\sariko-website
```

### **Step 2.3: Check Git is Installed**

```bash
git --version
```

**Should return:** `git version 2.x.x` or higher

If not installed:
- **Mac:** `brew install git`
- **Windows:** Download from git-scm.com
- **Linux:** `sudo apt-get install git`

### **Step 2.4: Set Your Git Identity (One-time only)**

```bash
git config --global user.email "your@email.com"
git config --global user.name "Your Name"
```

**Example:**
```bash
git config --global user.email "poppet@sariko.app"
git config --global user.name "Poppet Celdran"
```

### **Step 2.5: Create GitHub Repository**

1. Go to **github.com** (logged in)
2. Click **+** icon (top right)
3. Click **"New repository"**
4. Fill in:
   - **Repository name:** `sariko-website`
   - **Description:** "SariKo marketplace website"
   - **Public** (so anyone can see it)
   - **Initialize with README?** NO (we already have files)
5. Click **"Create repository"**
6. Copy the commands it shows (you'll use them next)

### **Step 2.6: Upload Code to GitHub**

In your terminal, run these commands **in order:**

```bash
git init
git add .
git commit -m "Initial SariKo website - Phase 1"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/sariko-website.git
git push -u origin main
```

**Replace `YOUR_USERNAME`** with your GitHub username.

**Example:**
```bash
git remote add origin https://github.com/poppet-celdran/sariko-website.git
```

**What these commands do:**
- `git init` — Initialize Git repository
- `git add .` — Stage all files
- `git commit` — Create a snapshot
- `git branch -M main` — Set main branch name
- `git remote add origin` — Connect to GitHub
- `git push` — Upload to GitHub

### **Step 2.7: Verify Upload**

1. Go to **github.com/YOUR_USERNAME/sariko-website**
2. You should see all your files uploaded
3. ✅ Done with GitHub

---

## **PART 3: Deploy to Vercel (5 minutes)**

### **Step 3.1: Go to Vercel Dashboard**

1. Go to **vercel.com**
2. Make sure you're logged in
3. Click **"Add New"** → **"Project"**

### **Step 3.2: Import GitHub Repository**

1. Under **"Import Git Repository"**
2. You should see your GitHub repos listed
3. Find **`sariko-website`**
4. Click **"Select"**

### **Step 3.3: Configure Project**

The page shows configuration options. **Leave everything as default:**

- **Framework Preset:** Next.js (should auto-detect)
- **Root Directory:** `./`
- **Environment Variables:** (leave empty)

Click **"Deploy"**

### **Step 3.4: Wait for Deployment**

- You'll see "Building..." 
- Then "Analyzing"
- Then "Compiling"
- Finally "✓ Deployed"
- Takes ~1-2 minutes

### **Step 3.5: Get Your Live URL**

Once deployed, you'll see:
```
Congratulations! Your project is live at:
https://sariko-website.vercel.app
```

**That's your live website URL.** Share this!

---

## **PART 4: Test Your Site (5 minutes)**

### **Step 4.1: Visit Your Site**

1. Click the URL or copy-paste into browser
2. https://sariko-website.vercel.app
3. Should load your SariKo website

### **Step 4.2: Test All Buttons**

- [ ] Hero buttons work
- [ ] "Become Founding Seller" goes to link.zenapappro.com/sariko-icp
- [ ] Buyer email form works
- [ ] Community buttons show "Coming Soon" (greyed out)
- [ ] Footer email link works

### **Step 4.3: Test on Mobile**

1. Open on phone
2. Should be responsive (no horizontal scroll)
3. All text readable
4. Buttons tappable

### **Step 4.4: Share the URL**

Send `https://sariko-website.vercel.app` to Poppet and early community.

---

## **PART 5: Update Community Links Later (When Ready)**

When you create your Facebook, WhatsApp, Zalo groups:

### **Step 5.1: Edit the File**

1. Open `sariko-website/app/page.tsx` in a text editor
2. Find the Community section (around line 428)
3. Replace the greyed-out buttons with real links

### **Step 5.2: Update the Code**

Find this section:
```jsx
<div style={{ position: 'relative', display: 'inline-block' }}>
  <button disabled style={{...}}>
    Facebook Group →
  </button>
```

Change it to:
```jsx
<a href="https://facebook.com/groups/YOUR_ID" className="btn" style={{ padding: '0.875rem 1.5rem', fontSize: '0.95rem' }}>
  Facebook Group →
</a>
```

Do the same for WhatsApp and Zalo.

### **Step 5.3: Deploy the Update**

```bash
git add .
git commit -m "Add community group links"
git push origin main
```

Vercel **auto-deploys** when you push to GitHub.

---

## **PART 6: Custom Domain (Optional, Next Week)**

If you want `sariko.app` instead of `sariko-website.vercel.app`:

### **Option A: Use Zen Tech Asia Subdomain (Recommended)**

Use `sariko.zenapappro.com`

**Steps:**
1. Tell Zen Tech Asia hosting team to create subdomain
2. In Vercel project → Settings → Domains
3. Add `sariko.zenapappro.com`
4. Vercel gives you nameservers
5. Host updates nameservers
6. Live in ~1 hour

### **Option B: Buy Your Own Domain**

Cost: $12-15/year

**Steps:**
1. Buy at Hostinger, GoDaddy, Namecheap
2. In Vercel → Settings → Domains
3. Add your domain
4. Update nameservers (Vercel provides them)
5. Live in ~24 hours

**For now:** Use free `sariko-website.vercel.app` until you're ready to invest in custom domain.

---

## **Quick Reference: All Commands**

```bash
# Step 1: Navigate to project
cd /path/to/sariko-website

# Step 2: Set git identity (one-time)
git config --global user.email "poppet@sariko.app"
git config --global user.name "Poppet Celdran"

# Step 3: Initialize and push to GitHub
git init
git add .
git commit -m "Initial SariKo website - Phase 1"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/sariko-website.git
git push -u origin main

# Step 4: Future updates (after you add community links)
git add .
git commit -m "Add community links"
git push origin main
# Vercel auto-deploys
```

---

## **Troubleshooting**

### **Problem: `git` command not found**

**Solution:**
- **Mac:** `brew install git`
- **Windows:** Download from git-scm.com
- **Linux:** `sudo apt install git`

Then run `git --version` to verify.

---

### **Problem: "Repository not found" error**

**Solution:**
1. Check your GitHub username is correct
2. Make sure GitHub repo exists (visit github.com/YOUR_USERNAME/sariko-website)
3. Check your git remote: `git remote -v`
4. If wrong, fix it: `git remote set-url origin https://github.com/YOUR_USERNAME/sariko-website.git`

---

### **Problem: Vercel build fails**

**Solution:**
1. Go to vercel.com → Your project → Deployments
2. Click the failed deployment
3. Look at the error message
4. Most common: Missing files or syntax error
5. Fix in your editor, push again: `git push origin main`
6. Vercel auto-retries

---

### **Problem: Site is blank or shows error**

**Solution:**
1. Wait 2 minutes (sometimes takes time)
2. Hard refresh browser (Ctrl+Shift+R or Cmd+Shift+R)
3. Check Vercel deployment logs
4. Check for typos in code

---

## **Post-Launch Checklist**

- [ ] Website is live at sariko-website.vercel.app
- [ ] All buttons work
- [ ] Mobile view works
- [ ] Share URL with Poppet
- [ ] Share with 5-10 early community
- [ ] Monitor founding seller inquiries (link.zenapappro.com/sariko-icp)
- [ ] Monitor buyer email signups
- [ ] When community groups ready → Update links → Push to GitHub → Auto-deploy
- [ ] Week 2: Share in Facebook groups, WhatsApp, Zalo
- [ ] Week 3: Collect feedback, iterate

---

## **What Now?**

1. **Have you created a GitHub account?** If not, do step 1.1 first
2. **Once you have GitHub + Vercel accounts:** Run the commands in PART 2
3. **Once code is on GitHub:** Follow PART 3 to deploy to Vercel
4. **Done!** Site is live

---

## **Need Help?**

- **GitHub docs:** docs.github.com
- **Vercel docs:** vercel.com/docs
- **Terminal stuck?** Press Ctrl+C to stop, then try again
- **Have questions?** Email poppet@sariko.app

---

## **Status**

✅ Code is ready  
✅ Community links are greyed out (will update later)  
✅ You have this deployment guide  
✅ Ready to go live  

**What's blocking you?**
- [ ] GitHub account?
- [ ] Vercel account?
- [ ] Terminal/command line?

Let me know and we'll get you unblocked.

---

**TL;DR:**
1. Create GitHub + Vercel accounts
2. Run git commands to upload to GitHub
3. Click "Deploy" in Vercel
4. Your site is live in 60 seconds
5. Share the URL

**Estimated time:** 30 minutes (first time). After that, updates take 1 minute (just push to GitHub, Vercel auto-deploys).
