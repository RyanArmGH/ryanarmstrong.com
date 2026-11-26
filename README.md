# Static video portfolio

Plain HTML with inlined CSS and a few lines of inline JavaScript. No build step needed to host it;
no third-party requests until a visitor presses play on a video.

- `index.html` — portfolio grid. Clicking a thumbnail opens that video above the grid (`/#/<slug>/`)
  with prev / next and a back link. Without JavaScript, thumbnails link to the project pages.
- `<slug>/index.html` — one page per project. A few older addresses are kept as small redirect pages.
- Videos use a click-to-load preview: a local poster image and play button. The YouTube player
  (youtube-nocookie.com, captions off) is loaded only after a click.
- `img/thumbs`, `img/posters` — AVIF and WebP with JPEG fallback. `img/archive` — unused images kept for reference.
- `fonts/` — Jost only (SIL Open Font License), self-hosted: weights 400 and 500, Latin subset, `font-display: swap`; the 500 weight is preloaded. No Google Fonts or other font service is used. Fallback stack: Futura, Century Gothic, Trebuchet MS, sans-serif.
- `404.html`, `robots.txt`, `favicon.ico`, `favicon.png`.
