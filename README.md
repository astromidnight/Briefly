# Briefly — site (GitHub Pages)

Static site for **briefly.pt**. No build step.

## Files
- `index.html`, `about.html`, `privacy.html`, `terms.html` — pages
- `assets/` — logo, favicon, share image (1200×630)
- `robots.txt`, `sitemap.xml` — SEO
- `CNAME` — custom domain (briefly.pt). **Keep this file.**
- `.nojekyll` — disables Jekyll processing on GitHub Pages

## Deploy to GitHub Pages
1. Put **all these files in the root** of the repo (not in a subfolder),
   or use the `/docs` folder and point Pages at it.
2. Repo → **Settings → Pages** → Source: `Deploy from a branch`,
   branch `main`, folder `/ (root)`.
3. Under **Custom domain**, confirm it shows `briefly.pt` (the CNAME file sets this).
4. At your domain registrar, point DNS to GitHub Pages:
   - 4 `A` records on the apex (`briefly.pt`) → `185.199.108.153`,
     `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - optional `CNAME` for `www` → `<your-user>.github.io`
5. Enable **Enforce HTTPS** once the certificate is issued.

## After it's live
- Submit `https://briefly.pt/sitemap.xml` in Google Search Console.
- Validate share image at developers.facebook.com/tools/debug (Scrape Again).
