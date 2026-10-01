# Emily Rhodes: personal website

A static one-page site built with plain HTML, CSS and JS. There's no build step.

- `index.html` holds the content (search for `TODO` to find placeholders)
- `styles.css` holds the styling (colors are at the top in `:root`, with dark mode supported)
- `script.js` runs the mobile menu, the scroll fade-ins and the footer year

## Preview locally

Open `index.html` in a browser, or run `python3 -m http.server` and go to http://localhost:8000.

## Publish on your domain (GitHub Pages, free)

1. On GitHub, go to **Settings → Pages**. Set the source to **Deploy from a branch**, then choose `master` / `root`.
2. The `CNAME` file already sets the custom domain to `emrhodes.com`. Confirm it shows under **Custom domain** in the same screen.
3. At your domain registrar, add DNS records:
   - Apex domain (`emrhodes.com`): `A` records pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`
   - `www`: a `CNAME` record pointing to `emrho.github.io`
4. Once DNS has propagated, tick **Enforce HTTPS**.

Netlify, Vercel and Cloudflare Pages also work: drag and drop the folder, then connect the domain.
