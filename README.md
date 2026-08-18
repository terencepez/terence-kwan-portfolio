# Terence Kwan Portfolio — Cloudflare Pages Static Export

This folder is a standalone, static export of the public portfolio. It is intentionally independent of the current database, owner authentication, administrator CMS, uploads, and contact-submission notification service.

## Local validation

```bash
node --check build.mjs
npm run build
```

The deployable output is `dist/`.

## Current Cloudflare Pages deployment

The static site has been published by direct upload at:

> https://terence-kwan-portfolio.pages.dev/

The Cloudflare Pages project name is `terence-kwan-portfolio`. The current output has been verified publicly on Home, Work, and Contact.

## Future Cloudflare Pages updates

1. Update the files inside `site/` and run `npm run build`.
2. In Cloudflare Dashboard, open **Workers & Pages** → `terence-kwan-portfolio`.
3. Use the Pages direct-upload flow to upload the `dist/` folder, or connect a GitHub repository for future Git-based deployments.
4. Check the provided `pages.dev` URL after each deployment.

## Static-version limitations

- Content changes require editing these static HTML files and redeploying.
- `/admin` is intentionally not included.
- The Contact page provides direct telephone and email links only. It does not submit enquiries or notify the owner.
- Images have been copied into `site/assets/` so the Cloudflare version does not rely on the existing Manus image URLs.
Cloudflare deployment connected
