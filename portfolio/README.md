# Mastan — QA Automation Engineer Portfolio

A premium, responsive portfolio website showcasing 8+ years of QA & automation expertise.

![Status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

- **Premium Design** — Modern blue/gray technology theme
- **Light & Dark Mode** — Toggle with localStorage persistence
- **Animated Counters** — Key metrics animate into view
- **Fully Responsive** — Desktop, tablet, and mobile optimized
- **Sticky Navigation** — With active section highlighting
- **Smooth Animations** — Scroll-triggered via IntersectionObserver
- **GA4 Analytics** — Visitor tracking + resume download events
- **SEO Optimized** — Meta tags, OpenGraph, JSON-LD, sitemap, robots.txt

## 📁 Folder Structure

```
portfolio/
├── index.html          # Main HTML
├── style.css           # All styles (light + dark mode)
├── script.js           # Interactivity & analytics
├── assets/
│   └── Mastan_Resume.pdf   # Your resume (downloadable)
├── favicon.ico         # Browser tab icon
├── sitemap.xml         # SEO sitemap
├── robots.txt          # Search engine rules
└── README.md           # This file
```

---

## 🚀 Deployment

### Option 1: GitHub Pages

1. Create a **new GitHub repo** (e.g., `mastan-portfolio`)
2. Push all files from the `portfolio/` folder to the repo:
   ```bash
   cd portfolio
   git init
   git add .
   git commit -m "Initial portfolio deploy"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/mastan-portfolio.git
   git push -u origin main
   ```
3. In repo **Settings → Pages**, set **Source** to `main` / `/ (root)`
4. Your site will be live at `https://YOUR_USERNAME.github.io/mastan-portfolio/`

### Option 2: Vercel

1. Install Vercel CLI (optional): `npm i -g vercel`
2. Navigate to the `portfolio/` directory
3. Run:
   ```bash
   vercel --prod
   ```
4. Or go to [vercel.com](https://vercel.com), import your GitHub repo, and deploy with defaults
5. Your site will be live at the provided `.vercel.app` URL

---

## ✏️ How to Update Content

All editable sections are marked with:
```html
<!-- EDIT CONTENT BELOW -->
```

Simply search for this comment in `index.html` to find all customizable areas:
- **Hero section** — Name, title, statement, metric values
- **About Me** — Summary paragraphs
- **Skills** — Skill tags within each category
- **Experience** — Company details, dates, achievements
- **Certifications** — Names and descriptions
- **Education** — Degree and institution
- **Contact** — Email, LinkedIn, GitHub links

---

## 📄 How to Replace the Resume

1. Place your new PDF in the `assets/` folder
2. Name it `Mastan_Resume.pdf` (or update the `href` in `index.html`)
3. Commit and push to GitHub (auto-deploys if using Pages/Vercel)

---

## 📊 Setting Up Google Analytics (GA4)

### Step 1: Get Your Measurement ID

1. Go to [analytics.google.com](https://analytics.google.com/)
2. Create an account → Create a **Property**
3. In **Admin → Data Streams → Web**, add your site URL
4. Copy the **Measurement ID** (format: `G-XXXXXXXXXX`)

### Step 2: Add It to Your Site

In `index.html`, find this line near the top:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
```

Replace **both** instances of `GA_MEASUREMENT_ID` with your actual ID:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
    ...
    gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Step 3: View Resume Download Stats

1. In GA4, go to **Reports → Engagement → Events**
2. Look for the event named **`resume_download`**
3. Click it to see download count, user demographics, and timeline

---

## 🎨 Customization Tips

| What | Where |
|------|-------|
| Colors & Fonts | CSS custom properties in `style.css` (`:root`) |
| Dark mode colors | `[data-theme="dark"]` block in `style.css` |
| Social links | Search `href="#"` in `index.html` |
| Favicon | Replace `favicon.ico` with your own |
| Domain references | Search `yourdomain.com` and replace everywhere |

---

## 📜 License

This portfolio is for personal use by Mastan. Feel free to fork and customize for your own portfolio.
