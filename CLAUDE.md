# The English Lounge — project notes

Static marketing site for The English Lounge (Rome).
Plain HTML/CSS/JS, served by GitHub Pages from the `main` branch root of
`Mj-myhub/englishloungerome` (custom domain englishloungerome.com).

This repository was started fresh in Nov 2026 with no history, so that old
personal data in the previous repository's history is not public. The old
repository (`Mj-myhub/english-lessons`, made private) keeps the full history,
including the removed IELTS practice pages. Never copy history from it into
this repository.

Owner edits files on mobile via the GitHub app, so keep files small and root-level.

## Standing instructions

- **Always commit and push changes to GitHub automatically.** After making
  any change the user asked for, commit it and push to the working branch
  without asking for confirmation. If no PR exists for the branch, open a
  draft PR. The user does not want to be asked "should I push?" each time.
- Develop on the branch specified in the task; never push to a different
  branch without explicit permission.
- All IELTS content must be **original** (no Cambridge/British Council
  copyrighted material).

## Structure

- `index.html` — bilingual (EN/IT) home page.
- IELTS practice pages were removed (Nov 2026); their source is only in the old private repository.
- `privacy.html` — bilingual privacy notice (noindex, so not in the sitemap). Update it if a new third-party service is added.
- `fonts.css` + `fonts/` — self-hosted web fonts (no Google Fonts requests). `canada-flag.svg` is local too.
- Both pages carry a Content-Security-Policy meta tag; a new external script, image host or form endpoint must be added to it.
- `sitemap.xml` — add every new page here.

## Content notes

- Teacher's public name on the site is **Jasper**.
- Prices are hidden: the `#pricing` section stays in `index.html` with `hidden` so it can be restored; all CTAs point to the free-trial booking.

## Privacy

- Never commit personal data (codice fiscale, birth date, personal phone, private emails). Business contact details on the site are fine.

## Business (all of this is already public on the site)

- The English Lounge, Rome. Tagline "Learn English in Comfort".
- Teacher's public name: Jasper. Native Canadian, 12+ years teaching, M.A. Linguistics (Siena), TTC/TEFL.
- Lessons: General, Business, IELTS/Cambridge prep; in person in Rome and online; free 20-minute trial.
- Contact on the site: theenglishlounge.rome@gmail.com, WhatsApp +39 352 080 9945 (business number, keep it).
- Bookings: Cal.com user `the.englishlounge`; every "Book Now" CTA points to `/free-trial`.
- Level test leads are emailed to the business inbox by Web3Forms (key in `index.html`, public by design).
  The result screen promises that Jasper will email the report, so the owner sends it manually.

## Design and copy rules

- Colours: emerald #15604A, deep #0B3026, sand gold #CBA15B, clay #C2683F, porcelain background #F7F8F8.
- Fonts: Fraunces (headings), Plus Jakarta Sans (body), Cormorant Garamond (accents), all self-hosted.
- Pill-shaped buttons; logo uses border-radius 8px.
- Site copy: no em dashes; testimonials without quotation marks, apostrophes or real surnames;
  no TOEFL (only IELTS/Cambridge); no "materials included" or "score improvement guarantee";
  avoid stock photos (three Unsplash service photos remain until the owner sends real ones).
- Every visible text needs both `data-en` and `data-it` versions.

## Working with the owner

- Works only on iPhone: give step-by-step mobile instructions, never terminal commands.
- Wants the highest quality and everything double-checked before pushing.
- Changes go live only after the PR is merged into `main` (GitHub Pages builds in about 2 minutes).

## Open items

- Restrict the Web3Forms key to englishloungerome.com (owner, in the Web3Forms dashboard).
- `text.txt` contains robots.txt directives; it should be renamed to `robots.txt`.
- Replace the three Unsplash service photos with the owner's own photos.
