# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static HTML/CSS served by GitHub Pages from `main`, repository root (`.nojekyll`). No JavaScript, cookies, forms, analytics, or third-party resources: the privacy policy (`confidentialitate/`) states this, so fonts and images must be self-hosted. Confirmed by the owner, 12 October 2026.

## Users

Two audiences, weighted equally:

- Classic Romanian crossword solvers (rebusiști) who grew up with paper careuri and the morning coffee ritual.
- Casual phone players (Wordle, Sudoku habits) looking for a short, calm break.

Secondary: existing players who arrive from the App Store looking for support, purchase restoration, or privacy information.

## Product Purpose

Rebus la cafea is an iPhone app of Romanian crosswords (careuri) written in Romanian, with real diacritics. The site persuades visitors to download it from the App Store and serves as the app's public support and privacy pages (the URLs are registered in App Store Connect).

## Positioning

Careuri written for Romanian from the start: Ă, Â, Î, Ș, Ț are distinct letters in the grid with a dedicated key row, clues are original and playful, and there are no ads, ever. Paid once (Premium), never a subscription.

## Operating Context

- Played in short breaks, typically with coffee; no timer, no penalties.
- Works offline; progress saves locally and syncs through iCloud (free).
- Visitors reach the site from the App Store listing (support/privacy links), shared links (Open Graph image), and search.
- App Store link: `https://apps.apple.com/ro/app/id6819084037?pt=129528005&ct=site&mt=8` (campaign-tagged).

## Capabilities and Constraints

- Content as of version 1.1 (live on the App Store since 12 Oct 2026; the site describes 1.1): 100 permanently free main careuri; Premium has 40 (the general collection of 30 plus the thematic pack „Strigoi și dovleci”); 140 main careuri total. Sizes 5×5 to 7×7. Premium includes new thematic packs added through app updates, with no promised cadence or end date; never present future themes as available.
- „Strigoi și dovleci”: 10 careuri of Romanian night folklore (strigoi, moroi, iele, Sfântul Andrei), 2 Ușor / 3 Mediu / 5 Greu; the first, „Musafiri deghizați”, is a free sample; „Miezul nopții” is the special challenge. In-app event 18 Oct – 3 Nov 2026; the site may feature it in a temporary, removable section.
- „Careul zilei”: a free series of 60 daily 9 × 9 challenges, one per day by Romanian time, starting the day the app is first opened; past days stay in an archive, future days are locked; no new dailies are promised after day 60.
- Free helpers: „Verifică”, „O literă”, „Indiciu”; explanations after a word is solved.
- iCloud sync included free; no account; no tracking.
- Price is set by Apple and shown in-app; the site must not state a price.
- The app's own source (`../rebus-la-cafea`, DESIGN.md, Docs/APP_STORE.md) is the reference for product facts; its `SupportSite/` folder is behind this repository.
- Root URL must keep the support content and FAQ reachable (`#suport`); privacy lives at `/confidentialitate/` with anchor `#mesaje-suport`.
- Contact: rebuslacafea@icloud.com. Publisher: Eddie Roman.

## Brand Commitments

- Name: „Rebus la cafea”. Romanian-language site, Romanian quotation marks („…”).
- App icon (green mug with an „R” crossword square and steam) stays. All other visual decisions (colour, type, composition) are free; the app's palette is not binding on the site.
- Promise: no ads, now or later („Fără reclame, pentru totdeauna”).
- Voice: warm, calm, plain Romanian; not corporate, not childish.

## Evidence on Hand

- Real iPhone screenshots in `img/` (from the app repo's `Builds/Screenshots-2026-10-12/iPhone-17-Pro-Max/`, light and dark): `ecran-03-game-typing` (Careul 1 with the Ă Â Î Ș Ț keyboard), `ecran-08-completion` („Careu gata.”), `ecran-11-daily` (Ziua 3 din 60), `ecran-01-home` (Acasă with „Strigoi și dovleci”). Higher-resolution captures of every screen live in that folder.
- Real clues used on the site: careu-02 „Încă o înghițitură”, 1 Orizontal ROȘU „Culoarea sângelui și a macului.”; strigoi-01, BUHĂ „Pasăre de noapte, rudă cu bufnița.”
- Icon assets: `img/apple-touch-icon.png`, `img/favicon-32.png`; share card `img/og-image.png`.
- Real puzzle data in the app repo (`Rebus/Resources/puzzles.json`, `daily.json`), e.g. careu-02 „Încă o înghițitură” (ROȘU, COVOR, RECUL, TREN, VAS) and strigoi-01 „Musafiri deghizați” (CEAȚĂ, COSTUM, BUHĂ, LUP, MASCĂ).
- Icon SVG sources: `../rebus-la-cafea/Tools/app-icon*.svg`.
- No testimonials, reviews, ratings, press, or download numbers exist. Do not invent them.

## Product Principles

1. Romanian first: the language is the product, not a localisation.
2. Calm over compulsion: no ads, timers, streak pressure, or dark patterns.
3. Honest and specific: real counts, real clues, no invented claims or prices.
4. Support is part of the product: answers stay easy to find from the App Store link.

## Accessibility & Inclusion

Audience includes older readers: generous text size, strong contrast, 44px+ targets, works without JavaScript, respects reduced motion and light/dark preference.
