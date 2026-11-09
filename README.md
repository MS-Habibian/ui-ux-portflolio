# Maya Chen Portfolio

A small, responsive, single-page portfolio for a fictional UI/UX and product designer. The site uses plain HTML, CSS, and JavaScript, with CSS-built artwork so it can deploy as a static site without a build step or dependencies.

## Structure

```text
public/
├── index.html
├── styles.css
├── script.js
└── assets/
```

There are currently no required files in `public/assets/`.

## Run locally

From the repository root, run any simple static HTTP server, for example:

```bash
python3 -m http.server 8000 --directory public
```

Open `http://localhost:8000` in a browser. No installation or build command is required.

## Push to GitHub

Create an empty repository on GitHub, then add it as the remote and push the `main` branch:

```bash
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

## Cloudflare Pages

Create a Pages project using the repository's GitHub integration with these settings:

- Framework preset: **None**
- Production branch: **main**
- Build command: **Empty**
- Build output directory: **public**
- Root directory: **Repository root**

Cloudflare Pages will deploy `public/index.html` directly. Pushes to `main` create production deployments; pushes to other branches create preview deployments. To update the deployed site, commit changes and push them to the configured branch.
