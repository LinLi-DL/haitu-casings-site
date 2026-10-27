# Haitu Casing website structure

## Source layout
- `src/pages/en/index.astro` and `src/pages/ru/index.astro`: language homepages.
- `src/pages/en/<page>/index.astro`: English second-level pages, organized into folders while preserving their public URLs.
- `src/pages/en/plastic-casings/<product>.astro`: individual polyamide casing detail pages.
- `src/pages/ru/<page>/index.astro`: Russian second-level pages, organized into folders while preserving their public URLs.
- `src/components/Header.astro` and `Footer.astro`: shared navigation and footer.
- `src/layouts/SiteLayout.astro`: shared document layout and global styles.
- `src/data/products.ts`: shared product category names, descriptions, images and EN/RU links.
- `public/images/`: image assets. Image locations were kept unchanged to avoid breaking references.
- `archive/homepage-drafts/`: old homepage draft files, outside `src/pages` so Astro does not publish them as active routes.

## Product priority
1. Polyamide Casings — smoke-permeable, high-barrier matte and printed options. Public URL: `/en/plastic-casings/`.
2. Collagen Casings.
3. Cellulose Casings.
4. Fibrous Casings.
5. Food Processing Equipment.

## URL and maintenance notes
The folder organization changes the source layout, not the public URLs. Existing links such as `/en/about-us/`, `/en/plastic-casings/`, `/ru/o-kompanii/` and `/ru/plastikovye-obolochki/` are retained. Product detail pages remain under `/en/plastic-casings/<product>/`.

Update product category copy and links in `src/data/products.ts`; update page content in the matching `src/pages/<language>/<page>/index.astro`. Do not add unverified technical specifications or certifications.

## Run locally
```bash
npm.cmd install
npm.cmd run dev
npm.cmd run build
```
