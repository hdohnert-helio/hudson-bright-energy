# Hudson Bright Energy — website

Static website for Hudson Bright Energy, an independent residential solar
consulting business serving CT, NY, MA and NJ. Hosted on GitHub Pages.

Plain HTML and one stylesheet. No frameworks, no build step, no JavaScript,
no cookies or trackers.

## Files

| File | What it is |
|---|---|
| `index.html` | Home page (hero, services, how it works, contact form) |
| `privacy.html`, `terms.html`, `accessibility.html` | Legal pages |
| `thank-you.html` | Shown after the contact form is submitted |
| `404.html` | "Page not found" |
| `styles.css` | All styling (colors are variables at the top) |
| `favicon.svg`, `robots.txt`, `sitemap.xml` | Browser icon and search-engine files |

## Editing

1. Open the page on github.com, click the pencil icon, edit the text, and
   click **Commit changes**. The live site updates within about a minute.
2. The header and footer are repeated in every page — if you change one,
   change it in all of them.
3. If you change a legal page, update its "Last updated" date.

## Contact form

The form posts to [Formspree](https://formspree.io), which emails each
submission. The endpoint is the `action="..."` on the `<form>` in
`index.html`; the post-submit redirect is the hidden `_next` field.

## Custom domain (later)

Add the domain under **Settings → Pages**, then replace
`https://hdohnert-helio.github.io/hudson-bright-energy/` in every page's
canonical/Open Graph tags, the form's `_next` field, `robots.txt` and
`sitemap.xml`, and change `/hudson-bright-energy/` to `/` in `404.html`.
