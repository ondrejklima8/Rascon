# Rascon Construction — projekt

## Co je to
Jednoduchý statický web (HTML/CSS/JS, žádný framework) pro českou stavební firmu Rascon construction s.r.o.
Live: https://ondrejklima8.github.io/Rascon/

## Soubory
- `index.html` — jediná stránka (631 řádků)
- `style.css` — veškeré styly (1243 řádků)
- `main.js` — veškerá logika (456 řádků)
- `img/` — složka s obrázky (není v gitu, musíš dodat lokálně)

## Chybějící stránky (vedou na 404)
- `sluzby-retail.html`
- `sluzby-kancelare.html`
- `sluzby-rezidence.html`

## Chybějící obrázky (složka img/ není v gitu)
- `img/favicon.jpg`
- `img/logo.png`
- `img/clients/` — 17 log klientů: swarovski.jpg, hervis-sports.png, intersport.png, c-amp-a.svg, hamleys.jpg, lagard-re-paul.jpg, immofinanz.png, cpi-property-group.jpg, technopark.png, centrum-pivovar-d-n.jpg, central-most.jpg, es-te-design-amp-consulting.jpg, gemini-o-n-klinika.jpg, tipox.jpg, excipia.jpg, dehotel.jpg, umber-amp-co.jpg

## Design systém
- Barvy: `--accent: #6B9AB8`, `--bg: #fbf8f2`, `--bg-panel: #0d1419`, `--text: #0a1420`
- Fonty: DM Serif Display (nadpisy), DM Sans (text), JetBrains Mono (kódy/štítky)
- Styl: "blueprint minimalism", světlé téma, mřížka na pozadí

## Sekce v index.html (v pořadí)
1. `site-nav` — navigace (fixed, hamburger menu na mobilu pod 860px)
2. `#hero` — animovaný SVG půdorys + typewriter nadpis
3. `#stats` — 3 countery (80+ projektů, 17+ let, CZ·SK·HU)
4. `#about` — O nás (centrovaný text)
5. `#services` — 3 service karty (Retail, Kanceláře, Rezidence)
6. `#process` — 4kroková timeline
7. `#clients` — grid 5×4 loga klientů (18 buněk, z toho 1 inline SVG = Forum Liberec)
8. `#career` — kariéra
9. `#contact` — 3 karty (telefon, email, fakturační údaje) + social strip
10. footer
11. cookie modal (FAB tlačítko vlevo dole)

## Klíčové technické detaily
- i18n: CS/EN přes JS dictionary v main.js, atributy `data-i18n` a `data-i18n-html`
- Email ochrana: injektován JS za runtime (atributy `data-email-user`, `data-email-domain`)
- Scroll animace: třída `.reveal` + IntersectionObserver v main.js
- Countery: atribut `data-count-to` na `<span>`
- Mobilní menu: id=`mobile-menu`, toggle id=`mobile-toggle`
- Breakpointy: 1100px, 1024px, 860px (hamburger), 720px

## Kontakt firmy
- Tel: +420 739 316 574
- Email: info@rascon.cz
- Adresa: Hlučkova 813/12, Praha 9 — Letňany, 199 00
- IČO: 14280299, DIČ: CZ14280299
- Sociální sítě: Facebook, LinkedIn, Instagram (@rascon_construction)
