# Portfolio

Osobní portfolio — statický web (HTML/CSS/JS, bez buildu), nasazovaný na GitHub Pages.

## Struktura

- `index.html` — hlavní stránka (O mně, Projekty)
- `studium.html` — přehled studia po semestrech (rozbalovací seznam předmětů)
- `cv.html` — profesní CV, náhled PDF přes pdf.js + odkaz ke stažení
- `styles.css` — vzhled, barvy a typografie (tmavé téma, animace)
- `script.js` — doplnění aktuálního roku v patičce
- `uploads/` — statické soubory (fotka, `CV_Vala.pdf`)
- `.github/workflows/deploy.yml` — automatické nasazení na GitHub Pages při pushi do `main`

## Úprava obsahu

- **O mně / úvodní text** — `index.html`, sekce `.hero`
- **Projekty** — `index.html`, sekce `#projects` (každý projekt jako `<li class="entry">`)
- **Studium** — `studium.html`, jednotlivé `<details class="sem">` po semestrech
- **CV** — nahraď `uploads/CV_Vala.pdf` vlastním souborem se stejným názvem (nebo uprav cestu v `cv.html`)

## Lokální náhled

Stačí otevřít `index.html` v prohlížeči, nebo spustit lokální server, např.:

```bash
python3 -m http.server 8000
```

a otevřít `http://localhost:8000`.

## Nasazení na GitHub Pages

1. V repozitáři jdi do **Settings → Pages**.
2. U **Build and deployment → Source** vyber **GitHub Actions**.
3. Po pushnutí do `main` proběhne workflow `Deploy Portfolio to GitHub Pages` a web bude dostupný na
   `https://<uživatel>.github.io/<repo>/`.
