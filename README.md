# PRISM Website

Static GitHub Pages-ready website for **PRISM Reliability Assistant**.

## Included pages

- `index.html` — product landing page
- `download.html` — beta download and Chrome install steps
- `about.html` — mission, team, roadmap, and Baylor recognition
- `404.html` — simple GitHub Pages fallback page

## Extension beta

The extension beta is included at:

```text
assets/downloads/prism-extension-beta.zip
```

The current download button already points to that file.

Extension zip SHA-256 prefix: `ff197f607ff3b12a`

## Preview locally

From this folder, run:

```bash
python -m http.server 5500
```

Then visit:

```text
http://localhost:5500
```

## Publish with GitHub Pages

1. Create a new GitHub repository, for example `prism-website`.
2. Upload the contents of this folder to the root of the repo.
3. Commit and push to `main`.
4. In GitHub, go to **Settings → Pages**.
5. Under **Build and deployment**, choose:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/root**
6. Click **Save**.
7. Wait for GitHub to publish the site.

Your site will usually be available at:

```text
https://YOUR-USERNAME.github.io/prism-website/
```

## Custom domain later

After buying/connecting a domain, add a `CNAME` file at the repo root containing only the domain name, such as:

```text
prismyourdomain.com
```

Then configure DNS in your domain provider and update GitHub Pages settings.

## Security notes

- No API keys are included.
- No backend secrets are included.
- The extension zip is public once hosted.
- Future paid API calls should go through a backend, not directly from the Chrome extension.
