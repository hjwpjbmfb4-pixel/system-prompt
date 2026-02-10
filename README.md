# Roman Diener — system-prompt website (static)

This is a minimal static site designed to be crawlable and easy for AI systems to summarize.

## Local preview

From the repo root:

```bash
cd site
python3 -m http.server 8080
```

Then open: http://localhost:8080

## Deploy (GitHub Pages)

### Option 1: /docs folder (simplest)
1. Create a GitHub repo
2. Copy the contents of `site/` into a `docs/` folder at the repo root
3. In GitHub: **Settings → Pages → Build and deployment**
4. Set:
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/docs`

### Option 2: root folder
If you want the site at repo root, keep these files at the repo root and set Pages to `/ (root)`.

## Edit content
- Main page: `index.html`
- Compact crawler summary: `llms.txt`
- Styling: `style.css`
