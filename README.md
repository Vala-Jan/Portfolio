# Portfolio

Osobní portfolio — statický web (HTML/CSS/JS, bez buildu), nasazovaný na GitHub Pages.

## Struktura

- `index.html` — obsah stránky
- `styles.css` — vzhled, barvy a typografie (světlý/tmavý režim)
- `script.js` — přepínač motivu a drobné doplňky
- `.github/workflows/deploy.yml` — automatické nasazení na GitHub Pages při pushi do `main`

## Úprava obsahu

Vlastní texty, projekty a odkazy uprav přímo v `index.html`:

- **O mně** — sekce `#about`
- **Dovednosti** — sekce `#skills`
- **Projekty** — sekce `#projects` (styl "changelogu", každý projekt jako jedna položka `<li class="entry">`)
- **Kontakt** — sekce `#contact` (email, GitHub, LinkedIn)

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
