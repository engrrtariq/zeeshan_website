# Zeeshan Ali Security — Bodyguard Website

A fast, SEO-optimized static website for **Zeeshan Ali Security Services**.
Based in Karachi, serving all over Pakistan.

Built with plain HTML, CSS, and a tiny bit of JavaScript — no frameworks, no build step.

## What's in this site

- **4 pages**: Home, Services, About, Contact
- **Custom logo**: Gold shield with "ZA" monogram + wordmark (SVG, scales perfectly)
- **Click-to-call** everywhere: `tel:+923053199282`
- **WhatsApp deep links**: pre-filled message → opens chat directly
- **Local SEO**: LocalBusiness schema, multi-region areaServed (Pakistan + cities)
- **Mobile-first**: sticky floating call button on phones
- **Coverage section**: clearly shows Sindh, Balochistan, Punjab, KPK reach
- **Contact form**: FormSubmit → emails `zeeshankaleri328@gmail.com`

## Pre-filled details

| Field | Value |
|---|---|
| Name | Zeeshan Ali |
| Phone | +92 305 3199282 |
| Email | zeeshankaleri328@gmail.com |
| Base city | Karachi |
| Service area | All Pakistan (Sindh, Balochistan, Punjab, KPK) |
| Planned domain (SEO) | `zeeshanalisecurity.com` *(update meta/sitemap when you register)* |

## File structure

```
/
├── index.html          ← Homepage with coverage map
├── services.html       ← 5 services + pricing
├── about.html          ← Bio, credentials, code of conduct
├── contact.html        ← Call/WhatsApp/Email + form
├── robots.txt          ← Search engine instructions
├── sitemap.xml         ← Helps Google index every page
├── .nojekyll           ← Tells GitHub Pages not to run Jekyll (static files as-is)
├── site.webmanifest    ← PWA / Add-to-Home-Screen
├── css/style.css       ← All styles
├── js/main.js          ← Mobile menu + smooth scroll
└── assets/
    ├── favicon.svg     ← Browser tab icon (ZA shield)
    └── logo.svg        ← Full logo for sharing/email signature
```

---

## How to preview locally

Pick **one** of these in Terminal (you have both Python and Node already installed):

```bash
cd ~/Desktop/zeeshan
python3 -m http.server 8000
```

Or:

```bash
cd ~/Desktop/zeeshan
npx serve
```

Then open **http://localhost:8000** (or whatever port it shows).

To preview on your phone (same WiFi):
```bash
ipconfig getifaddr en0   # gives your Mac's IP
```
Then on your phone visit `http://<that-ip>:8000` — best way to feel the mobile UX.

---

## Optional next steps

### 1. Custom domain (~$10/year)

SEO URLs use `zeeshanalisecurity.com`. When you register a domain, connect it in your host's dashboard and, if the name changes, update `canonical` links, `sitemap.xml`, and JSON-LD in the HTML files.

### 2. Contact form (first-time setup)

The form uses **FormSubmit** and delivers to `zeeshankaleri328@gmail.com`. On the **first** submission, FormSubmit sends a **confirmation link** to that inbox — open it once so future enquiries go through.

### 3. Small edits anytime

