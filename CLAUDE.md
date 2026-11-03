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
