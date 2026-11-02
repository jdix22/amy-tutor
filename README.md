# Beyond the Classroom Tutoring

JK–Grade 3 tutoring site for Amy (B.Ed., OCT, Special Education Specialist, Sounds-Write trained).
Built from her flyer, November 2026, with her edits of 2 Nov 2026. Single static page, no build step.

Live preview: https://jdix22.github.io/amy-tutor/

## Amy's wording rules

- First name only. Her surname is not to appear anywhere on the site.
- Experience is shown as "10+ years in special education". She has taught for longer but prefers not to give the total.
- She has taught in the TDSB, YRDSB and private schools.

## Before launch: things to confirm with Amy

Everything on the page comes from her flyer and her edits. These were not given, so the site avoids them:

- Rates, session length, hours and availability (the site says "contact Amy for rates").
- Where sessions happen: her home, the family's home, or both.
- Whether she offers online sessions, an assessment, or a first free chat.
- A photo of Amy for the "Meet Amy" panel (currently her first name set as a monogram).
- Parent testimonials she has permission to use (none are on the site; never invent them).
- "Getting started" steps (reach out, talk it through, begin sessions) are a sensible default; check they match how she works.
- Her email (amyjb@rogers.com) contains her initials; a business email on her own domain would avoid that.

## Go-live checklist

1. Remove `<meta name="robots" content="noindex">` from `index.html` (it's a prospect preview until she approves).
2. Point canonical, `og:url`, `og:image`, JSON-LD URLs, `robots.txt` and `sitemap.xml` at her real domain.
3. Optional: set `FORM_ENDPOINT` in the page script (e.g. Formspree) so the form sends without opening an email app.
4. Owner to-dos: claim a Google Business Profile (service-area business: Thornhill, Richmond Hill, Maple, no public address),
   use the same name, phone and email everywhere, and ask happy families for Google reviews.

The `?name=` link trick still works for trying other names: https://jdix22.github.io/amy-tutor/?name=Another%20Name

## Files

- `index.html`: the whole site (styles and script inline). Facts sheet is the comment at the top of the `<style>` block.
- `assets/img/`: Unsplash photos (free Unsplash licence), WebP.
  - child-reading-with-finger: https://unsplash.com/photos/child-reading-book-at-wooden-table-BPXSTl_HBhk
  - decodable-reader-practice: https://unsplash.com/photos/two-people-learning-together-at-a-wooden-table-JZXGFdD6UDk
  - tracing-numbers-math: https://unsplash.com/photos/a-child-is-writing-on-a-sheet-of-paper-AfXDm5I-yDo
- `assets/og.png`, `apple-touch-icon.png`: rendered from `_src/` with the visibility-pillars og-image script.
- Sounds-Write is a trademark of its owner, named only to describe Amy's training.

Website designed by jdix.ca.
