# jouster-skutsje — design files

Static HTML mockups for the redesign of [jousterskutsje.nl](https://www.jousterskutsje.nl/). The ship is the **Oeral Thús**, the 1924 Jouster skûtsje, which sails the **SKS skûtsjesilen** championship.

## Round 2 — blue/orange, real photos, news & agenda first

Twelve genuinely different directions. Open `index.html` to compare. Round 1 (heritage serif) was scrapped.

| File | Direction | Feel |
|------|-----------|------|
| `index.html` | Gallery | Compare all twelve directions |
| `variant-1-wedstrijdcentrale.html` | Wedstrijdcentrale | Sport/broadcast. Dark hero, orange live-band, the full race calendar as the centerpiece. |
| `variant-2-krant.html` | De Krant | News-first newspaper front page. Masthead, lead story, agenda as a fixed sidebar. |
| `variant-3-poster.html` | Poster | Bold graphic. Huge Anton type, colour blocks, a sail-shaped photo, agenda as a poster list. |
| `variant-4-helder.html` | Helder | Clean card system. Agenda and Nieuws side by side, both prominent. |
| `variant-5-op-het-water.html` | Op het water | Cinematic. Full-bleed photo hero with a floating agenda card overlapping it. |
| `variant-6-logboek.html` | Logboek | Data-forward. Race schedule table, standings, news feed, dashboard style. |
| `variant-7-tijdlijn.html` | Tijdlijn | Centennial timeline as the spine: 1924 → 2026, culminating in the agenda. |
| `variant-8-kaart.html` | Op de kaart | SKS route plotted on a stylized map of the Frisian lakes; agenda tied to geography. |
| `variant-9-diptych.html` | Diptych | Split-screen: fixed identity/photo panel left, scrolling agenda + news right. |
| `variant-10-clubhuis.html` | Clubhûs | Heraldic sports-club identity: crest, fixtures list, squad (Oswald condensed). |
| `variant-11-raster.html` | Raster | Brutalist mono grid: hard borders, monospace, zine/terminal aesthetic. |
| `variant-12-wimpels.html` | Wimpels | Nautical signal-flag system: every race gets its own flag, bunting, playful. |

Display fonts vary per variant for distinct feel: Barlow Condensed (1), Archivo (2/5/9/12), Anton (3), Inter (4/6), Space Grotesk (7/8), Oswald (10), IBM Plex Mono (11).

## Research baked in

- **Skûtsjesilen** — competitive sailing of historic Frisian flat-bottomed cargo ships (skûtsjes), a 180-year tradition. The **SKS** (Sintrale Kommisje Skûtsjesilen) runs the championship; only skippers from the old Frisian skipper families may compete.
- **Real SKS agenda 2026** used throughout: championship 18–31 July (Grou → De Veenhoop → Earnewâld → Terherne → Langweer → rest day → Stavoren → Woudsend → Elahuizen → Lemmer I → Lemmer II → Sneek), plus foarwedstriden from 30 May and the na-seizoen in September.
- **Real news** items: "Oeral Thús weer uit de Kolk" (9 apr 2026), "Wedstrijdkalender 2026 bekend" (4 mrt 2026), "Jouster Skûtsje derde plek" (1 aug 2025).

## Design system

- **Colours from the logo:** blue + vivid orange (`#f24e0e`-ish), with deep navy and white. oklch tokens in each file's `@theme`.
- **Type:** Inter (body, rsms.me) + IBM Plex Mono (data/eyebrows). Display font varies per variant for distinct feel: Barlow Condensed (V1), Archivo (V2/V5), Anton (V3), Inter (V4/V6).
- **Photos are real**, downloaded from the live site into `assets/`: `logo.png`, `logo-footer.png` (white), `news-kolk.jpeg`, `sail-2.jpg`, `sail-3.jpg`, `detail-lieren.png`. Swap/extend with the club's full photo library in the build.
- Dutch copy, no em-dashes, NL/FY toggle, accessible (role="list", focus-visible, alt text).

## Next step

Pick a direction (mixing is fine, e.g. Wedstrijdcentrale's calendar with Helder's card clarity). I expand the winner into the full page set (Home, Agenda, Over ons / Historie / Bemanning / Bestuur, Sponsoring, Merchandise, Club van 100, Contact) and then to a WordPress FSE parent/child theme.
