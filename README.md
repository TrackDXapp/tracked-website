# trackdx-website

Marketing website for **TrackDX**, served at [www.trackdx.net](https://www.trackdx.net).

Plain HTML/CSS/JS — no build step, no frameworks, no dependencies. Designed to be hosted for free on
GitHub Pages with a custom domain.

## Structure

```
trackdx-website/
├── index.html          # home page
├── about.html           # About page
├── support.html         # Support page
├── css/style.css        # styling — matches the app's coral & cream theme
├── js/main.js            # small script for the mobile nav menu
├── assets/img/           # app icon + screenshots
├── CNAME                 # tells GitHub Pages this site is www.trackdx.net
└── .gitignore
```

## Local preview

Open `index.html` directly in a browser, or run a tiny local server from this folder:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deployment

See the step-by-step GitHub Pages + Squarespace DNS instructions provided separately (or the project's
deployment notes). Short version:

1. Push this folder to a GitHub repository.
2. Enable GitHub Pages for the repo (Settings → Pages → deploy from the `main` branch).
3. Add `www.trackdx.net` as the custom domain in the Pages settings (the `CNAME` file already contains this).
4. In Squarespace Domains → DNS settings for `trackdx.net`, add a `CNAME` record for `www` pointing to
   `<your-github-username>.github.io`, and either an `A`/ALIAS record set or a redirect so the bare
   `trackdx.net` forwards to `www.trackdx.net`.

## Content ownership

TrackDX™ — © 2026 TrackDX, LLC. All rights reserved. This website's copy, design, and the TrackDX name are
the property of TrackDX, LLC.
