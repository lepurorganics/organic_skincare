# Le Pur Organics — GitHub Pages Brand Hub

Static two-page SEO brand hub for `https://lepurorganics.com/`.
Plain HTML, CSS and JavaScript. No build step, no frameworks.

## Live URLs

- Home: `https://lepurorganics.github.io/organic_skincare/`
- Top 10 products: `https://lepurorganics.github.io/organic_skincare/signature-products.html`

## Files

| File | Purpose |
|---|---|
| `index.html` | Page 1 — brand profile, story, standard, concerns, FAQ |
| `signature-products.html` | Page 2 — top 10 product guide, comparison table, routine, FAQ |
| `media.html` | Page 3 — press coverage archive, starting with Dawn Images (2023) |
| `style.css` | Brand theme |
| `script.js` | Mobile menu and footer year only |
| `404.html` | Branded not-found page |
| `sitemap.xml` | Both canonical URLs |
| `robots.txt` | Intent only (see note below) |
| `.nojekyll` | Disables Jekyll processing |
| `assets/` | Official logo, product images, social share image, icons, self-hosted Nunito Sans |

## Deploy

1. Repository must be **public**: `lepurorganics/organic_skincare`.
2. Upload the **contents** of this folder to the repository root (not the folder itself).
   If the browser upload skips the hidden `.nojekyll` file, create an empty file with that exact name in the repo root.
3. GitHub → Settings → Pages → Source: **Deploy from a branch** → Branch: **main** → Folder: **/ (root)** → Save.
4. Wait 1–3 minutes, then open the home URL.
5. Confirm `signature-products.html`, `style.css` and `assets/` all load.

## Search engines

1. Google Search Console → Add property → **URL prefix**:
   `https://lepurorganics.github.io/organic_skincare/`
2. Verify with the HTML meta tag. Paste the Google tag into the `<head>` of `index.html` and `signature-products.html`.
3. Submit the sitemap:
   `https://lepurorganics.github.io/organic_skincare/sitemap.xml`
4. Request indexing for both pages.
5. Bing Webmaster Tools → add the same URL prefix → submit the sitemap.

### robots.txt note

Search engines read `robots.txt` only at the host root (`https://lepurorganics.github.io/robots.txt`), which this project does not control. The included `robots.txt` documents intent; it is not what Google will read. Indexing is controlled by the `<meta name="robots">` tags and Search Console.

## SEO rules for future edits

- Keep every page self-canonical to its full GitHub Pages URL.
- Do not copy text from the Shopify store or the WordPress guide blog. Keep this content original.
- Do not add prices. Link to the official product page for current pricing.
- Do not invent certifications, awards, ingredients or review counts.
- Only use claims already made by Le Pur Organics.
- Keep one H1 per page and preserve the H2/H3 order.
- Use relative paths (`style.css`, `assets/...`). Never use root-absolute paths.
- Add `width` and `height` to every image, plus descriptive alt text.
- Update `lastmod` in `sitemap.xml` when page content changes.
- Re-check product URLs and claims every quarter.

## Recommended

Add one link from `lepurorganics.com` (footer or About page) to this hub, for example:

`<a href="https://lepurorganics.github.io/organic_skincare/">Brand Profile</a>`

That link makes the hub discoverable and gives it a legitimate place in the brand's link graph.
