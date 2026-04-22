# QuoteFlow Cascos R0426 – 2 e 4 Colonne

Configuratore e generatore di preventivi/ordini per sollevatori Cascos (2 e 4 colonne).

PWA professionale per uso commerciale: funziona offline, installabile su smartphone e desktop.

## Novità rispetto alla versione 2 colonne

- Nuovo step iniziale nel wizard: scelta tra 2 colonne e 4 colonne
- 4 categorie d'impiego per i 4 colonne: Standard, Assetto ruote, Con sollevatore integrato, Industriale
- 23 nuovi modelli 4 colonne con schede tecniche PDF estraibili on-demand

## Stack

- React 18 + Vite 5
- Tailwind CSS
- vite-plugin-pwa (service worker + manifest)
- xlsx (import listino Excel)
- pdf-lib (estrazione schede tecniche da PDF cataloghi)

## Setup

```bash
npm install
npm run dev      # sviluppo locale
npm run build    # build produzione
```

## Deploy

Il workflow GitHub Actions (.github/workflows/deploy.yml) deploya automaticamente su GitHub Pages ad ogni push su main.

## Listino prezzi

I prezzi NON sono inclusi nel repository per motivi di riservatezza commerciale.
L'utente carica il listino Excel dalla dashboard della PWA e i prezzi vengono salvati nel localStorage del browser.

Formato Excel atteso: colonne "Riferimento" e "Netto Riv. (€)".

## Licenza

Uso interno Cormach Srl / PezzaliApp. Non distribuire senza autorizzazione.
