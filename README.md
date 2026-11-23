# keval-devani.github.io

My personal portfolio, live at **https://keval-devani.github.io**.

Plain HTML, CSS and a little JavaScript, served as-is by GitHub Pages. No framework, no build step.

## Files

- `index.html` – the portfolio page
- `resume.html` – resume as a web page, also used for the PDF
- `assets/Keval-Devani-Resume.pdf` – resume download
- `assets/css/style.css` – styles (colors and fonts are variables at the top, dark mode included)
- `assets/js/main.js` – theme toggle and mobile menu
- `assets/img/` – photo, favicon and the link preview image
- `og.html` – layout used for the link preview image

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Updating

- Edit content directly in `index.html` and `resume.html`.
- To refresh the PDF, open `resume.html` in a browser and print to PDF (A4, no headers or footers), saving over `assets/Keval-Devani-Resume.pdf`.
- Push to `main` to publish.
