# Outstanding verification

Point-in-time notes from the October 2026 update. Re-check before adding anything below to the site.

- AussieBattlers: confirm the public play URL and current public title; aussiebattlers.com previously redirected to a parking page, and the Render URL timed out.
- Joshi's Nightmare: the Vercel link was HTTP 200 in review; re-test actual gameplay.
- Trackn, Jellyfish: no public URL, so no demo links are shown.
- Real screenshots: none exist in this repo for the four featured projects; the cards use plain typographic panels. Add approved screenshots when available.
- Thailand Your Way, Mareni Studio, TiTumbler, Crappy Turd, Midnight Pisser, rhythm game, The Birthing: confirm status and permission to show any art or audio before adding links.
- Early work: Read It & Wipe and Rad Kelly's Heroku demos were unavailable; Naruto Run (Netlify) not re-verified.
- Résumé: `photo/RESUME.pdf` is outdated and not linked. Publish a current one before re-adding a link.

## Accessibility checks (local, headless Chromium)

Done: text contrast on every text element in light and dark mode (min 6.0:1 light, 8.07:1 dark; AA needs 4.5:1); white labels on the project cover panels (min 5.0:1); keyboard tab order (skip link first, 24 stops, visible focus ring on every one, skip link lands on `#work`); tap targets at least 44px high; no horizontal overflow at 320, 390, 768 and 1440px; smooth scrolling disabled under reduced motion.

Not done: screen-reader testing (VoiceOver/NVDA), testing on real phones, the 320–1440px visual pass beyond the desktop and 390px screenshots, a Lighthouse/axe run, and any check of the deployed `/david_portfolio/` site, which this environment could not reach. Colours are checked by computed value only, not against images (there are none in the featured section).
