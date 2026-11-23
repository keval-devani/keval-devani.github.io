# keval-devani.github.io

Personal portfolio of **Keval Devani**, Senior Flutter & Mobile IoT Engineer.
Live at **https://keval-devani.github.io**.

Plain HTML, CSS and a little JavaScript. No framework and no build step: GitHub Pages serves the files as they are.

## Structure

| Path | What it is |
|---|---|
| `index.html` | The portfolio page (all sections and content) |
| `resume.html` | Print-friendly resume page; the PDF is generated from it |
| `assets/Keval-Devani-Resume.pdf` | Resume download linked from the page |
| `assets/css/style.css` | All styles. Colors are CSS variables at the top; dark mode included |
| `assets/js/main.js` | Theme toggle, mobile menu, scroll reveal (optional enhancements) |
| `assets/img/` | Avatar, favicon, touch icon, social preview image (`og-image.png`) |
| `og.html` | Source for `og-image.png` (not linked from the site) |
| `404.html`, `robots.txt`, `sitemap.xml` | Not-found page and SEO files |

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Updating content

- **Text, projects, experience:** edit `index.html` directly. Each section is commented.
- **Resume:** edit `resume.html`, then regenerate the PDF with any Chromium browser:

  ```bash
  "/Applications/Brave Browser.app/Contents/MacOS/Brave Browser" --headless --no-pdf-header-footer \
    --print-to-pdf=assets/Keval-Devani-Resume.pdf resume.html
  ```

- **Social preview image:** edit `og.html`, then:

  ```bash
  "/Applications/Brave Browser.app/Contents/MacOS/Brave Browser" --headless --hide-scrollbars \
    --window-size=1200,630 --screenshot=assets/img/og-image.png og.html
  ```

## Deploy

Push to `main`. GitHub Pages is set to deploy from `main` / root.
