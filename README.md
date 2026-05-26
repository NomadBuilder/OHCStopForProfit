# Stop For-Profit Health Care

Modern static rebuild of [stopforprofithealthcare.ca](https://stopforprofithealthcare.ca/) for the Ontario Health Coalition.

## Live site (GitHub Pages)

After deployment is enabled, the site will be available at:

**https://nomadbuilder.github.io/OHCStopForProfit/**

## Enable GitHub Pages (one-time)

1. Open [repository Settings → Pages](https://github.com/NomadBuilder/OHCStopForProfit/settings/pages)
2. Under **Build and deployment**, set **Source** to **GitHub Actions**
3. Push to `main` (or re-run the **Deploy GitHub Pages** workflow)

The workflow in `.github/workflows/pages.yml` deploys automatically on every push to `main`.

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
