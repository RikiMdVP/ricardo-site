# ricardo-site

Personal academic website of Ricardo Martínez de Vega Perancho
(PhD candidate in Economics, Universidad de Oviedo).

Live at <https://rikimdvp.github.io/ricardo-site/>

## Structure

Static HTML and CSS, no build step, no JavaScript. Served by GitHub Pages
from the `main` branch.

| File | Purpose |
| --- | --- |
| `index.html` | Welcome page: bio, contact, research interests |
| `research.html` | Publications, working papers, work in progress |
| `teaching.html` | Courses and seminars |
| `cv.html` | Web version of the CV + PDF download |
| `404.html` | Not-found page |
| `style.css` | Single stylesheet for every page |
| `sitemap.xml`, `robots.txt` | Search-engine indexing |
| `favicon.svg`, `apple-touch-icon.png` | Icons |
| `og-image.png` | Preview card shown when a link is shared |

## Editing notes

- The header, navigation and `<head>` block are duplicated in every page.
  When adding a page, copy an existing one and update: `<title>`,
  `<meta name="description">`, `<link rel="canonical">`, the `og:` tags,
  the `aria-current="page"` marker in the nav, and `sitemap.xml`.
- Paper PDFs and slides live at the root and are linked with relative paths.
- Compress slide decks before committing (`gs -dPDFSETTINGS=/printer`);
  Git keeps every version of a binary forever.
