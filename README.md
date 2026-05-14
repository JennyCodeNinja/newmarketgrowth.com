# New Market Growth — Website

Static marketing site for [newmarketgrowth.com](https://www.newmarketgrowth.com/).

## Stack

Single-file static HTML. No build step, no framework, no dependencies. Edit `index.html` and the change is live.

- HTML/CSS, vanilla
- Hosted on [Cloudflare Pages](https://pages.cloudflare.com/) (auto-deploys on every push to `main`)
- Fonts via Google Fonts CDN (Plus Jakarta Sans)
- Form handling: Typeform (external)
- No JavaScript dependencies

## File map

```
.
├── index.html              The website
├── favicon.png             32×32 browser tab icon
├── apple-touch-icon.png    180×180 iOS home-screen icon
├── og-image.png            1200×630 social link preview (LinkedIn, Slack, etc.)
├── carlos-caro.jpg         Founder headshot
├── robert-cezeaux.jpg      Managing partner headshot
├── nmg-web-logos/          Marketplace partner logos
├── robots.txt              Search engine crawl rules
├── sitemap.xml             Single-page sitemap
└── llms.txt                LLM-friendly site description
```

## Making edits

The site is one HTML file. Common edits:

- **Copy changes:** edit the text directly in `index.html`. Search for the sentence you want to change, edit it, commit.
- **Add a new Toaster episode:** find the `<section id="toaster">` block and copy the pattern of an existing `<a class="piece-card">` block.
- **Swap a marketplace logo:** drop the new SVG/PNG into `nmg-web-logos/`, then update the matching `<img src=...>` line in `index.html`.
- **Update headshots:** replace `carlos-caro.jpg` or `robert-cezeaux.jpg` with new files of the same name (max 640×640, JPEG, ~80–120KB).

## Deploy

Auto-deploys to Cloudflare Pages on every push to `main`. Typical deploy time: under 60 seconds.

## Contact

[carlos@newmarketgrowth.com](mailto:carlos@newmarketgrowth.com)
