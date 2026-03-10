# Fusion 29 Presskit

Live site: https://vlainic.github.io/fusion29-presskit/

---

## How to Update & Deploy

### 1. Edit source files

- `data/data.xml` — company info (team, description, socials)
- `data/product/data.xml` — game info (features, trailers, links)
- `assets/css/master.css` — styling

### 2. Build

```bash
npm run build
```

### 3. Deploy

```bash
cd build
git add .
git commit -m "Your message here"
git push -u origin gh-pages --force
```

When prompted:
- Username: `vlainic`
- Password: your GitHub Personal Access Token (not your password)

---

## Notes

- Always run commands from a **real terminal** (not Cursor's built-in terminal) to avoid auth issues.
- The `build/` folder has its own `.git` — it's a separate repo pointing to the `gh-pages` branch.
- The main project folder tracks the `main` branch (source files only).
- GitHub Pages takes ~1-2 minutes to reflect changes after pushing.
