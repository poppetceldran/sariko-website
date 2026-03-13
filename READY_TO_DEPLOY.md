# ✅ SariKo Website - Ready to Deploy Summary

---

## **What You Have**

A complete, production-ready Next.js website for SariKo.

**Status:** ✅ READY TO DEPLOY  
**Cost:** $0 (free Vercel tier)  
**Time to launch:** 30 minutes  

---

## **Final Updates Applied**

✅ Pricing tiers: FREE / Tindahan / Negosyo  
✅ 3-month free offer (not 6 months)  
✅ Teresa's revenue removed from card  
✅ Form link: link.zenapappro.com/sariko-icp  
✅ **Community buttons greyed out with "Coming Soon"** (you'll activate them later)  
✅ Email fallback: poppet@sariko.app  

---

## **Current Website Sections**

1. **Hero** — "Start free. 5 products, 3 months."
2. **Problem** — Invisible sellers, chaotic payments, lost orders
3. **Teresa's Story** — Founding Seller #1 (127 orders, 4.9★)
4. **Three Ways to Start** — FREE / Tindahan / Negosyo pricing
5. **How It Works** — Create → Discover → Grow
6. **Founder's Why** — Poppet's 30-year story + Zen Tech Asia
7. **Roadmap** — Q1-Q3 milestones + 3-month free mention
8. **Community** — Facebook/WhatsApp/Zalo (greyed out for now)
9. **Founding Seller Form** — Direct link to link.zenapappro.com/sariko-icp
10. **Buyer Waitlist** — Email capture
11. **Footer** — Zen Tech Asia + poppet@sariko.app

---

## **How to Deploy (3 Main Steps)**

### **STEP 1: Create Accounts (5 minutes)**

**GitHub (if you don't have):**
- Go to github.com
- Click "Sign up"
- Verify email

**Vercel:**
- Go to vercel.com
- Click "Sign up"
- Use "Continue with GitHub"

---

### **STEP 2: Upload to GitHub (10 minutes)**

**In your terminal/command prompt:**

```bash
cd /path/to/sariko-website
```

Then run these commands (copy-paste one by one):

```bash
git config --global user.email "your@email.com"
git config --global user.name "Your Name"
```

```bash
git init
git add .
git commit -m "Initial SariKo website - Phase 1"
git branch -M main
```

Then go to **github.com** → Click **+** → **New repository** → Name it `sariko-website` → Create

Then copy the commands GitHub shows and run them. Should look like:

```bash
git remote add origin https://github.com/YOUR_USERNAME/sariko-website.git
git push -u origin main
```

---

### **STEP 3: Deploy to Vercel (5 minutes)**

1. Go to **vercel.com** (logged in)
2. Click **"Add New"** → **"Project"**
3. Select `sariko-website` repo
4. Click **"Deploy"**
5. Wait ~60 seconds
6. **Copy the URL** — That's your live site

Example: `https://sariko-website.vercel.app`

---

## **Files to Reference**

| File | Purpose |
|------|---------|
| **DEPLOYMENT_STEPS.md** | 📖 READ THIS FIRST — Full step-by-step guide |
| **DEPLOY_CHECKLIST.md** | ✅ Quick checklist version |
| **UPDATES_MADE.md** | 📝 What changed from original version |
| **QUICK_START.md** | 🚀 5-minute quick reference |
| **README.md** | 📚 Complete overview of everything |

---

## **What Happens After Deploy**

### **Immediately (Day 1)**
- [ ] Share URL with Poppet: `https://sariko-website.vercel.app`
- [ ] Share with 5-10 early community members
- [ ] Test all buttons work
- [ ] Check on mobile phone

### **This Week**
- [ ] Share in Facebook groups (Filipino diaspora HCMC)
- [ ] Share in WhatsApp groups you're in
- [ ] Collect founding seller inquiries
- [ ] Monitor email signups (buyer form)

### **When You Create Groups**
- [ ] Create Facebook group for SariKo sellers
- [ ] Create WhatsApp group
- [ ] Create Zalo group
- [ ] Email me the URLs OR update code yourself
- [ ] Push to GitHub
- [ ] Vercel auto-deploys (buttons go live)

---

## **Community Links Update (For Later)**

When you create your groups:

**In code (around line 428), replace:**
```jsx
<button disabled>Facebook Group →</button>
```

With:
```jsx
<a href="https://facebook.com/groups/YOUR_ID">Facebook Group →</a>
```

Do the same for WhatsApp and Zalo. Then:

```bash
git add .
git commit -m "Add community links"
git push origin main
```

Vercel auto-deploys. Done.

---

## **Key Numbers**

**Founding Seller Benefits:**
- FREE tier: 5 items, $0/month, 18% commission
- Tindahan: $19/mo (FREE × 3 months), unlimited items, 16% commission
- Negosyo: $39/mo (FREE × 3 months), unlimited items, 14% commission
- **All founding sellers lock in these rates forever**

**Form Link:**
- Founding Seller applications: link.zenapappro.com/sariko-icp
- Buyer waitlist: (capture emails on website)

**Contact:**
- Email: poppet@sariko.app

---

## **Common Questions**

### **Q: Do I need to buy a domain?**
A: No, not yet. Use free `sariko-website.vercel.app` to launch. Later, you can get `sariko.zenapappro.com` (free subdomain) or buy `sariko.app` ($12/year).

### **Q: Will the site get traffic automatically?**
A: No, you need to share it. Send to Poppet, Facebook groups, WhatsApp, Zalo. Then organic growth from founding sellers telling others.

### **Q: What if I want to change something after deploying?**
A: Edit the code → `git add . && git commit -m "message" && git push origin main` → Vercel auto-deploys in 60 seconds.

### **Q: Can I test locally before deploying?**
A: Yes! Run `npm install` then `npm run dev` → Visit http://localhost:3000 → Test everything → Then deploy.

### **Q: What if something breaks?**
A: All your code is on GitHub. You can revert to previous version anytime. Also, Vercel keeps 50+ old deployments. Easy to rollback.

---

## **Deployment Confidence Checklist**

Before you deploy, make sure:

- [ ] GitHub account created (github.com)
- [ ] Vercel account created (vercel.com)
- [ ] Terminal/Command Prompt working
- [ ] Project folder on your computer
- [ ] Have 30 minutes free
- [ ] DEPLOYMENT_STEPS.md is open for reference

If all checked: **You're ready to deploy.**

---

## **Support**

**Before deploying:**
- Read DEPLOYMENT_STEPS.md (covers 90% of questions)
- It has troubleshooting section

**After deploying:**
- Vercel docs: vercel.com/docs
- Next.js docs: nextjs.org/docs
- GitHub docs: github.com/docs

**Still stuck?**
- Email: poppet@sariko.app
- Share error message you're getting

---

## **Timeline**

| Step | Time | What |
|------|------|------|
| 1 | 5 min | Create GitHub + Vercel accounts |
| 2 | 10 min | Upload code to GitHub (git commands) |
| 3 | 5 min | Click "Deploy" in Vercel |
| 4 | 1 min | Wait for build |
| 5 | 1 min | Get live URL |
| **Total** | **~30 min** | **Site is LIVE** |

---

## **What You'll Get**

✅ Live website at `https://sariko-website.vercel.app`  
✅ Auto-deploys when you push to GitHub  
✅ Mobile-optimized  
✅ Fast (edge caching)  
✅ Free SSL certificate (https://)  
✅ 99.9% uptime  
✅ Easy to update  

---

## **Next Phase (After Deploy)**

1. **Share & collect sellers** — Use founding seller form
2. **Build email list** — Use buyer waitlist form
3. **Activate community groups** — When ready, add links
4. **Iterate** — Add new sellers, testimonials, update copy
5. **Scale** — More sellers, bigger reach, prepare for launch

---

## **You're Ready**

Everything is done. Code is ready. Guide is clear. 

**Next action:** 
1. Open DEPLOYMENT_STEPS.md
2. Follow the steps
3. Deploy
4. Share the URL

**That's it. You got this.** 🚀

---

**Current Status:**
✅ Website built  
✅ Pricing tiers finalized  
✅ Community links greyed out (ready to activate later)  
✅ Form link integrated  
✅ Deployment guide complete  
✅ Ready to go live  

**Blocked on:** Nothing. Go deploy.

---

*"Ang iyong tindahan, para sa ating lahat" — Your store, for all of us*
