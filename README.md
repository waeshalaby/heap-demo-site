# Heap Demo Site (3 static pages)

This is a minimal website to practice Heap setup, tagging (visual labeling), and basic analyses.

## Files
- `index.html` — Home page
- `product.html` — Product page with "Add to Cart"
- `checkout.html` — Checkout page with a fake form
- `styles.css` — Minimal styling

---

## 1) Insert your Heap snippet

1. Sign up for Heap (trial/free) and create a project to get your **App ID**.
2. In Heap > Project Settings > Install, copy the **JavaScript snippet**.
3. Replace the placeholder snippet block in **all three HTML files**:
   - Find: `<!-- HEAP SNIPPET: paste your script here -->`
   - Paste your actual snippet **inside the <head>** element.

> Tip: The standard Heap snippet looks like a small JS block calling `window.heap.load("YOUR_APP_ID")`.

---

## 2) Local test

Just double-click `index.html` to open in your browser and click around.  
Heap will autocapture your interactions, but **some browsers may block local file referrer/host headers**.
For the most realistic data, deploy to a real URL (see below).

---

## 3) Deploy options

### Option A — GitHub Pages (free)
1. Create a new public repo (e.g., `heap-demo-site`).
2. Upload these four files.
3. In GitHub, go to **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: **main** / root
4. Wait ~1–2 minutes. Your site will be live at:
   `https://<your-username>.github.io/heap-demo-site/`

### Option B — Netlify (free)
1. Go to netlify.com and log in.
2. Drag & drop this folder into Netlify.
3. It will auto-deploy and give you a URL like:
   `https://your-site-name.netlify.app/`

### Option C — Vercel (free)
1. Create a new project.
2. Import your GitHub repo.
3. Deploy.

---

## 4) What to tag in Heap (Visual Labeling)

Open Heap → Launch **Visual Labeling** on your deployed site URL and tag:

- `Add to Cart` button on `product.html` as **AddToCart_Click**
- `Checkout` link on `product.html` as **Checkout_Click**
- `Place Order` button on `checkout.html` as **PlaceOrder_Submit**
- Optional: text field interactions on `checkout.html`

---

## 5) Suggested analyses

### Funnel
`Viewed Product (product.html)` → `AddToCart_Click` → `Checkout_Click` → `PlaceOrder_Submit`

### Journeys
- After `AddToCart_Click`, see common next steps.
- Before `PlaceOrder_Submit`, see detours.

### Retention (optional)
- Use `PlaceOrder_Submit` as the returning action if you revisit on multiple days.

---

## 6) Notes
- This site is purposely simple: no frameworks, no build step.
- You can customize text, images, and links freely.
- If you want SPA routing later, start with this then move to a router-based demo.
