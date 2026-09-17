# joe-ogorman.com

Personal site. Plain HTML/CSS, deployed via GitHub Pages.

## Local preview

Open `index.html` directly in a browser, or run a local server:

```
python3 -m http.server 8000
```

## Deployment

This repo is deployed with GitHub Pages, pointed at the custom domain
`joe-ogorman.com` via the `CNAME` file.

1. Push to the `main` branch.
2. In the repo's Settings → Pages, set the source to the `main` branch, root folder.
3. At your domain registrar, add these DNS records:
   - `A` records for the apex domain (`joe-ogorman.com`) pointing to GitHub Pages' IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - `CNAME` record for `www` pointing to `<github-username>.github.io`
4. Back in Settings → Pages, enter `joe-ogorman.com` as the custom domain and enable
   "Enforce HTTPS" once DNS has propagated (can take up to a few hours).
