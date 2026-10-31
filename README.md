# SimplyIT website

Production static website for [simplyit.cc](https://simplyit.cc). It is intentionally dependency-free and served directly from the repository root by GitHub Pages.

## Local preview

From the repository root:

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000/` in a browser.

## Editing

- Page content and metadata: `index.html`
- Visual styles and responsive layout: `assets/styles.css`
- Navigation behavior and footer year: `assets/site.js`
- Primary contact address: search for `hello@simplyit.cc` in `index.html`
- Brand artwork: `assets/simplyit-logo.webp` (display) and `assets/simplyit-logo.png` (social sharing)

The source logo supplied for the project was not modified; optimized derivatives are stored in `assets/`.

## GitHub Pages setup

Before activating GitHub Pages, the owner should review and confirm all page copy and confirm that `hello@simplyit.cc` is the intended contact address. The repository does not provision or verify that mailbox.

1. Open the repository on GitHub and go to **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select the `main` branch and the `/ (root)` folder, then save.
4. The site is currently available at `https://jimtennant.dev/simplyit.cc/` through the GitHub account's existing Pages domain.
5. To activate `simplyit.cc` later, configure the domain's DNS records for GitHub Pages, add a `CNAME` file containing `simplyit.cc`, then enable **Enforce HTTPS** after the certificate is available.

No build command or package installation is required.
