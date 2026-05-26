# Stop For-Profit Health Care

Modern static rebuild of [stopforprofithealthcare.ca](https://stopforprofithealthcare.ca/) for the Ontario Health Coalition.

## Live site (GitHub Pages)

After deployment is enabled, the site will be available at:

**https://nomadbuilder.github.io/OHCStopForProfit/**

## Enable GitHub Pages (one-time — pick one)

### Option A — Deploy from branch (simplest)

1. Open [Settings → Pages](https://github.com/NomadBuilder/OHCStopForProfit/settings/pages)
2. **Build and deployment** → **Source**: **Deploy from a branch**
3. **Branch**: `main` → folder **`/ (root)`** → **Save**

The site should be live within a few minutes. No GitHub Actions required.

### Option B — GitHub Actions

1. Open [Settings → Pages](https://github.com/NomadBuilder/OHCStopForProfit/settings/pages)
2. **Source**: **GitHub Actions**
3. Re-run the [Deploy GitHub Pages](https://github.com/NomadBuilder/OHCStopForProfit/actions/workflows/pages.yml) workflow

Future pushes to `main` deploy automatically.

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
