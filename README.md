# NOCT — Vercel-ready storefront

This package contains the tested responsive one-page store, the supplied product-family image, and Vercel configuration. No build step or application dependencies are required.

## Deploy with GitHub

1. Unzip the package.
2. Add the contents of `noct-vercel` to a GitHub repository. The repository root should contain `vercel.json`, `README.md`, and `dist/`.
3. In Vercel, select **Add New → Project** and import that repository.
4. Use **Other** as the framework preset, leave the build command empty, and use **dist** as the output directory. The included `vercel.json` supplies these settings.
5. Select **Deploy**.

If you add this folder to an existing repository instead, set the Vercel project's Root Directory to `noct-vercel`.

## Deploy from your terminal

With Node.js installed, open a terminal in this folder and run:

```sh
npx vercel --prod
```

Sign in and follow the Vercel prompts to create or select your project.

## Files

- `dist/index.html` — page layout and metadata
- `dist/style.css` — visual direction and responsive layout
- `dist/app.js` — three products, product details, and cart logic
- `dist/product-family.png` — supplied product photograph
- `vercel.json` — static hosting configuration

The cart is held in memory and resets on reload. There is no checkout, payment collection, account system, or backend. Product specifications and prices are proposed concepts. The supplied photograph intentionally omits the kit's graphics; the detail view identifies that difference.

Checks completed: three products total INR 49,000; quantity increases, decreases, removals, and empty cart; adding from product details; mobile layouts at 320 and 390 pixels; desktop layout at 1280 pixels; crop zoom values 1.10, 1.00, and 1.05; keyboard dismissal of product details. Vercel deployment has not been performed.

Vercel configuration reference: https://vercel.com/docs/project-configuration/vercel-json
