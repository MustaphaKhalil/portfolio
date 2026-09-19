# Mustapha Khalil — Portfolio Website

A single-file, static portfolio site (`index.html`). No build step, no dependencies beyond a Google Fonts stylesheet link — just open it in a browser or host it as-is.

## Publish it on GitHub Pages (free hosting)

1. **Create a new repository on GitHub**
   - Go to [github.com/new](https://github.com/new)
   - Name it whatever you like — for a *user* site at `https://<your-username>.github.io`, the repo must be named exactly `<your-username>.github.io`. For a *project* site at `https://<your-username>.github.io/<repo-name>`, any repo name works.
   - Keep it Public (GitHub Pages on the free tier requires a public repo, unless you have GitHub Pro/Team/Enterprise).
   - Don't initialize it with a README (this folder already has one).

2. **Push this folder to the repo**
   From inside this `portfolio-website` folder, run:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

3. **Turn on GitHub Pages**
   - In the repo, go to **Settings → Pages**.
   - Under "Build and deployment", set **Source** to `Deploy from a branch`.
   - Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
   - GitHub will give you a live URL in a minute or two (either `https://<your-username>.github.io` or `https://<your-username>.github.io/<repo-name>`).

4. **Optional: custom domain**
   - Add a `CNAME` file to this folder containing just your domain (e.g. `mustaphakhalil.com`).
   - Point your domain's DNS at GitHub Pages (an `A` record to GitHub's IPs, or a `CNAME` record to `<your-username>.github.io` for a subdomain).
   - Enter the domain under **Settings → Pages → Custom domain** and enable "Enforce HTTPS" once it's verified.

## Updating the site later

Edit `index.html`, then:
```bash
git add .
git commit -m "Update site"
git push
```
GitHub Pages redeploys automatically within a minute or two of any push to `main`.

## Files

- `index.html` — the entire site (HTML, CSS, content). Fonts load from Google Fonts via CDN link; everything else is self-contained.
