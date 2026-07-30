# Publish to GitHub Pages — drjavi

Your portfolio is already committed locally and configured for:

| Item | Value |
|------|--------|
| GitHub user | **drjavi** |
| Repository | **drjavi.github.io** |
| Live URL | **https://drjavi.github.io** |
| Remote | `https://github.com/drjavi/drjavi.github.io.git` |

This sandbox cannot log into your GitHub account, so the final push must run on **your computer** (or GitHub’s website). Pick one method below.

---

## Method 1 — GitHub website (easiest, ~3 minutes)

1. Open **[https://github.com/new](https://github.com/new)** while logged in as **drjavi**.
2. Repository name: **`drjavi.github.io`** (exactly this name for a root user site).
3. Set visibility to **Public**.
4. **Do not** add a README, .gitignore, or license (this folder already has them).
5. Click **Create repository**.
6. On the empty repo page, click **uploading an existing file**.
7. Open the `portfolio` folder on your machine (or unzip `drjavi-portfolio-github.zip`).
8. Drag in **all files** at the root of the portfolio:
   - `index.html`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
   - `.nojekyll`
   - `assets/` folder (with css + js inside)
9. Commit message: `Initial portfolio site`
10. Click **Commit changes**.
11. Go to **Settings → Pages**.
12. Under **Build and deployment**:
    - Source: **Deploy from a branch**
    - Branch: **main** (or **master**), folder **/ (root)**
    - Save
13. Wait 1–2 minutes, then visit **[https://drjavi.github.io](https://drjavi.github.io)**.

---

## Method 2 — Git command line (recommended long-term)

On your computer, with [Git](https://git-scm.com/) installed and logged into GitHub:

### A. Create the empty repo first

1. Go to [https://github.com/new](https://github.com/new)
2. Name it **`drjavi.github.io`**, Public, no README → Create.

### B. Push this portfolio

```bash
# Download / copy the portfolio folder, then:
cd portfolio

# If git is not initialized yet:
git init
git add .
git commit -m "Initial portfolio site for Tosin Gbajavi"
git branch -M main

git remote add origin https://github.com/drjavi/drjavi.github.io.git
# If remote already exists:
# git remote set-url origin https://github.com/drjavi/drjavi.github.io.git

git push -u origin main
```

When prompted, sign in with your GitHub username (**drjavi**) and a **Personal Access Token** (not your password).

**Create a token:** GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic) → Generate  
Scopes needed: **`repo`**

### C. Enable Pages

**Settings → Pages → Deploy from a branch → main / root → Save**

Site: **https://drjavi.github.io**

---

## Method 3 — GitHub CLI

```bash
# Install: https://cli.github.com/
gh auth login
cd portfolio
gh repo create drjavi.github.io --public --source=. --remote=origin --push
gh api -X POST repos/drjavi/drjavi.github.io/pages -f build_type=legacy -f source[branch]=main -f source[path]=/
```

---

## After it’s live

- Share: https://drjavi.github.io  
- Add the link to your LinkedIn **Featured** or **Website** field  
- Optional: custom domain under **Settings → Pages → Custom domain**

### Update the site later

```bash
cd portfolio
# edit files...
git add .
git commit -m "Update portfolio content"
git push
```

GitHub Pages rebuilds automatically in about a minute.

---

## Troubleshooting

| Issue | Fix |
|-------|-----|
| 404 on drjavi.github.io | Confirm repo name is exactly `drjavi.github.io` and Pages is enabled on `main` / root |
| Site shows old content | Hard refresh (Ctrl+Shift+R) or wait 2–5 min for CDN |
| Push rejected / auth failed | Use a Personal Access Token with `repo` scope |
| CSS/JS not loading | Ensure `assets/` was uploaded and `.nojekyll` is in the repo root |
