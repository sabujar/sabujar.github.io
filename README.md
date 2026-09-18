# Sheikh Abujar — Academic Website

A single, self-contained `index.html` in the plain, classic style of a traditional
CS faculty homepage. No framework, no build step, no external fonts — just
Times/serif HTML that loads instantly and
deploys straight to GitHub Pages.

## Structure

```
sabujar.github.io/
├── index.html          # the entire site (all content, inline CSS)
├── assets/
│   ├── img/            # → add headshot.jpg here (shows automatically)
│   └── cv/             # historical LaTeX source (not linked)
└── README.md
```

## Assets

1. **Headshot** — save a photo as `assets/img/headshot.jpg`. It appears at the top
   automatically; if the file is missing, the page simply omits it.
2. **CV** — no CV PDF is published or linked, at the owner's request.
   The existing LaTeX source is historical; the homepage uses the September 2026
   academic CV supplied separately.

## Editing

Everything lives in `index.html`. To add a publication, award, or talk, copy an
existing line and edit it. All styling is the small `<style>` block in the `<head>`.
Update the footer's explicit last-updated date when changing the content.
The homepage was synchronized with the supplied academic CV on September 18, 2026.
`v2.html` and `versions/` are historical design alternatives, not maintained profiles.

## Deploy

The repo `sabujar.github.io` is already published via GitHub Pages at
<https://sabujar.github.io>. To update: `git add -A && git commit -m "..." && git push`.

> The earlier multi-page version (separate Research/Publications/Teaching/Service
> pages with a stylesheet and dark-mode toggle) remains in the git history if ever
> needed.
