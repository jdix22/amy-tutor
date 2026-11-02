# Amy Jubas-Bernstein: JK–Grade 3 tutoring site

Prospect site for Amy Jubas-Bernstein (B.Ed., OCT, Special Education Specialist, Sounds-Write trained).
Built from her flyer, November 2026. Single static page, no build step.

Live preview: https://jdix22.github.io/amy-tutor/

## The business name (not chosen yet)

The working name is **Sound Start Tutoring**. To show Amy other names live, add `?name=` to the link:

- https://jdix22.github.io/amy-tutor/?name=Bright%20Steps%20Learning
- https://jdix22.github.io/amy-tutor/?name=First%20Sounds%20Tutoring
- https://jdix22.github.io/amy-tutor/?name=Amy%20JB%20Tutoring

Once she picks one, find-and-replace `Sound Start Tutoring` across `index.html`, `404.html` and
`_src/og.html`, then re-render the social image (`assets/og.png`).

## Before launch: things to confirm with Amy

Everything on the page comes from her flyer. These were not on it, so the site avoids them:

- Rates, session length, hours and availability (the site says "contact Amy for rates").
- Where sessions happen: her home, the family's home, or both.
- Whether she offers online sessions, an assessment, or a first free chat.
- Whether texting 416-725-7499 is fine (site currently says "Call").
- A photo of Amy for the "Meet your tutor" panel (currently an AJB monogram).
- Parent testimonials she has permission to use (none are on the site; never invent them).
- "Getting started" steps (reach out → talk it through → begin sessions) are a sensible default; check they match how she works.

## Go-live checklist

1. Remove `<meta name="robots" content="noindex">` from `index.html` (it's a prospect preview until she approves).
2. Point canonical, `og:url`, `og:image`, JSON-LD URLs, `robots.txt` and `sitemap.xml` at her real domain.
3. Optional: set `FORM_ENDPOINT` in the page script (e.g. Formspree) so the form sends without opening an email app.
4. Owner to-dos: claim a Google Business Profile (service-area business: Thornhill, Richmond Hill, Maple, no public address),
   use the same name, phone and email everywhere, and ask happy families for Google reviews.

## Files

- `index.html`: the whole site (styles and script inline). Facts sheet is the comment at the top of the `<style>` block.
- `assets/img/`: Unsplash photos (free Unsplash licence), WebP.
  - child-reading-with-finger: https://unsplash.com/photos/child-reading-book-at-wooden-table-BPXSTl_HBhk
  - decodable-reader-practice: https://unsplash.com/photos/two-people-learning-together-at-a-wooden-table-JZXGFdD6UDk
  - tracing-numbers-math: https://unsplash.com/photos/a-child-is-writing-on-a-sheet-of-paper-AfXDm5I-yDo
- `assets/og.png`, `apple-touch-icon.png`: rendered from `_src/` with the visibility-pillars og-image script.
- Sounds-Write is a trademark of its owner, named only to describe Amy's training.

Website designed by jdix.ca.
