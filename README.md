# Haitu Casing website (Astro)

## Run locally

```bash
npm.cmd install
npm.cmd run dev
```

Open the local URL shown by Astro (usually http://localhost:4321).

## Main files
- `src/layouts/SiteLayout.astro`: shared header, footer, navigation, logo location and global styles.
- `src/pages/en/index.astro`: English homepage and 4-image hero carousel.
- `src/pages/en/plastic-casings.astro`: plastic casing series and model detail sections.
- `src/pages/en/collagen-casings.astro` and `cellulose-casings.astro`: catalog structure placeholders to replace with verified model names.
- `public/images/`: images used by the site.

## Replace the logo
Replace `public/images/haitu-logo.svg` with your company logo converted to SVG, or change the image path in `src/layouts/SiteLayout.astro` to `/images/haitu-logo.png` if your logo is a PNG. Keep a transparent background if possible.

## Replace hero carousel photos
The English homepage currently rotates through four local image files every 5 seconds: `hero-products-preview.jpg`, `plastic-casings-preview.jpg`, `collagen-casings-preview.jpg`, and `cellulose-casings-preview.jpg`. Replace these files with your selected photos (keep the same filenames), or update the `slides` array in `src/pages/en/index.astro`. Use optimized landscape images, ideally around 1400 x 900 pixels.

The initial product-model cards and descriptions are editable draft placeholders. Verify product names, specifications, and claims before publication. No DNS settings are changed by this project.
