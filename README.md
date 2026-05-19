# Portfolio

A personal portfolio site built with plain HTML and CSS, hosted on GitHub Pages.

**Live site**: `https://yourusername.github.io`

---

## Running locally

No build step required. Just clone the repo and open the file:

```bash
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io
open index.html
```

Or drag `index.html` into your browser directly.

---

## File structure

```
├── index.html        # All markup and content
├── style.css         # All styles and CSS variables
├── README.md
└── assets/           # Images, icons, or other static files (if any)
```

---

## Customising the palette

All colours are defined as CSS variables at the top of `style.css` inside `:root`. To change the palette, update these four values:

```css
:root {
  --bg: #DDE6ED;        /* Page background */
  --ink: #27374D;       /* Headings and body text */
  --ink-muted: #526D82; /* Secondary text, accent colour */
  --ink-faint: #9DB2BF; /* Hints, borders, placeholders */
}
```

Everything else — buttons, tags, dividers, nav — references these variables and will update automatically.

---

## Updating content

**Projects** — each project is a `.project-card` div inside the `#projects` section in `index.html`. Copy an existing card and update the title, description, tags, and status badge (`status-planned`, `status-wip`, or `status-live`).

**Skills** — each skill is a `.skill-item` div inside the `#about` section. Update the `.skill-name` and `.skill-tag` text.

**Contact links** — find the `.contact-links` div near the bottom of `index.html` and update the `href` attributes and link labels.

**Nav links** — update the `<ul class="nav-links">` list in the `<nav>` element at the top of `index.html`.

---

## Fonts

This site uses [DM Sans](https://fonts.google.com/specimen/DM+Sans), [DM Serif Display](https://fonts.google.com/specimen/DM+Serif+Display), and [DM Mono](https://fonts.google.com/specimen/DM+Mono) via Google Fonts, loaded in the `<head>` of `index.html`.

To swap fonts, replace the Google Fonts `<link>` tag and update the corresponding variables in `:root`:

```css
--mono: 'DM Mono', monospace;
--serif: 'DM Serif Display', serif;
--sans: 'DM Sans', sans-serif;
```

---

## Deployment

The site is hosted on [GitHub Pages](https://pages.github.com/) and deploys automatically on every push to `main`.

```bash
git add .
git commit -m "your message"
git push origin main
```

Changes are live within a minute or two. The repository must be named `yourusername.github.io` for the root URL to work, or configure a custom domain under **Settings → Pages**.
