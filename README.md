# link-page

One-page link site for [thomasholland.link](https://thomasholland.link). Plain HTML and CSS, with self-hosted fonts. There is no build step, no analytics and no third-party requests.

## Files

- `index.html`, `style.css`: the page.
- `fonts/`: DM Sans, DM Mono and Instrument Serif, copied from [thomasholland.uk](https://thomasholland.uk).
- `favicon.svg`, `apple-touch-icon.png`, `og.png`: icons and social preview image.
- `assets/og.html`: source for `og.png` (1200×630) and `apple-touch-icon.png`. Open it in a browser and screenshot it to regenerate.

## Editing links

Links live in the `<ul class="links">` list in `index.html`. Entries marked `TODO` are placeholders with no `href`. To fill one in, replace the `<span class="link is-todo">` element with an `<a class="link" href="...">`. The Mastodon link needs `rel="me"` for profile verification.

## Hosting

Cloudflare Pages, deployed from `main` with no build command and `/` as the output directory. Custom domain: `thomasholland.link`.
