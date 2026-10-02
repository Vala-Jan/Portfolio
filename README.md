# Portfolio

Osobní portfolio — statický web (HTML/CSS/JS, bez buildu), nasazovaný na GitHub Pages.

## Struktura

- `index.html` — hlavní stránka (O mně, Projekty)
- `styles.css` — vzhled, barvy a typografie (tmavé téma, animace)
- `uploads/` — statické soubory (fotka, `CV_Vala.pdf`)
- `.github/workflows/deploy.yml` — automatické nasazení na GitHub Pages při pushi do `main`

## Úprava obsahu

- **O mně / úvodní text** — `index.html`, sekce `.hero`
- **Projekty** — `index.html`, sekce `#projects` (každý projekt jako `<li class="entry">`)
- **Studium** — `studium.html`, jednotlivé `<details class="sem">` po semestrech
- **CV** — nahraď `uploads/CV_Vala.pdf` vlastním souborem se stejným názvem (nebo uprav cestu v `cv.html`)
