# Haitu Casing website (Astro)

## Run locally

```bash
npm.cmd install
npm.cmd run dev
```

Open the local URL shown by Astro (usually http://localhost:4321).

## Main files
- `src/layouts/SiteLayout.astro`: shared header, footer, navigation, logo location and global styles.
- `src/pages/en/index.astro`: English homepage and 3-slide hero carousel.
- `src/pages/en/*/index.astro`: organized English second-level pages; existing public URLs are preserved.
- `src/pages/ru/*/index.astro`: organized Russian second-level pages; existing public URLs are preserved.
- `archive/homepage-drafts/`: inactive old homepage drafts, kept outside Astro routing.
- `src/pages/en/plastic-casings.astro`: plastic casing series and model detail sections.
- `src/pages/en/collagen-casings.astro` and `cellulose-casings.astro`: catalog structure placeholders to replace with verified model names.
- `public/images/`: images used by the site.

## Replace the logo
Replace `public/images/haitu-logo.svg` with your company logo converted to SVG, or change the image path in `src/layouts/SiteLayout.astro` to `/images/haitu-logo.png` if your logo is a PNG. Keep a transparent background if possible.

## Replace hero carousel photos
The English homepage rotates through three local images configured in the `slides` array in `src/pages/en/index.astro`. Use optimized landscape images and check crop behavior at desktop and mobile sizes.

The initial product-model cards and descriptions are editable draft placeholders. Verify product names, specifications, and claims before publication. No DNS settings are changed by this project.
