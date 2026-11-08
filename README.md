# 🌟 UNICO - All-in-One Affiliate Deals & Monetization Platform

> **UNICO** is a high-converting, modern, multi-category affiliate deals platform. It connects shoppers with handpicked, verified bargains across **Fashion, Household & Living, DIY & Tools, Tech & Gadgets, and Beauty** from global marketplaces (**Amazon, Flipkart, Myntra, Etsy, AliExpress, Walmart**).

---

## 🚀 Key Features

- **Multi-Niche Aggregator**: Curated collections for Fashion & Streetwear, Household & Smart Living, DIY Tools & Crafting, Tech Gadgets, and Beauty & Wellness.
- **Multi-Store Support**: Pre-styled platform tags and colors for Amazon, Flipkart, Myntra, Etsy, AliExpress, and Walmart.
- **Deal of the Day Hero Banner**: Interactive flash deal showcase with a live ticking countdown timer.
- **1-Click Coupon Code Copy**: Built-in coupon badges with one-click clipboard copy and toast notifications.
- **Live Search & Smart Filtering**: Real-time search across product titles, descriptions, stores, and categories with instant results.
- **Saved Deals / Wishlist**: LocalStorage-powered wishlist drawer allowing shoppers to save deals and return later.
- **Built-in Curator / Admin Panel**:
  - Add new affiliate deals in seconds with custom pricing, discount calculation, image URL, and affiliate tracking URL.
  - Edit or delete existing deals.
  - **Export JSON**: Download updated product databases to commit to your repository.
  - **Import JSON**: Bulk-load deal catalogs instantly.
  - Track total affiliate link referral clicks.
  - Passcode protected.
- **Dark Mode & Light Mode**: Smooth theme toggling with automatic OS preference detection.
- **FTC & Amazon Compliance**: Integrated affiliate disclosure badges and transparent disclaimers.
- **100% Zero-Build Deployable**: Ready to deploy in seconds to **Netlify, Vercel, GitHub Pages, or Cloudflare Pages** with zero npm dependencies.

---

## 📁 Project Structure

```
UNICO/
├── unico.html              # 🌟 All-in-one standalone single-file version (Open directly in any browser!)
├── index.html              # Modular production storefront entrypoint
├── css/
│   └── styles.css          # Premium styling, glassmorphism, shimmers, modals, and toasts
├── js/
│   ├── deals-data.js       # Curated database of 16+ verified high-discount deals & store styles
│   ├── app.js              # State management, search, filters, wishlist, modals, analytics
│   └── admin.js            # Deal Curator control panel (Add, Edit, Delete, Export, Import)
├── data/
│   └── deals.json          # Raw backup JSON of all deals for backend/batch editing
├── serve.py                # 1-click Python local development server
├── netlify.toml            # Zero-config deployment for Netlify
├── vercel.json             # Zero-config deployment for Vercel
└── README.md               # Complete setup, monetization, and deployment guide
```

---

## 💻 Instant Local Testing

You have two easy ways to run the website locally:

### Option 1: One-Click Python Server (Recommended)
Open your terminal in the `UNICO` directory and run:
```bash
python3 serve.py
```
This opens `http://localhost:8000` automatically in your default browser.

### Option 2: Standalone File
Double-click `unico.html` directly in Finder or open it in any web browser. It contains all code and styles self-contained in a single file!

---

## 🌐 Instant Free Deployment (2 Minutes)

### Method 1: Netlify Drop (Easiest - 30 Seconds, No Terminal Needed)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag and drop the `UNICO` folder into the browser window.
3. Your website is instantly live with a free custom SSL URL (e.g., `https://unico-deals.netlify.app`).

### Method 2: Vercel
1. Install Vercel CLI (or connect your GitHub repo at [vercel.com](https://vercel.com)):
   ```bash
   npx vercel
   ```
2. Press Enter to accept defaults. The pre-configured `vercel.json` ensures instant clean routing.

### Method 3: GitHub Pages
1. Push this folder to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial release of UNICO Deals Platform"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo-name>.git
   git push -u origin main
   ```
2. In your GitHub repository:
   - Go to **Settings** > **Pages**.
   - Under **Build and deployment** > **Branch**, select `main` and `/ (root)`.
   - Click **Save**. Your site will be live at `https://<your-username>.github.io/<your-repo-name>/`.

---

## 💰 How to Connect Your Own Affiliate Accounts

1. Open `js/deals-data.js` or use the **Admin Panel** on the live site:
   - Click the ⚙️ **Settings icon** in the top right header (Passcode: `akshay2906`).
   - Enter your curator passcode.
2. Replace the placeholder affiliate links with your affiliate tags:
   - **Amazon Associates**: Replace `?tag=unico-household-20` with your Amazon Associate Store ID.
   - **Flipkart Affiliate**: Add your `affid=...` parameter.
   - **Myntra / Cuelinks / EarnKaro**: Paste your customized deep links.
   - **AliExpress / Admitad**: Paste your tracking links.
3. Once you add or edit deals through the Admin Panel, click **"Export deals.json"** to download the updated JSON.

---

## 🔒 Security & Admin Configuration

- **Change Admin Passcode**: Open `js/admin.js` and update line 7:
  ```javascript
  const ADMIN_PASSCODE = "your_new_secret_password";
  ```
- **Click Tracking**: Every time a user clicks **"Grab Deal"**, the click count is saved in local browser analytics and displayed in the curator panel.

---

## 📄 License
MIT License. Created for the UNICO affiliate program.
