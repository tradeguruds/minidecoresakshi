# Mini Decor — Website (by Sakshi Wagh)

A simple one-page website for Mini Decor's handmade woolen crafts, with:
- WhatsApp ordering (auto-filled message per product)
- UPI payment QR code
- Instagram link

This is a **static website** — just one file (`index.html`). No server, no database, nothing to install. That makes it very easy to publish for free using **GitHub Pages**.

---

## 🚀 How to publish this on GitHub Pages (free)

### Step 1 — Create a GitHub account
Go to [github.com](https://github.com) and sign up (skip if you already have an account).

### Step 2 — Create a new repository
1. Click the **+** icon (top-right) → **New repository**
2. Name it something like `mini-decor-website`
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload the files
1. On your new repo page, click **Add file** → **Upload files**
2. Drag and drop `index.html` (and `README.md`) from this folder
3. Click **Commit changes**

### Step 4 — Turn on GitHub Pages
1. In your repo, go to **Settings** → **Pages** (left sidebar)
2. Under **Branch**, choose `main` and folder `/ (root)`
3. Click **Save**
4. Wait ~1 minute, then refresh — GitHub will show your live link, something like:

```
https://your-username.github.io/mini-decor-website/
```

That link is your live website. Share it anywhere — Instagram bio, WhatsApp status, etc.

---

## ✏️ How to edit the website later

Everything you'll want to change lives near the bottom of `index.html`, inside the `<script>` tag, clearly marked:

```js
const PHONE = "918888040240";      // WhatsApp number
const UPI_ID = "8888040240@upi";   // Real UPI ID goes here
const PAYEE_NAME = "Sakshi Wagh";

const PRODUCTS = [
  { name: "Crochet Flower Bouquet", desc: "...", price: "₹499", ... },
  ...
];
```

**To make a change:**
1. On GitHub, open `index.html` in your repo
2. Click the ✏️ pencil icon (top-right) to edit
3. Find the part you want to change, edit it
4. Scroll down, click **Commit changes**
5. Your live site updates automatically in under a minute

### Things you'll likely want to update:
| What | Where |
|---|---|
| Real UPI ID (e.g. `sakshiwagh@okhdfcbank`) | `UPI_ID` |
| WhatsApp number | `PHONE` |
| Product names, prices, descriptions | `PRODUCTS` list |
| Real product photos | add `img: "photo-link.jpg"` inside a product's `{ }` — see note below |

### Adding real photos
Right now products show simple hand-drawn icons since there are no real photos yet. To add a real photo:
1. Upload the photo to your GitHub repo (e.g. into a new `images` folder)
2. In `PRODUCTS`, set `img: "images/bouquet.jpg"` for that item — it will replace the icon automatically

---

## 📁 Files in this project

```
mini-decor-website/
├── index.html    → the entire website (HTML + CSS + JS in one file)
└── README.md      → this guide
```

---

## ⚠️ Before going fully live
- [ ] Replace the placeholder `UPI_ID` with Sakshi's real UPI ID
- [ ] Double check the WhatsApp number is correct
- [ ] Update product prices to real, final prices
- [ ] Add real product photos when available
