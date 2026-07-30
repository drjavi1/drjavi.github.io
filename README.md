# Tosin Gbajavi — Portfolio

**Clinical Informatics Specialist | Doctor of Optometry (OD) & MPH | Digital Health & Health AI**

Personal portfolio website showcasing clinical informatics experience, digital health expertise, education, and certifications.

🌐 **Live site:** [https://drjavi.github.io](https://drjavi.github.io)  
🔗 **LinkedIn:** [linkedin.com/in/tosingbajavi](https://www.linkedin.com/in/tosingbajavi)  
✉️ **Email:** [tosin.vincent@gmail.com](mailto:tosin.vincent@gmail.com)
📦 **GitHub:** [github.com/drjavi](https://github.com/drjavi)

---

## What’s included

| Section | Content |
|--------|---------|
| **Hero** | Professional headline, location, CTA |
| **About** | Dual clinician–informaticist narrative |
| **Expertise** | Clinical workflows, Health AI, data governance, leadership |
| **Experience** | Full career timeline from LinkedIn |
| **Education** | OD (University of Benin) · MPH (Ahmadu Bello University) |
| **Certifications** | Azure AI, Oracle Cloud AI, Claude/Bedrock, SQL |
| **Contact** | Email, LinkedIn, phone, location |

Built with plain **HTML, CSS, and JavaScript** — no build step, ready for **GitHub Pages**.

---

## Project structure

```
portfolio/
├── index.html              # Main portfolio page
├── README.md               # This file
├── LICENSE                 # MIT license
└── assets/
    ├── css/style.css       # Styles
    └── js/main.js          # Nav, scroll effects
```

---

## Deploy to GitHub Pages (step by step)

### Option A — New repository (recommended)

1. Create a new GitHub repo named **`drjavi.github.io`** (user site → live at https://drjavi.github.io).  
   - Or use any name (e.g. `portfolio`) → site at `https://drjavi.github.io/portfolio/`

2. Push this folder:

```bash
cd portfolio
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/drjavi/drjavi.github.io.git
git push -u origin main
```

3. On GitHub: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main** / folder: **/ (root)**
   - Save

4. Wait 1–2 minutes, then open https://drjavi.github.io

### Option B — Upload via GitHub web UI

1. Create a new repository on GitHub.
2. Click **Add file → Upload files**.
3. Drag in everything from this `portfolio` folder.
4. Commit, then enable Pages as in step 3 above.

---

## Local preview

Open `index.html` in a browser, or serve locally:

```bash
# Python
python3 -m http.server 8080

# Node (if you have npx)
npx serve .
```

Then visit `http://localhost:8080`.

---

## Customize

| What | Where |
|------|--------|
| Contact details | `index.html` → `#contact` and hero meta |
| Experience bullets | `index.html` → `#experience` |
| Colors / fonts | `assets/css/style.css` → `:root` variables |
| Add a photo | Replace the `.avatar` initials block with an `<img>` |

---

## Tech notes

- Fully responsive (mobile nav, fluid type)
- Accessible landmarks, focus styles, reduced-motion support
- Zero dependencies — fast load on GitHub Pages
- SEO-friendly title and meta description

---

## License

MIT — see [LICENSE](LICENSE). Content (bio, experience) © Tosin Gbajavi.
