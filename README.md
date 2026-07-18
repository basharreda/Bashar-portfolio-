# Bashar Reda — Portfolio Website

A single-file, self-contained HTML portfolio for graphic/motion designer **Bashar Reda**. Dark theme with an acid-green (`#b8ff00`) accent, built for a fast, media-rich browsing experience — every image, illustration, and presentation slide is embedded directly in the HTML as base64, so the whole site works offline from one file with no external assets or build step.

## Live file

`bashar-portfolio.html` — ~79 MB, single file, no dependencies.

Just open it in any browser, or upload it to any static host (GitHub Pages, Netlify, etc.) as `index.html`.

## Structure

The page is a single scrolling site with the following sections, in order:

1. **Hero** — large avatar, bold "BASHAR" background typography, nav bar, stats strip.
2. **Clients** — grid of 15 organizations Bashar has worked with, each with a real logo image (eYouth, IBM, EFE, J.P. Morgan, Ministry of Communications & IT, Digilians, DEBI, Halaly Pets, Rafef, Vevian, InRide, The Beauty Mom, Sinai White Cement, Rwad Misr, Ashbal Misr El-Raqmeya).
3. **Experience** — work history timeline (eYouth, ACE Marketing, Global IMC, Morgan Advertising, Patmos, Freelance).
4. **Skills** — core tool proficiency (Photoshop, Illustrator, After Effects).
5. **Portfolio** — the main showcase, organized into 8 tabs:
   | Tab | Content |
   |---|---|
   | **Social Media** | 48 real campaign images (Halaly Pets, Rafif Beauty, The Beauty Mom, Sinai White Cement, eYouth, IBM SkillsBuild, EFE, Digilians, Rwad Misr, Baraaem Misr, and more) |
   | **Branding** | 4 external case-study links (Behance) — Karakenyo, Imaginary Brand Identity, Nova Photography, Tak Store |
   | **Presentation Design** | 5 embedded slide decks, viewable in a built-in slide viewer — Program Overview, Q1 2026 Report, DECI, PMO October Report, Karakenyo Company Profile |
   | **Print Design** | 18 outdoor/print mockups — metro posters, brochures, banners, billboards, ID badges, stickers, packaging |
   | **Typography** | 2 Arabic typography design pieces |
   | **Illustrations** | 8 vector/digital art pieces |
   | **Play Store Screens** | 6 InRide app marketing screens, shown in their native portrait aspect ratio |
   | **Menu** | External link to an interactive digital menu build (Karakenyo) |
6. **Education** — Cairo University, Computers & AI, Information Systems / Decision Support (2020).
7. **Contact** — acid-green call-to-action block with email/phone/location.
8. **Footer**.

## How images and decks work

- **Image grids** (Social Media, Illustrations, Typography, Play Store, part of Print Design) use a shared lightbox: clicking any thumbnail opens `openLB(index, category)`, which pulls from a matching JS data array (`socialData`, `illustrationData`, `typographyData`, `playstoreData`, `printData`). The array index and the grid's click index must always match 1:1.
- **Presentation decks** use a separate slide viewer (`openDeck(key)`), backed by `presentationDecks` (slide images per deck) and `deckTitles` (display names).
- **Branding** and **Menu** are simple external link cards that open the linked page (Behance, or a live site) in a new tab — no embedded images.

## Tech notes

- Pure HTML/CSS/JS — no frameworks, no build tools, no external requests except the two external link tabs (Branding, Menu).
- All photos/graphics are base64-encoded JPEG or PNG directly in the HTML.
- Because of the file size, editing this file requires care — see `PORTFOLIO_STATE.md` for the internal maintenance log and editing conventions if you're picking this project back up in a new session with an AI assistant.

## Credits

Design and development: **Bashar Reda**# Bashar-portfolio-
