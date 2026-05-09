# Prerana Nale — Portfolio

Personal portfolio website for Prerana Nale, AI Engineer & Full-Stack Developer.

**Live site:** https://prerananale.com

---

## 🗂 Project Structure

```
portfolio/
├── index.html              # Main portfolio page (single file site)
├── Nale_Prerana__Resume.pdf  # Resume (add this file yourself — not in git)
├── Prerana_Nale.jpeg       # Profile photo (add this file yourself — not in git)
├── .gitignore
└── README.md
```

> **Note:** The resume PDF and profile photo are excluded from git for privacy.
> Add them manually wherever you deploy.

---

## 🚀 Deploy Options

### Option 1 — Vercel (recommended, free)
1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → "Add New Project"
3. Import your GitHub repo
4. Framework preset: **Other** (it's plain HTML)
5. Click Deploy — done. Vercel gives you a free `.vercel.app` URL
6. Add your custom domain `prerananale.com` in Vercel's domain settings

### Option 2 — Netlify (free)
1. Go to [netlify.com](https://netlify.com) → "Add new site" → "Import from Git"
2. Connect your GitHub repo
3. Build command: *(leave empty)*
4. Publish directory: `.` (root)
5. Deploy

### Option 3 — GitHub Pages (free)
1. Push to GitHub
2. Go to repo Settings → Pages
3. Source: `Deploy from a branch` → `main` → `/ (root)`
4. Your site will be at `https://yourusername.github.io/portfolio`

### Option 4 — Hostinger (current)
Upload `index.html` + `Prerana_Nale.jpeg` + `Nale_Prerana__Resume.pdf`
directly into `public_html/` via File Manager.

---

## 💻 Run Locally

No build step needed — it's plain HTML/CSS/JS.

```bash
# Option A: Python (built into macOS/Linux)
cd portfolio
python3 -m http.server 3000
# Open http://localhost:3000

# Option B: Node.js (if installed)
npx serve .
# Open http://localhost:3000

# Option C: VS Code
# Install "Live Server" extension → right-click index.html → "Open with Live Server"
```

---

## 📁 Adding Your Files

Before deploying, place these two files in the same folder as `index.html`:

| File | Where to get it |
|------|----------------|
| `Prerana_Nale.jpeg` | Download from Hostinger File Manager |
| `Nale_Prerana__Resume.pdf` | Download from Hostinger File Manager |

---

## ✏️ Making Changes

Everything is in `index.html` — one file, no framework, no build step.

- **Update content:** Search for the text you want to change and edit it directly
- **Update colors:** Change CSS variables at the top of the `<style>` block (`:root { --bg, --ink, etc. }`)
- **Add a project:** Copy one of the `.pr` row blocks in the Work section and update the text

---

## 🌐 Custom Domain on Vercel

1. Deploy to Vercel first (Option 1 above)
2. In Vercel dashboard → your project → Settings → Domains
3. Add `prerananale.com`
4. Vercel shows you DNS records to update
5. In Hostinger → Domains → DNS Zone → update the `A` and `CNAME` records
6. Wait ~10 minutes → your domain now points to Vercel (faster, free SSL)
