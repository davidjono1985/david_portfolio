# Outstanding verification

Notes from the October 2026 update. Re-check before adding anything below to the site.

## Cover images
Covers are captures of each project's real landing page, rendered in headless Chromium at 390×844 (2×), taken after the page finished loading, with no browser chrome, and cropped to a common 4:3 frame (`photo/projects/`, 390w and 780w WebP). Pages were run locally from each project's source; no project repository or database was modified.

| Project | Cover | Notes |
| --- | --- | --- |
| Joshi's Nightmare | Title-screen capture | Cropped above the character portrait. The full page shows a recognisable person; confirm permission before showing it. |
| Trackn | Home-page capture | Local build without a backend. Cropped below the "accounts not available on this deployment" notice; recapture from a deployed URL. |
| Jellyfish | Demo-page capture | The real page, labelled "Infrastructure demo". |
| Crappy Turd | Title-screen capture | Local build. |
| AussieBattlers | Title panel | Need the repository or the live URL. |
| Mareni Studio | None | Need the site URL or repository. |
| Thailand Your Way | None | Needs a Supabase project to render; locally it shows "This site isn't connected yet". Need a deployed URL. |
| TiTumbler | None | Landing page is dominated by a real person's likeness; confirm permission. |
| Not My Tempo, The Midnight Pisser | None | Characters use real people's likenesses; confirm permission. |

## Links
- Joshi's Nightmare: the Vercel link was HTTP 200 in an earlier review. Re-test actual gameplay.
- AussieBattlers: confirm the public play URL and title (aussiebattlers.com previously redirected to a parking page; the Render URL timed out).
- Trackn, Jellyfish: no public site is linked.
- Early work: Read It & Wipe and Rad Kelly's Heroku demos were unavailable; Naruto Run (Netlify) not re-verified.
- Live deployment could not be reached from the build environment.

## Content to confirm with the owners
- Jellyfish: Emma's role and surname/credit wording; whether the public demo site and exploratory prototype should be linked.
- Statuses for Thailand Your Way, Crappy Turd, TiTumbler, Not My Tempo and Mareni Studio come from READMEs and earlier notes.

## Résumé
`photo/RESUME.pdf` is outdated, lists a home address and phone number, and is not linked. The site shows a non-clickable "Résumé — coming soon" placeholder. Replace the file and link it when a current résumé is ready.

## Original portfolio archive
`archive/original/` holds the pre-redesign site (index, project pages, stylesheet and the images it uses) as published at `6413c39`, with relative paths fixed, the dead résumé link and stylesheet integrity hash removed, a "current portfolio" banner and `noindex`. The devicon stylesheet URL was changed from the defunct RawGit CDN to jsDelivr (unverified). The original contact form still points at mailthis.to.

## Accessibility checks (local, headless Chromium)
Done at 320, 390, 768 and 1440px: no horizontal overflow; text contrast on every text element in light and dark mode (min 6.0:1 light, 8.07:1 dark); skip link first in tab order and landing on `#work` with focus continuing inside it; 25 tab stops with a visible focus ring, none hidden under the sticky header; all in-page links (nav, case-study, glimpse tiles) land with their heading below the header; tap targets at least 44px; no broken images; smooth scrolling disabled under reduced motion.

Not done: screen-reader testing, real-device testing, an axe or Lighthouse run, and checks of the deployed site.
