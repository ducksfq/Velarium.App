# Velarium website

Single-page static site for Velarium — serves both as the App Store
**Support URL** and **Marketing URL**. Pure HTML / CSS, no build step,
no JavaScript dependencies, no backend.

## Files

- `index.html` — landing page with sections for hero, features, support
  FAQ, and a privacy summary
- `styles.css` — dreamcore palette + serif wordmark to match the in-app
  aesthetic
- `assets/icon.png` — 1024×1024 app icon (also used as favicon and
  Open Graph preview)

## Hosting (free options)

### GitHub Pages (recommended)

1. Create a new public repo, e.g. `velarium-site`.
2. Copy the contents of this `website/` folder into the repo root.
3. Push to GitHub.
4. Repo → **Settings → Pages → Build from branch → main / root**.
5. Site goes live at `https://<your-username>.github.io/velarium-site/`.

### Cloudflare Pages

1. Sign in at <https://pages.cloudflare.com>.
2. **Create a project → Direct upload**.
3. Drag the `website/` folder onto the upload zone.
4. Site goes live at `https://velarium.pages.dev` (free tier includes
   unlimited bandwidth and a `*.pages.dev` subdomain).

### Netlify

1. Sign in at <https://app.netlify.com>.
2. **Add new site → Deploy manually**.
3. Drag the `website/` folder onto the drop zone.
4. Site goes live at `https://velarium-<random>.netlify.app`.

### Custom domain (optional, ~$15/year)

Buy a domain (Cloudflare Registrar tends to be cheapest at-cost) and
point its DNS at whichever host above you used. Each provider has a
"Custom domain" setting that takes care of HTTPS automatically.

## Updating the email address

The default contact email is `hello@velarium.app`. If you want to use
your own address before the domain is registered, edit the `mailto:`
link in `index.html` (search for `hello@velarium.app`).

## What goes into App Store Connect

Once the site is live, both fields point to the same URL:

- **Marketing URL:** `https://your-site/`
- **Support URL:** `https://your-site/#support` (anchored to FAQ)

Apple checks these are reachable during review.
