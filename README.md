# visquill

Interactive visualization of seafloor geomorphology, bathymetry, and primary productivity — built with [@visquill/visquill-gdk](https://visquill.com/developers).

---

## Deployment

### Local preview

```bash
npm install
npx serve .
# open http://localhost:3000
```

Or with Python (no install needed):

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

> The page must be served over HTTP — opening `index.html` directly as a `file://` URL will block the ES module imports.

---

### GitHub Pages

1. Push the branch and merge to `main`
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch**, select `main`, folder `/` (root)
4. GitHub will publish the site at `https://<your-username>.github.io/visquill/`

---

### Netlify (drag & drop)

1. Run `npm install` locally to ensure `node_modules` is present
2. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
3. Drag the entire `visquill/` project folder onto the page
4. Netlify gives you a live URL instantly — no config needed

---

### Netlify CLI

```bash
npm install -g netlify-cli
netlify deploy --dir . --prod
```

---

### Vercel

```bash
npm install -g vercel
vercel --prod
```

No framework preset needed — Vercel will detect it as a static site.

---

## Usage

Once open in a browser, drag the **◈ handle** along the ocean surface to explore:

- **Depth** at that location
- **Bathymetric zone** (Sunlit / Twilight / Midnight / Abyssal)
- **Primary productivity** index with bar indicator