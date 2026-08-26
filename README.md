# Achilles Sports Kit Builder

This is the current GitHub Pages package for the Achilles Sports 3D Kit Builder.

## Files

- `index.html` — latest kit builder
- `.nojekyll` — tells GitHub Pages to serve the files directly
- `shopify-custom-liquid.txt` — iframe code to paste into the Shopify Kit Builder page
- `README.md` — these instructions

## Latest changes already included

- Continue/buy flow downloads the combined kit design export first
- Export includes:
  - shirt front + back
  - shorts front + back
  - socks front + back
  - design details sidebar on the right
- Socks are moved closer to the shorts in the export image
- PNG filename is:
  `achilles-kit-design-export.png`
- Product page destination:
  `https://achillessports.com/products/custom-football-kit`

## GitHub setup

Upload these files to the ROOT of your GitHub Pages repository.

Your repository should look like:

```text
index.html
.nojekyll
README.md
shopify-custom-liquid.txt
```

Then go to:

Settings → Pages

Use:

- Source: Deploy from a branch
- Branch: main
- Folder: / (root)

## Shopify setup

Open `shopify-custom-liquid.txt`.

Replace:

`YOUR_GITHUB_PAGES_URL`

with your real GitHub Pages URL, for example:

`https://YOURUSERNAME.github.io/YOUR-REPOSITORY/`

Paste that code into the Custom Liquid section on the Shopify Kit Builder page.

You do NOT need the old `config.js` for this version.
