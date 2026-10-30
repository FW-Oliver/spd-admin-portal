# SPD Admin Portal v2

Initial static dashboard scaffold for GitHub Pages.

## Files
- `index.html` — dashboard structure
- `styles.css` — responsive styling
- `app.js` — client-side entry point (no secrets or backend calls yet)

## Publish with GitHub Pages
1. Create a GitHub repository named `spd-admin-portal-v2`.
2. Upload these files to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site.

## Security boundary
GitHub Pages is public static hosting. Anything placed in this repository or browser JavaScript can be viewed by visitors. Never commit:
- Cloudflare API tokens
- R2 access keys
- Master PDF or master authentication credentials
- hospital/device secrets

The dashboard is currently a visual scaffold only. It does not authenticate users, store organizations, upload CSV files, generate activation credentials, or connect to Cloudflare. Those functions will be implemented through a Cloudflare Worker, with D1 for structured records and a private R2 bucket for CSV files.
