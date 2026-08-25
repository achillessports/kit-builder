# Achilles Sports Kit Builder - GitHub Pages

This folder is ready to host as a static GitHub Pages site.

## Files

- `index.html` - the full 3D Achilles kit builder
- `config.js` - your Shopify store domain and product variant ID
- `.nojekyll` - tells GitHub Pages to serve the site as plain static files
- `.gitignore` - ignores common local system files

## 1. Configure Shopify

Open `config.js` and replace these values:

```js
window.ACHILLES_CONFIG = {
  shopifyDomain: "YOUR-STORE.myshopify.com",
  variantId: "YOUR_NUMERIC_VARIANT_ID",
  quantity: 1,
  returnTo: "/cart"
};
```

Use the numeric Shopify variant ID, not a `gid://shopify/ProductVariant/...` value.

## 2. Upload to GitHub

Create a repository such as `achilles-kit-builder` and upload everything in this folder to the repository root.

The repository root should look like:

```text
achilles-kit-builder/
├── index.html
├── config.js
├── .nojekyll
├── .gitignore
└── README.md
```

Do not put these files inside an extra nested folder.

## 3. Turn on GitHub Pages

In the repository:

1. Open **Settings**.
2. Open **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main**.
5. Select folder **/ (root)**.
6. Click **Save**.

GitHub should publish the site at a URL like:

`https://YOUR-USERNAME.github.io/achilles-kit-builder/`

## 4. Optional custom domain

In **Settings > Pages**, add a custom domain such as:

`builder.achillessports.co.uk`

Then configure the required DNS record with whoever manages your domain.

## Shopify checkout behaviour

The kit builder does not use a Storefront API token. When the customer presses Add to Cart, it submits a normal product form directly to your Shopify store and passes the kit customisation values as line-item properties.

## Important

GitHub Pages is suitable for static hosting and testing. GitHub's published Pages limits say it is not intended to be used as free hosting for a commercial online business or e-commerce site. If you use this as a live customer-facing commercial builder, review GitHub's current Pages terms and limits first.
