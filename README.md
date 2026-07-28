# URBO image assets

This package contains 34 source images converted into responsive WebP variants.

## Size reduction

- Original uploaded images: 96.5 MB
- All optimised variants combined: 5.8 MB
- Each image has a `large` and `small` version.

## Upload to GitHub

1. Create a public repository called `urbo-assets`.
2. Open the repository and choose **Add file → Upload files**.
3. Upload everything inside this folder:
   - `images`
   - `index.html`
   - `assets-manifest.json`
   - `vercel.json`
4. Commit the files.

Do not upload the unopened ZIP. Extract it first, then upload its contents.

## Deploy on Vercel

1. In Vercel choose **Add New → Project**.
2. Import the `urbo-assets` GitHub repository.
3. No build command or framework is required.
4. Deploy.

After deployment, an image URL will look like:

`https://urbo-assets.vercel.app/images/olivers-coffee-bar/olivers-homepage-large.webp`

## Use in a Hostinger embed

```html
<picture>
  <source
    media="(max-width: 700px)"
    srcset="https://urbo-assets.vercel.app/images/olivers-coffee-bar/olivers-homepage-small.webp"
  >
  <img
    src="https://urbo-assets.vercel.app/images/olivers-coffee-bar/olivers-homepage-large.webp"
    width="2400"
    height="1500"
    loading="lazy"
    decoding="async"
    alt="Oliver's Coffee Bar website"
  >
</picture>
```

The exact file paths and dimensions are listed in `assets-manifest.json`.
