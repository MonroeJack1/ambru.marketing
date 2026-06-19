# Ambru Marketing

Site static one-page pentru domeniul `ambru.marketing`.

## Fișiere principale

- `index.html` - structura paginii și conținutul în limba română
- `styles.css` - design responsive, dark premium, accent auriu
- `script.js` - meniul mobil și anul din footer
- `CNAME` - domeniul custom pentru GitHub Pages
- `.github/workflows/pages.yml` - deploy static prin GitHub Actions, dacă alegi sursa „GitHub Actions” în Pages
- `robots.txt` și `sitemap.xml` - fișiere SEO de bază

## Publicare pe GitHub Pages

1. Creează repository-ul, de exemplu `ambru.marketing` sau `<username>.github.io`.
2. Urcă toate fișierele din acest folder în branch-ul `main`.
3. În GitHub, mergi la **Settings → Pages**.
4. Alege una dintre variante:
   - **Deploy from a branch**: selectează `main` și folderul `/root`.
   - **GitHub Actions**: folosește workflow-ul inclus în `.github/workflows/pages.yml`.
5. La **Custom domain**, setează `ambru.marketing`.
6. Configurează DNS la providerul domeniului.

## DNS recomandat pentru apex domain

Pentru `ambru.marketing`, setează patru recorduri `A` către GitHub Pages:

```txt
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Pentru `www.ambru.marketing`, setează un `CNAME` către domeniul GitHub Pages al contului tău, de forma:

```txt
<username>.github.io
```

După propagare, activează **Enforce HTTPS** în GitHub Pages.