- **About:** Personal note is in `about.html`.
- **Pricing:** Three cards in `services.html`.
- **Images:** Compress JPEGs at [squoosh.app](https://squoosh.app). For rich WhatsApp/Facebook previews, use a **1200×630** image and point each page's `og:image` meta tag at it.

---

## Deploy (free, 5 minutes)

### Option A: Cloudflare Pages (recommended)

1. Push this folder to a GitHub repo, OR use Cloudflare's drag-and-drop.
2. Go to https://pages.cloudflare.com → **Create Project**
3. Connect repo (or drag the folder), click **Deploy**
4. Free URL like `zeeshan-ali-security.pages.dev` works instantly
5. To use a real domain: Custom Domains → add domain → follow DNS steps

### Option B: Netlify

Drag-and-drop this folder onto https://app.netlify.com/drop → done.

### Option C: GitHub Pages

1. Create a repo on GitHub and push this project (`main` branch).
2. **Settings → Pages** → **Build and deployment**: Source = **Deploy from a branch**, Branch = **`main`** → folder **`/ (root)`** → Save.
3. After ~1–2 minutes the site is live at **`https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`**.

This repo uses **relative paths** for navigation, favicon, and manifest so it works both on that URL and on a **custom domain** (e.g. `zeeshanalisecurity.com`) later. A **`.nojekyll`** file is included so GitHub does not skip or process files with Jekyll.

**Custom domain:** After you connect the domain under **Pages → Custom domain**, keep `canonical` / `sitemap.xml` / JSON-LD pointed at the final `https://…` URL you want Google to index.

---

## The SEO checklist (do these AFTER deploying)

This is what actually gets him calls. The website alone is only half the job.

### A. Google Business Profile (MOST IMPORTANT)

- Go to https://business.google.com → create a profile
- Business name: **Zeeshan Ali Security Services**
- Category: **Security Service** (and add **Bodyguard** as secondary)
- Add real Karachi address (or set as service-area business covering all Pakistan)
- Phone: +92 305 3199282
- Hours: 24/7
- Add 5+ photos of him on the job
- Link the website
- **Ask 5–10 past clients to leave Google reviews.** This is what makes him appear on Google Maps when people search "bodyguard near me" in Karachi.

### B. Submit sitemap to Google

- Sign up at https://search.google.com/search-console
- Add domain (verify via Cloudflare DNS — 1 click)
- Sitemaps → submit `https://zeeshanalisecurity.com/sitemap.xml`

### C. Bing Webmaster Tools

- https://www.bing.com/webmasters → submit same sitemap
- Powers Bing, Yahoo, and DuckDuckGo

### D. Facebook Business Page

- Create Page → Local Business / Security
- Use the same logo (`assets/logo.svg`)
- Link the website
- Post weekly: job photos (with permission), security tips, client wins (with permission)

### E. WhatsApp Business

- Install **WhatsApp Business** on his phone (free, separate from regular WhatsApp)
- Set business name, hours, catalog
- The site's WhatsApp links already point to +92 305 3199282

### F. Local directories & backlinks

Submit business listings to:
- OLX Pakistan (Services → Security)
- Lamudi / PakWheels-style local platforms
- Karachi Chamber of Commerce
- Yellow Pages PK
- Facebook & Instagram business profiles

Each backlink helps SEO.

### G. Target Pakistan-wide search terms

The site is already optimized for these searches:
- "bodyguard Karachi"
- "bodyguard Pakistan"
- "personal security Karachi"
- "VIP protection Karachi"
- "bodyguard interior Sindh"
- "bodyguard Balochistan"
- "hire bodyguard Lahore" / "Islamabad" / "Quetta"
- "close protection Pakistan"

To strengthen these, post on Facebook/Instagram weekly using these keywords.

---

## Pre-launch test checklist

Before sharing the link with clients:

- [ ] Open the site on a real phone — does the **call button** dial his number?
- [ ] Tap **WhatsApp** button — does it open chat with `+92 305 3199282`?
- [ ] Submit the contact form — does the email arrive at `zeeshankaleri328@gmail.com`?
- [ ] Run [Google PageSpeed Insights](https://pagespeed.web.dev) — should score 95+
- [ ] Run [Rich Results Test](https://search.google.com/test/rich-results) — confirms LocalBusiness schema works
- [ ] Share URL on WhatsApp to yourself — does the **preview image** show up?
- [ ] Test mobile menu (☰) on a small phone screen
- [ ] Check all pages on iPhone Safari, Android Chrome

---

## Adding more pages later

To add a city-specific landing page (great for SEO, e.g. `bodyguard-lahore.html`):

1. Copy `services.html` as a starting template
2. Update `<title>`, `<meta description>`, JSON-LD `addressLocality`, and content to focus on that city
3. Add the new URL to `sitemap.xml`
4. Link to it from the homepage Coverage section

City-specific pages rank dramatically better for "bodyguard [city]" searches than a generic page does.

---

## Quick contact summary (for sharing on cards / signatures)

```
Zeeshan Ali Security Services
Bodyguard & Personal Protection
Karachi · All Pakistan

📞  +92 305 3199282  (24/7)
💬  wa.me/923053199282
✉️  zeeshankaleri328@gmail.com
🌐  zeeshanalisecurity.com  (after launch)
```
