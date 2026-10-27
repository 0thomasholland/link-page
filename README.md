# link-page

One-page link site for [thomasholland.link](https://thomasholland.link). Plain HTML and CSS, with self-hosted fonts. There is no build step, no analytics and no third-party requests.

## Files

- `index.html`, `style.css`: the page.
- `fonts/`: DM Sans, DM Mono and Instrument Serif, copied from [thomasholland.uk](https://thomasholland.uk).
- `favicon.svg`, `favicon.ico`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `site.webmanifest`: favicons. `og.png`: social preview image.
- `assets/og.html`: source for `og.png` (1200×630). Open it in a browser and screenshot it to regenerate. The PNG icons are renders of `favicon.svg` on a full-bleed square.

## Editing links

Links live in the `<ul class="links">` list in `index.html`. The Twitter entry is a `TODO` placeholder with no `href`. To fill one in, replace the `<span class="link is-todo">` element with an `<a class="link" href="...">`. The Mastodon link carries `rel="me"` for profile verification, so keep it.

## Hosting

Cloudflare Pages, deployed from `main` with no build command and `/` as the output directory. Custom domain: `thomasholland.link`.

Pushes to `main` deploy automatically through the Cloudflare Pages Git connection.
