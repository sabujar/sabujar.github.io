# Sheikh Abujar — Academic Website

A clean, self-contained academic website. No build step, no framework — just
HTML + CSS + a tiny bit of JavaScript. Deploys directly to GitHub Pages.

## Structure

```
sabujar.github.io/
├── index.html          # About / home
├── research.html       # Research projects
├── publications.html   # Publication list
├── teaching.html       # Teaching, experience, education, awards
├── assets/
│   ├── css/style.css   # All styling (light + dark mode)
│   ├── js/theme.js     # Light/dark toggle
│   ├── img/            # → add headshot.jpg here
│   └── cv/             # → add Sheikh_Abujar_CV.pdf here
└── README.md
```

## Before it goes live — two things to add

1. **Headshot** — save a square photo as `assets/img/headshot.jpg`, then in
   `index.html` replace the `<div class="headshot-placeholder">…</div>` block with:
   ```html
   <img class="headshot" src="assets/img/headshot.jpg" alt="Sheikh Abujar">
   ```
2. **CV PDF** — compile your LaTeX CV and save it as
   `assets/cv/Sheikh_Abujar_CV.pdf` (all the "CV" links already point there).

## Deploy to GitHub Pages

1. Create a public repo named **`sabujar.github.io`** on GitHub.
2. Push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial academic website"
   git branch -M main
   git remote add origin https://github.com/sabujar/sabujar.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source → Deploy from branch → `main` / root**.
4. Your site goes live at **https://sabujar.github.io** within a minute or two.

## Editing tips

- Colors, fonts, and spacing are all controlled by the `:root` variables at the top
  of `assets/css/style.css` — change the accent color in one place.
- To add a news item, publication, or project, copy an existing block and edit it.
- Dark mode follows the visitor's system setting and can be toggled with the ☾ button.

## Custom domain (optional, later)

Buy a domain (e.g. `sheikhabujar.com`), add a file named `CNAME` containing the
domain, and point the domain's DNS at GitHub Pages.
