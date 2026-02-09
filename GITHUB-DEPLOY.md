# 🚀 GitHub Deployment Instructions

Follow these simple steps to deploy PromptVault to GitHub Pages (FREE hosting!)

## 📦 Files to Upload to GitHub

You need these **4 essential files:**

1. ✅ **index.html** - Landing page (redirects to gallery)
2. ✅ **gallery.html** - Main public gallery  
3. ✅ **admin.html** - Admin panel
4. ✅ **README.md** - Project documentation

**Optional (but recommended):**
5. LICENSE - MIT license
6. .gitignore - Git ignore rules

---

## 🎯 Step-by-Step Deployment

### Option 1: GitHub Website (Easiest - No Git Knowledge Required)

#### Step 1: Create GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Create free account

#### Step 2: Create New Repository
1. Click the **+** icon (top-right)
2. Select **"New repository"**
3. Repository name: `promptvault` (lowercase, no spaces)
4. Description: "AI Image Prompt Gallery"
5. Choose **Public**
6. ✅ Check "Add a README file"
7. Click **"Create repository"**

#### Step 3: Upload Files
1. In your new repo, click **"Add file"** → **"Upload files"**
2. Drag and drop these files:
   - `index.html`
   - `gallery.html`
   - `admin.html`
   - `README.md`
   - `LICENSE` (optional)
3. Scroll down
4. Type commit message: "Initial commit - PromptVault v1.0"
5. Click **"Commit changes"**

#### Step 4: Enable GitHub Pages
1. Click **"Settings"** tab (in your repo)
2. Scroll down to **"Pages"** (left sidebar)
3. Under "Source":
   - Branch: Select **"main"**
   - Folder: Select **"/ (root)"**
4. Click **"Save"**
5. Wait 1-2 minutes

#### Step 5: Get Your Live URL
1. Refresh the Settings → Pages
2. You'll see: **"Your site is live at https://yourusername.github.io/promptvault/"**
3. Click the link to view your site!

---

### Option 2: Using Git (For Developers)

If you know Git commands:

```bash
# Navigate to your folder with the files
cd /path/to/promptvault

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - PromptVault v1.0"

# Add remote (replace YOUR-USERNAME)
git remote add origin https://github.com/YOUR-USERNAME/promptvault.git

# Push to GitHub
git push -u origin main
```

Then enable Pages in Settings (same as Option 1, Step 4).

---

## 🔧 Before You Deploy - Important!

### 1. Change Admin Password ⚠️

**Open `admin.html` and find this (around line 470):**
```javascript
const ADMIN_CREDENTIALS = {
    username: 'admin',
    password: 'admin123'  // ⚠️ CHANGE THIS NOW!
};
```

**Change to something secure:**
```javascript
const ADMIN_CREDENTIALS = {
    username: 'admin',
    password: 'MySecurePass123!'  // ✅ Much better!
};
```

### 2. Update Donation Link

**Open `gallery.html` and find this (around line 845):**
```html
<a href="https://www.buymeacoffee.com/yourusername" target="_blank" class="buy-egg-btn">
```

**Change to your Ko-fi/BMAC link:**
```html
<a href="https://ko-fi.com/yourname" target="_blank" class="buy-egg-btn">
```

### 3. Customize Branding (Optional)

**In `gallery.html`, find:**
```html
<div class="logo-text">PromptVault</div>
```

**Change to your site name:**
```html
<div class="logo-text">YourSiteName</div>
```

---

## 🎯 Your Live URLs

After deployment, your site will be at:

- **Homepage:** `https://yourusername.github.io/promptvault/`
- **Gallery:** `https://yourusername.github.io/promptvault/gallery.html`
- **Admin:** `https://yourusername.github.io/promptvault/admin.html`

**Note:** Replace `yourusername` with your actual GitHub username!

---

## 🔄 How to Update Your Site

### Method 1: GitHub Website
1. Go to your repo
2. Click on the file you want to edit
3. Click the ✏️ pencil icon
4. Make changes
5. Scroll down, click "Commit changes"
6. Changes go live in 1-2 minutes!

### Method 2: Upload New Version
1. Go to your repo
2. Click "Add file" → "Upload files"
3. Select the updated file
4. Check "Replace existing file"
5. Commit changes

### Method 3: Git Command Line
```bash
# Make your changes to files
# Then:
git add .
git commit -m "Updated prompts"
git push
```

