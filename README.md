# Tosin Gbajavi — Portfolio

**Clinical Informatics Specialist | Doctor of Optometry (OD) & MPH | Digital Health & Health AI**

Personal portfolio website showcasing clinical informatics experience, digital health expertise, education, and certifications.

🌐 **Live site:** [https://drjavi1.github.io/drjavi.github.io/](https://drjavi1.github.io/drjavi.github.io/) *(or [https://drjavi1.github.io/](https://drjavi1.github.io/) if repository is renamed to `drjavi1.github.io`)*  
🔗 **LinkedIn:** [linkedin.com/in/tosingbajavi](https://www.linkedin.com/in/tosingbajavi)  
✉️ **Email:** [tosin.vincent@gmail.com](mailto:tosin.vincent@gmail.com)  
📦 **GitHub:** [github.com/drjavi1](https://github.com/drjavi1)

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

Built with plain **HTML, CSS, and JavaScript** — no build step required, ready for **GitHub Pages**.

---

## Project structure

```
drjavi.github.io/
├── index.html              # Main portfolio page
├── README.md               # This documentation
├── PUBLISH.md              # Publishing guide
├── LICENSE                 # MIT license
├── .nojekyll               # Disables Jekyll processing on GitHub Pages
└── assets/
    ├── css/
    │   └── style.css       # Styles and responsive layout
    └── js/
        └── main.js         # Nav, scroll effects, dynamic year
```

---

## Publishing to GitHub Pages (2 quick clicks on GitHub)

Your portfolio code and styling assets are fully configured and ready to go live on GitHub Pages.

1. Go to your GitHub repository Pages settings:  
   👉 **[https://github.com/drjavi1/drjavi.github.io/settings/pages](https://github.com/drjavi1/drjavi.github.io/settings/pages)**
2. Under **Build and deployment**:
   - Set **Source** to **Deploy from a branch**
   - Choose Branch **`main`** and Folder **`/ (root)`**
   - Click **Save**
3. Wait approximately 1–2 minutes, and your live portfolio will be published at:
   - 🌐 **https://drjavi1.github.io/drjavi.github.io/**

> **Tip — Root domain URL:**  
> To serve your portfolio directly at **https://drjavi1.github.io** (without `/drjavi.github.io/` at the end), go to **Settings → General** on GitHub and rename this repository from `drjavi.github.io` to **`drjavi1.github.io`**.

---

## Local preview

Open `index.html` directly in a browser, or serve locally using any HTTP server:

```bash
# Python
python3 -m http.server 8080

# Node
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

- Fully responsive (mobile nav, fluid typography, modern layout)
- Accessible landmarks, focus styles, reduced-motion support
- Zero dependencies — fast load on GitHub Pages
- SEO-friendly title and meta description

---

## License

MIT — see [LICENSE](LICENSE). Content (bio, experience) © Tosin Gbajavi.
