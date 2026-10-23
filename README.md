# Portfolio site — sinan-altaie.github.io

Single-file static site (`index.html`, no build step, no external dependencies, no tracking). Public-safe by design: no phone number, no customer names, no internal metrics, incidents described at category level.

## Publish on GitHub Pages (free, ~5 minutes)

Use your personal GitHub account (`sinan-altaie`), not the company org.

1. On GitHub, create a new **public** repository named exactly `sinan-altaie.github.io`.
2. From this folder, in Terminal:

```bash
cd "$HOME/Downloads/Sinan Al Taie Resume 2026/portfolio"
git init -b main
git add index.html README.md
git commit -m "Portfolio site"
git remote add origin https://github.com/sinan-altaie/sinan-altaie.github.io.git
git push -u origin main
```

3. In the repo: Settings → Pages → Source: "Deploy from a branch" → Branch `main`, folder `/ (root)` → Save.
4. Wait a minute, then open https://sinan-altaie.github.io/

GitHub will prompt for login on `git push` (use a browser-based login or a personal access token, not your password).

## Custom domain (optional)

If you buy a domain such as `sinanaltaie.com`: add a file named `CNAME` containing the domain to this folder, push, then in your registrar's DNS add a CNAME record `www → sinan-altaie.github.io` and the four GitHub Pages A records for the apex. GitHub Pages issues the HTTPS certificate automatically.

## Updating

Edit `index.html`, then:

```bash
git add index.html && git commit -m "Update" && git push
```

## Adding a resume download (optional, not done by default)

The resume PDF contains your phone number. If you want a download button on the site, make a copy without the phone line first, then add it to this folder and link it from the hero section.
