# All-You-Need — Free Deployment Guide

Your website is a single `index.html` file — no server, no database needed.
Products are saved in the browser's localStorage so they persist across visits on the same device/browser.

---

## 🔐 Change Your Admin Password (Important!)

Before deploying, open `index.html` in a text editor and find this line near the top of the `<script>` section:

```js
const ADMIN_PASSWORD = 'admin@AYN2026';
```

Change it to your own strong password. Example:
```js
const ADMIN_PASSWORD = 'MySecretPass#99';
```

---

## 🚀 Option 1 — Netlify (Recommended, Easiest)

**Steps:**
1. Go to https://netlify.com and sign up for free
2. Click **"Add new site"** → **"Deploy manually"**
3. Drag and drop your `index.html` file (or the whole folder) into the deploy box
4. Netlify gives you a free URL like `https://all-you-need.netlify.app`
5. Optionally connect a custom domain (e.g. allyouneed.in) for free

**Custom domain:** Settings → Domain management → Add custom domain

---

## 🚀 Option 2 — GitHub Pages (Also Free)

**Steps:**
1. Go to https://github.com and create a free account
2. Click **"New repository"** → name it `all-you-need`
3. Upload your `index.html` file
4. Go to **Settings → Pages → Source → Deploy from branch → main**
5. Your site is live at `https://yourusername.github.io/all-you-need`

---

## 🚀 Option 3 — Vercel (Very Fast)

**Steps:**
1. Go to https://vercel.com and sign up
2. Click **"New Project"** → **"Continue with GitHub"** (connect your GitHub repo from Option 2)
3. Click Deploy — done!
4. Free URL: `https://all-you-need.vercel.app`

---

## 🛠 How to Use the Admin Panel

1. Click **"⚙ Admin"** in the top navigation bar
2. Enter your admin password
3. You'll see the Admin Panel with:
   - **Add Product form** — fill name, price, description, category, background style, emoji icon
   - **Product list** — edit or delete any existing product
4. Products are automatically saved in the browser
5. Click **"← Back to Store"** to return to the shop

> **Note:** Products are stored in the browser's localStorage. They will persist on the same browser/device. If you want products to be shared across devices, you would need a backend (e.g. Firebase — ask for help upgrading!).

---

## 📱 Device Compatibility

The website works on:
- ✅ Mobile phones (iOS & Android)
- ✅ Tablets (iPad, Android tablets)
- ✅ Laptops & Desktops
- ✅ All modern browsers (Chrome, Safari, Firefox, Edge)

---

## 📋 Files in This Package

```
allyouneed/
├── index.html          ← Your entire website (deploy this!)
└── DEPLOY_GUIDE.md     ← This file
```

---

## 💡 Quick Tips

- To update contact details (phone, email, address), open `index.html` and search for `hello@allyouneed.in` or `+91 98765 43210` and replace with your real info
- To update your Pinterest handle, search for `@allyouneed.decor`
- To change the brand name, search for `All-You-Need`

---

Made with ❤️ by Claude for All-You-Need | Pune, Maharashtra
