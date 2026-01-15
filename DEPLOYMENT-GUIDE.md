# The Supply Store - Website Deployment Guide

## 📁 Your Website Files

Your complete website consists of:
- **index.html** - Home page with enquiry form and location map
- **products.html** - Products page with shade card
- **about.html** - About page with leadership team
- **dealerships.html** - Dealerships page
- **styles.css** - All styling
- **script.js** - Interactive features
- **logo.png** - Your company logo
- **shade-card.pdf** - Product shade card

## 🚀 Deployment Options (All FREE)

### **Option 1: GitHub Pages (RECOMMENDED - Easiest)**

#### Step 1: Create GitHub Account
1. Go to https://github.com
2. Click "Sign up" and create a free account
3. Verify your email address

#### Step 2: Create New Repository
1. Click the "+" icon in top right → "New repository"
2. Name it: `the-supply-store`
3. Make it **Public**
4. DON'T check "Add a README file"
5. Click "Create repository"

#### Step 3: Upload Your Files
**Easy Method (No Command Line):**
1. On your repository page, click "uploading an existing file"
2. Drag ALL your website files into the upload area:
   - index.html
   - products.html
   - about.html
   - dealerships.html
   - styles.css
   - script.js
   - logo.png
   - shade-card.pdf
3. Scroll down and click "Commit changes"

#### Step 4: Enable GitHub Pages
1. Go to your repository settings (Settings tab)
2. Click "Pages" in the left sidebar
3. Under "Source", select "main" branch
4. Click "Save"
5. Wait 2-3 minutes
6. Your site will be live at: `https://[your-username].github.io/the-supply-store/`

---

### **Option 2: Netlify (Also Very Easy)**

#### Step 1: Sign Up
1. Go to https://www.netlify.com
2. Click "Sign up" → Sign up with GitHub (or email)

#### Step 2: Deploy
1. After logging in, click "Add new site" → "Deploy manually"
2. Create a folder on your computer with ALL your website files
3. Drag the entire folder into the Netlify upload area
4. Wait 30 seconds
5. Your site is live! Netlify gives you a URL like: `random-name-123.netlify.app`

#### Step 3: Custom Domain (Optional)
1. Click "Domain settings"
2. You can change the subdomain to: `the-supply-store.netlify.app`
3. Or add your own custom domain if you buy one

---

### **Option 3: Vercel**

#### Steps:
1. Go to https://vercel.com
2. Sign up with GitHub
3. Click "Add New" → "Project"
4. Import your GitHub repository (from Option 1)
5. Click "Deploy"
6. Done! Your site is live

---

## 🔧 Before Deploying - Important Updates

### 1. Update WhatsApp Number
In **index.html**, find this line (around line 100):
```html
<a href="https://wa.me/YOUR_WHATSAPP_NUMBER" class="chat-link" target="_blank">
```
Replace `YOUR_WHATSAPP_NUMBER` with your actual WhatsApp number (with country code, no + or spaces).
Example: `https://wa.me/919876543210`

### 2. Update Google Maps (Optional)
The current map iframe has a placeholder. To update:
1. Go to https://www.google.com/maps
2. Search for: "The Supply Store, Changodar, Ahmedabad"
3. Click "Share" → "Embed a map"
4. Copy the iframe code
5. Replace the iframe in **index.html** (around line 170)

### 3. Add Your Contact Information
Add phone numbers, email addresses where you see comments in the HTML files.

---

## 📱 Testing Your Site Locally

Want to see how it looks before deploying?

### Method 1: Just Open the File
1. Find your `index.html` file
2. Right-click → "Open with" → Choose your web browser
3. Click through the navigation to test all pages

### Method 2: Use a Local Server (Better)
If you have Python installed:
```bash
# Open terminal/command prompt in your website folder
python -m http.server 8000
# Then visit: http://localhost:8000
```

---

## 🎨 Customization Tips

### Change Colors
Edit **styles.css**, find these lines at the top:
```css
:root {
    --navy-blue: #0B2C4D;
    --business-gold: #C6A24A;
    --white: #FFFFFF;
}
```

### Update Content
- Company name, descriptions → Edit the HTML files
- Add more products → Add to `products.html`
- Change team info → Edit `about.html`

---

## 📧 Form Submissions

**Important:** The forms currently show an alert message. To actually receive form submissions, you need to:

### Option A: Use a Form Service (FREE)
1. **Formspree** (https://formspree.io)
   - Sign up free
   - Get your form endpoint
   - Add to your forms

2. **Netlify Forms** (if you deploy on Netlify)
   - Add `netlify` attribute to your forms
   - Submissions appear in Netlify dashboard

### Option B: Google Forms
Create Google Forms and link to them from your contact buttons

---

## ✅ Checklist Before Going Live

- [ ] Updated WhatsApp number
- [ ] Updated Google Maps embed
- [ ] Tested all pages locally
- [ ] All images loading correctly
- [ ] Forms work (show alert or submit somewhere)
- [ ] All links work
- [ ] Mobile responsive (test on phone)
- [ ] Checked spelling/grammar

---

## 🆘 Troubleshooting

### Images not showing?
- Make sure `logo.png` is in the same folder as your HTML files
- Check that filenames match exactly (case-sensitive)

### Styles not applying?
- Ensure `styles.css` is in the same folder
- Check browser console for errors (F12 → Console tab)

### Pages not linking?
- Make sure all HTML files are in the same folder
- Check that filenames are exactly: `index.html`, `products.html`, `about.html`, `dealerships.html`

---

## 📞 Need Help?

If you get stuck:
1. Check the browser console (F12) for error messages
2. Make sure all files are in the same folder
3. Try the "Open with browser" method first to test

---

## 🎉 You're All Set!

Your professional paint supply website is ready to launch. Choose your deployment method and you'll be live in minutes!

**Recommended Path:**
1. Test locally by opening `index.html` in browser
2. Update WhatsApp number and any other details
3. Deploy to GitHub Pages (easiest)
4. Share your new website URL!

Good luck! 🚀
