# reflectiveintelligence.life — Website Deployment Guide

## What's in this folder
```
ri-website/
├── index.html      ← Complete website (all CSS + JS inline, no build needed)
└── ri-logo.png     ← Your Reflective Intelligence eye logo
```

## How to go live — 3 options (all free)

---

### Option A: Netlify Drop (easiest — 2 minutes)
1. Go to https://app.netlify.com/drop
2. Drag the entire `ri-website/` folder onto the page
3. You get a live URL instantly (e.g. https://amazing-cactus-123.netlify.app)
4. To connect your custom domain `reflectiveintelligence.life`:
   - In Netlify → Site Settings → Domain Management → Add custom domain
   - Update your domain's DNS: add a CNAME record pointing to your Netlify URL

---

### Option B: GitHub Pages (recommended for version control)
1. Create a GitHub account if you don't have one
2. Create a new repository named `reflective-intelligence-site`
3. Upload both files (`index.html` and `ri-logo.png`) to the repo
4. Go to Settings → Pages → Source: Deploy from branch → main / root
5. Your site is live at `https://yourusername.github.io/reflective-intelligence-site`
6. For custom domain: add a `CNAME` file with content `reflectiveintelligence.life`
   and update your domain DNS with GitHub's nameservers

---

### Option C: Any static web host
This is a static site — no server, no database, no build process needed.
Works on: Vercel, Cloudflare Pages, Render, Firebase Hosting, or any cPanel host.

Upload both files together. Make sure `ri-logo.png` is in the same folder as `index.html`.

---

## After going live — things to update in index.html

Search for these placeholder values and replace:

| Placeholder | Replace with |
|-------------|--------------|
| `https://lumeri.co.in` | Your actual LumeRI URL |
| `hello@reflectiveintelligence.life` | Your actual email |
| `research@reflectiveintelligence.life` | Your research email |
| `https://linkedin.com/company/reflective-intelligence` | Your LinkedIn page URL |

---

## Logo file
The file `ri-logo.png` is already in this folder and referenced correctly in the HTML.
If you ever change the logo, just replace `ri-logo.png` with the new file (same filename).

---

## Site structure (6 sections)
1. **Hero** — "The observer and the observed are not two things" + floating eye logo
2. **The Symbol** — Why the eye? Krishnamurti, the vertical axis, the mirror line
3. **The Science** — 4 research cards: metacognition, Pennebaker, DMN, narrative coherence
4. **The Philosophy** — 6 thinker cards: Krishnamurti, Ramana, Nisargadatta, Rumi, Watts, Tao
5. **The Manifesto** — 6 belief statements with numbered layout
6. **For Researchers** — Constructs, research architecture, collaboration CTA
7. **Join** — Newsletter signup + LumeRI link + closing quote

---

Built with: Pure HTML + CSS + Vanilla JS. No frameworks. No build tools. No dependencies.
Fonts loaded from Google Fonts (requires internet connection).
