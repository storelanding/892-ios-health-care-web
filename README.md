# Health Care — website

Static landing site for the **Health Care** iOS app (App Store): `index.html`, `policies.html` (Privacy Policy),
`terms.html` (Terms of Use), `app-ads.txt`, `404.html`. No build step — deploy the repository root as-is.

## Deploy

**Cloudflare Pages:** Workers & Pages → Create → Pages → Connect to Git → choose this repo.
Framework preset **None**, build command empty, output directory `/`. Add your domain under Custom domains.

**Vercel:** Add New → Project → import this repo. Framework **Other**, no build command, output directory `.`.
Add your domain under Settings → Domains.

## After deploy

- `app-ads.txt` must be reachable at `https://<your-domain>/app-ads.txt`, and that domain must match the developer
  website declared on the App Store listing.
- Privacy Policy URL for App Store Connect: `https://<your-domain>/policies.html`.
- Site metadata lives in `site.json`; update it and regenerate when store details change.
