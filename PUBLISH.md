# Publish to GitHub Pages — Tosin Gbajavi Portfolio

Your portfolio is committed locally and configured for your GitHub repository:

| Item | Value |
|------|--------|
| GitHub user | **drjavi1** |
| Repository | **drjavi.github.io** *(or `drjavi1.github.io` if renamed)* |
| Live URL | **https://drjavi1.github.io/drjavi.github.io/** *(or **https://drjavi1.github.io**)* |
| Remote | `https://github.com/drjavi1/drjavi.github.io.git` |

---

## How to Publish Live on GitHub Pages (Fastest Method)

All portfolio files (`index.html`, `assets/css/style.css`, `assets/js/main.js`, `README.md`, and `.nojekyll`) are included in this repository.

To activate the live site:

1. Open your repository settings on GitHub:  
   👉 **[https://github.com/drjavi1/drjavi.github.io/settings/pages](https://github.com/drjavi1/drjavi.github.io/settings/pages)**
2. Under **Build and deployment**:
   - Select **Source: Deploy from a branch**
   - Choose **Branch: `main`** and **Folder: `/ (root)`**
   - Click **Save**
3. Wait approximately 1–2 minutes, then visit your live site:  
   🌐 **[https://drjavi1.github.io/drjavi.github.io/](https://drjavi1.github.io/drjavi.github.io/)**

> **Tip — Root domain URL:**  
> If you want your site at **https://drjavi1.github.io** without `/drjavi.github.io/` at the end, go to **Settings → General** on GitHub and rename the repository from `drjavi.github.io` to **`drjavi1.github.io`**.

---

## Updating Your Site Later

Whenever you want to add new certifications, update your experience, or adjust styling:

```bash
# Make your edits to index.html or assets/css/style.css, then run:
git add .
git commit -m "Update portfolio content"
git push origin main
```

GitHub Pages will automatically rebuild and deploy your changes within 1–2 minutes.

---

## Troubleshooting

| Issue | Fix |
|-------|-----|
| 404 on live site | Ensure Pages is enabled under **Settings → Pages** and wait 2–3 minutes for deployment to complete. |
| Site shows old content | Perform a hard refresh in your browser (`Ctrl+Shift+R` or `Cmd+Shift+R`) or wait for CDN cache to clear. |
| Missing styles or JavaScript | Ensure the `assets/` folder is present in the repository root (which is now configured by default). |
