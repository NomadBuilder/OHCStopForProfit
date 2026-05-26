# Stop For-Profit Health Care

Modern static rebuild of [stopforprofithealthcare.ca](https://stopforprofithealthcare.ca/) for the Ontario Health Coalition.

## Live site (GitHub Pages)

**https://nomadbuilder.github.io/OHCStopForProfit/**

Deployed from the `main` branch (root). Every push to `main` rebuilds the site automatically via GitHub’s built-in Pages workflow—no custom Actions workflow needed.

To change settings: [Settings → Pages](https://github.com/NomadBuilder/OHCStopForProfit/settings/pages) → **Deploy from a branch** → `main` / `/ (root)`.

## Local preview

```bash
./start.sh
# or: python3 -m http.server 8080
```

Open http://localhost:8080

## Project structure

```
index.html                  # Home
join-the-fight.html
facts-about-health-care.html
css/styles.css
js/main.js
public/images/              # Logos, favicon
public/assets/              # Hero image, charts
source/                     # Original scraped HTML (archive)
```

## Custom domain (optional)

To use `stopforprofithealthcare.ca`, add a `CNAME` file and configure DNS at your domain registrar. See [GitHub Pages custom domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
