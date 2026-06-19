# jouster-skutsje — design files

Static HTML mockups for the redesign of [jousterskutsje.nl](https://www.jousterskutsje.nl/). The ship is the **Oeral Thús**, the 1924 Jouster skûtsje, which sails the **SKS skûtsjesilen** championship.

## Shortlist — blue/orange, real photos, news & agenda first

Six selected directions (narrowed down from twelve). Open `index.html` to compare. Round 1 (heritage serif) was scrapped.

| File | Direction | Feel |
|------|-----------|------|
| `index.html` | Gallery | Compare the six directions |
| `variant-1-krant.html` | De Krant | News-first newspaper front page. Masthead, lead story, agenda as a fixed sidebar. |
| `variant-2-poster.html` | Poster | Bold graphic. Huge Anton type, colour blocks, a sail-shaped photo, agenda as a poster list. |
| `variant-3-op-het-water.html` | Op het water | Cinematic. Full-bleed photo hero with a floating agenda card overlapping it. |
| `variant-4-diptych.html` | Diptych | Split-screen: fixed identity/photo panel left, scrolling agenda + news right. |
| `variant-5-clubhuis.html` | Clubhûs | Heraldic sports-club identity: crest, fixtures list, squad (Oswald condensed). |
| `variant-6-raster.html` | Raster | Brutalist mono grid: hard borders, monospace, zine/terminal aesthetic. |

Display fonts vary per variant for distinct feel: Anton (Poster), Oswald (Clubhûs), IBM Plex Mono (Raster), Archivo (rest).

Live at **https://skutsje.autive.dev** (see [skutsje-hosting] notes). Earlier directions removed in this round: Wedstrijdcentrale, Helder, Logboek, Tijdlijn, Op de kaart, Wimpels.

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
