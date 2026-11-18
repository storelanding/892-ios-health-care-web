# Health Care — website

Static website for the Health Care iOS app (App Store): `index.html` (landing page), `policies.html` (Privacy Policy), `terms.html` (Terms of Use), `app-ads.txt`, `404.html`. No build step — deploy the repository root as is.

## Deploy

**Vercel**
1. Add New → Project → import this repo.
2. Framework Preset: **Other**. Build command: empty. Output directory: `.`
3. Add your domain in Settings → Domains.

**Cloudflare Pages**
1. Workers & Pages → Create → Pages → Connect to Git → choose this repo.
2. Framework preset: **None**. Build command: empty. Output directory: `/`
3. Add your domain in Custom domains.

## After deploying

- `app-ads.txt` must be reachable at `https://<your-domain>/app-ads.txt`, and that domain must match the developer website set on the App Store listing.
- Privacy Policy URL for the App Store: `https://<your-domain>/policies.html`
- Site metadata is kept in `site.json` for future updates.
