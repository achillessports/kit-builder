ACHILLES KIT BUILDER - SHOPIFY IFRAME CART FIX

1. GITHUB
Replace your existing index.html in the GitHub Pages repository with the index.html in this folder.
Keep config.js. It should contain:

window.ACHILLES_CONFIG = {
  shopifyDomain: "90fe1f-84.myshopify.com",
  variantId: "57150364811588",
  quantity: 1,
  returnTo: "/cart"
};

Commit the change and let GitHub Pages publish it.

2. SHOPIFY
Open shopify-custom-liquid.txt.
Replace BOTH occurrences of YOUR_GITHUB_PAGES_URL with the exact GitHub Pages URL for your builder, including https:// and the final / if your URL uses one.

Example only:
https://username.github.io/achilles-kit-builder/

Then paste the complete contents into the Custom Liquid section on your Shopify Kit Builder page, replacing the old iframe code.

3. TEST
Open the Shopify Kit Builder page, customise the kit, then press Add kit to cart.
The iframe sends the design to the parent Shopify page. Shopify calls its own /cart/add.js endpoint and redirects to /cart.

Variant configured: 57150364811588