---

## 🎨 Adding Your First Prompts

1. Go to: `https://yourusername.github.io/promptvault/admin.html`
2. Login with your password
3. Fill the form:
   - **Image URL:** Get from Unsplash.com
     - Go to unsplash.com
     - Find an image
     - Right-click → "Copy image address"
     - Paste the URL
   - **Prompt Text:** Describe the image
   - **Tags:** cyberpunk, neon, city (comma-separated)
   - **Likes:** 0 (or any starting number)
4. Click "Add Prompt"
5. View in gallery instantly!

---

## 📱 Share Your Site

Once live, share these links:

**For Users (Public):**
- `https://yourusername.github.io/promptvault/`

**For You Only (Admin):**
- `https://yourusername.github.io/promptvault/admin.html`
- ⚠️ Don't share this link publicly!

---

## 🎉 Post-Launch Checklist

After your site is live:

- [ ] Test gallery on mobile
- [ ] Test admin panel login
- [ ] Add 10+ sample prompts
- [ ] Test search functionality
- [ ] Test like button
- [ ] Verify donation link works
- [ ] Share on social media!

---

## 🐛 Troubleshooting

### "404 Not Found"
- Wait 2-3 minutes after enabling Pages
- Check Settings → Pages shows "Your site is published"
- Make sure you pushed all files

### "Admin login not working"
- Check you changed the password correctly
- Clear browser cache (Ctrl+Shift+Delete)
- Try incognito/private window

### "Images not loading"
- Check image URLs are publicly accessible
- Try opening image URL directly in browser
- Use https:// URLs, not http://

### "Changes not showing"
- Wait 1-2 minutes for GitHub Pages to update
- Clear browser cache
- Try hard refresh (Ctrl+Shift+R)

---

## 🚀 Next Steps

1. **Deploy** - Follow steps above (15 minutes)
2. **Add Content** - Upload 20+ prompts (1 hour)
3. **Share** - Post on Reddit, Twitter (ongoing)
4. **Monetize** - Add AdSense after 1,000 visitors

---

## 💡 Pro Tips

### 1. Custom Domain (Optional)
Want `yoursite.com` instead of GitHub URL?

1. Buy domain from Namecheap ($10/year)
2. In GitHub Settings → Pages
3. Add custom domain
4. Update DNS settings (GitHub shows instructions)

### 2. Free SSL
GitHub Pages includes free HTTPS automatically! ✅

### 3. Analytics
Add Google Analytics:
1. Sign up at analytics.google.com
2. Get tracking code
3. Add to `gallery.html` in `<head>` section

### 4. SEO
Already optimized! Your site has:
- ✅ Proper meta tags
- ✅ Semantic HTML
- ✅ Fast loading
- ✅ Mobile-friendly

---

## 📊 File Sizes

All files are lightweight:
- index.html: ~1 KB
- gallery.html: ~45 KB
- admin.html: ~30 KB
- README.md: ~8 KB

**Total:** Less than 100 KB! Super fast! ⚡

---

## ❓ Common Questions

**Q: Is GitHub Pages really free?**
A: Yes! 100% free forever for public repos.

**Q: Can I use my own domain?**
A: Yes! Add custom domain in Settings.

**Q: How many visitors can I have?**
A: GitHub recommends under 100GB bandwidth/month (plenty for most sites!)

**Q: Can I make the repo private?**
A: Yes, but you need GitHub Pro for Pages on private repos.

**Q: How do I backup my data?**
A: Use admin panel "Export Data" button to download JSON.

---

## 🎯 Summary

**Deploy Steps:**
1. Create GitHub account
2. Create new repo "promptvault"
3. Upload 4 files
4. Enable Pages in Settings
5. Wait 2 minutes
6. Site is live! 🎉

**Time needed:** 15 minutes total

**Cost:** $0 (completely free!)

---

## 🆘 Need Help?

If you get stuck:
1. Check Troubleshooting section above
2. Read GitHub Pages docs: [docs.github.com/pages](https://docs.github.com/pages)
3. Ask in GitHub Discussions

---

## 🎊 You're Ready!

Your PromptVault site will be live at:
**`https://yourusername.github.io/promptvault/`**

Now go deploy it! 🚀

---

**Built with ❤️ and lots of 🥚**
