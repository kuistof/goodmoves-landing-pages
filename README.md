# Good Moves Studio · Landing Pages

Single-file landing pages for Good Moves Studio, a low-impact pilates and movement studio in Prenzlauer Berg, Berlin. Each page is fully self-contained: one HTML file with inline CSS and JavaScript, no build step and no dependencies (web fonts load from Google Fonts).

## Pages

- `index.html` : main funnel. Generic studio intro, a short "Find your routine" questionnaire, and one recommended curated 6-week plan. Live at https://goodmoves-landing.vercel.app
- `summer.html` : Summer Deal. 99 EUR flat, unlimited classes until 15 September. Leads with the flexibility angle (no membership to pause, come when you can). Uses the official GMS brand system: display font Nersans Three with Nunito as the sanctioned fallback (the Nersans file is not in this repo), system font body, terracotta #B0482D, beige #EEDBC3, cream #FBF6F1, blue #001DA2, ink #000044, organic blob shapes. Interim photos live in `assets/`. Live at https://goodmoves-summer.vercel.app

## Notes

- Bilingual EN/DE. English is the in-markup default, German lives in `data-de` attributes. A small inline script detects the browser language on first visit, remembers the choice in localStorage, and toggles with no reload.
- `index.html` still uses the earlier brand pass: fonts Bricolage Grotesque, Figtree, Fredoka. Palette cream #F7F0E9, ink/navy #020F52, cobalt #0426CE, coral #BE3F21, peach.
- The checkout is currently mock: `index.html` shows a placeholder alert, `summer.html` opens a branded checkout modal with a start-day picker that does not submit anywhere yet. The real checkout connects to Mindbody.

Open the `.html` files straight in a browser, or clone and tinker.
