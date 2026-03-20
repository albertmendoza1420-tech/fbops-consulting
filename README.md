# FB Ops Consulting — Website

A complete 3-page website ready to deploy on **GitHub Pages** for free.

---

## 📁 File Structure

```
fbops-site/
├── index.html           ← Homepage (hero, services, team, process, pricing)
├── portfolio.html       ← Portfolio gallery + case studies
├── contact.html         ← Inquiry form + contact details
├── assets/
│   ├── css/
│   │   └── style.css    ← All styles
│   ├── js/
│   │   └── main.js      ← All JavaScript
│   └── images/          ← Put your photos here
│       ├── albert.jpg   ← Albert's team photo
│       ├── chris.jpg    ← Chris's team photo
│       ├── jimuel.jpg   ← Chef Jimuel's team photo
│       └── (gallery photos...)
└── README.md
```

---

## 🚀 Step-by-Step: Deploy to GitHub Pages (FREE)

### Step 1 — Create a GitHub account
Go to **github.com** → Sign Up (free). Use your email.

### Step 2 — Create a new repository
1. Click the **+** icon (top right) → **New repository**
2. Name it exactly: `fbops-consulting` (or any name you like)
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload your files
1. On the new repository page, click **uploading an existing file**
2. Drag and drop the entire `fbops-site` folder contents (all files and the `assets` folder)
3. Write a commit message: "Initial site upload"
4. Click **Commit changes**

### Step 4 — Enable GitHub Pages
1. Go to your repository → click **Settings** (top menu)
2. Scroll down to **Pages** in the left sidebar
3. Under "Source", select **Deploy from a branch**
4. Select branch: **main** | Folder: **/ (root)**
5. Click **Save**

### Step 5 — Your site is live! 🎉
Wait ~2 minutes, then visit:
```
https://YOUR-GITHUB-USERNAME.github.io/fbops-consulting/
```

---

## ✏️ Personalisation Checklist

Open each file in any text editor (Notepad, VS Code, etc.) and replace:

### In ALL files:
- [ ] `966XXXXXXXXX` → Your WhatsApp number (no + sign, e.g. `966501234567`)
- [ ] `hello@fbopsconsulting.com` → Your real email
- [ ] `+966 XX XXX XXXX` → Your WhatsApp display number
- [ ] `linkedin.com/in/yourprofile` → Your LinkedIn URL
- [ ] `© 2026 FB Ops Consulting` → Your actual business name

### In contact.html:
- [ ] `YOUR_FORMSPREE_ID` → Your Formspree form ID (see below)

### In index.html:
- [ ] Update the hero stats numbers if needed
- [ ] Update pricing if needed

---

## 📸 Adding Team Photos

1. Save your photos as `albert.jpg`, `chris.jpg`, `jimuel.jpg`
2. Place them in `assets/images/`
3. In `index.html`, find each team card and replace:

```html
<!-- BEFORE (placeholder) -->
<div class="team-photo-placeholder">
  <div class="team-initials">AM</div>
  ...
</div>

<!-- AFTER (with real photo) -->
<img src="assets/images/albert.jpg" alt="Albert Mendoza">
```

Do the same for Chris and Chef Jimuel.

---

## 📸 Adding Portfolio Photos

1. Name your photos clearly: `cheese-01.jpg`, `bread-sourdough.jpg`, etc.
2. Place them in `assets/images/`
3. In `portfolio.html`, find each gallery item and:
   - Add `data-src="assets/images/your-photo.jpg"` to the div
   - Replace the placeholder div with `<img src="assets/images/your-photo.jpg" alt="Description">`

Example:
```html
<!-- BEFORE -->
<div class="gallery-item" data-cat="cheese" data-src="" data-caption="Artisan Cheese Platter">
  <div class="gallery-placeholder">...</div>
  ...
</div>

<!-- AFTER -->
<div class="gallery-item" data-cat="cheese" data-src="assets/images/cheese-01.jpg" data-caption="Artisan Cheese Platter">
  <img src="assets/images/cheese-01.jpg" alt="Artisan Cheese Platter">
  ...
</div>
```

---

## 📬 Setting Up the Inquiry Form (Formspree — FREE)

Formspree sends all form submissions directly to your email. Setup takes 2 minutes:

1. Go to **formspree.io** → Create a free account
2. Click **+ New Form**
3. Name it "FB Ops Inquiry" and enter your email
4. You'll get an endpoint like: `https://formspree.io/f/abcdefgh`
5. Copy just the ID part: `abcdefgh`
6. In `contact.html`, find this line:
   ```html
   action="https://formspree.io/f/YOUR_FORMSPREE_ID"
   ```
7. Replace `YOUR_FORMSPREE_ID` with your actual ID:
   ```html
   action="https://formspree.io/f/abcdefgh"
   ```
8. Save and re-upload to GitHub

That's it — all inquiries go straight to your email.

---

## 🌐 Getting a Custom Domain (Optional)

Instead of `github.io/fbops-consulting`, you can use `yourname.com`:

1. Buy a domain at **Namecheap** (~$10–15/year for `.com`)
   - Good options: `albertmendoza.com`, `fbopsconsulting.com`, `lolivo-ops.com`
2. In your domain registrar, add a CNAME record:
   - Name: `www`
   - Value: `YOUR-USERNAME.github.io`
3. In GitHub Pages settings, add your custom domain
4. GitHub handles the HTTPS certificate automatically (free)

---

## 🔄 Updating the Site Later

To update any content:
1. Edit the HTML file on your computer
2. Go to your GitHub repository
3. Click the file → click the pencil edit icon → paste your changes
4. OR: drag and drop the updated file to upload

Changes go live within 1–2 minutes.

---

## 📞 Need Help?

If you get stuck at any step, send a WhatsApp message to your own consultant — or ask Claude to help with specific parts!
