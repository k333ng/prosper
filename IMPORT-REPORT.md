# Import report: Sacred Space for Intention & Transformation

Imported from https://prosper.love (Framer, Framer d485f69) on 2026-10-28 with `openspace import url`.
Sources: page HTML, the sitemap. 42 requests.

## Summary

- **11** pages, **0** collection items in 0 collection(s)
- **27** media files (7.3 MB) downloaded into `media/`
- **0** redirects so old addresses keep working
- **26** item(s) need your attention (below)

## Pages

| Old address | OpenSpace | Title | Sections | Blocks |
| --- | --- | --- | ---: | ---: |
| `/` | `/` | Home | 16 | 38 |
| `/thefield` | `/thefield` | THE FIELD | 6 | 9 |
| `/science` | `/science` | SCIENCE | 7 | 33 |
| `/about` | `/about` | ABOUT | 6 | 18 |
| `/form-prelaunch` | `/form-prelaunch` | JOIN THE FIELD | 2 | 4 |
| `/privacy-policy` | `/privacy-policy` | Privacy Policy | 19 | 19 |
| `/form-influencer1` | `/form-influencer1` | SERVE & GROW YOUR AUDIENCE | 2 | 5 |
| `/contact` | `/contact` | Reach Out We’re Listening | 1 | 4 |
| `/pricing` | `/pricing` | $0 | 1 | 1 |
| `/form-50` | `/form-50` | Reserve your Spot Unlock 50% Off Unlimited | 1 | 4 |
| `/terms-of-service` | `/terms-of-service` | Terms of Service | 27 | 27 |

## Design

The look was recreated with OpenSpace's own design system (Site Styles tokens, section color themes, layouts and section presets), not by copying Framer's CSS or code.

- Brand color #0099ff (the site's accent color).
- Fonts on Framer: Geograph Regular → pairing "Outfit" (Outfit / Outfit), the closest curated match. Licensed fonts can be uploaded in Site Styles → Fonts.
- Type scale on Framer: Heading 1 is 4.9× body text (very large; OpenSpace's display preset is the nearest). Density "comfortable" from the section heights.
- Geograph Regular (a licensed font) can't be copied, so Instrument Sans — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- Geograph Medium (a licensed font) can't be copied, so Proza Libre — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- Type scale on Framer (the live site, measured in a browser) kept: display 84px/44px, heading 1 84px/44px, heading 2 54px/44px, body 17px/17px, eyebrows 14px/12px caps.
- Page rhythm on Framer (the live site, measured in a browser): content 1200px wide, sections padded 184px (100px on phones) — kept in Site Styles.
- The contrast solver adjusted 7 color pairing(s) so every section theme meets WCAG AA (e.g. light accent, light accent-hover).

Design check: 0 error(s), 52 warning(s).

- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): This section is empty.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): “You are source.” is a second Heading 1 on this page. Use one Heading 1 per page.
- warning (/): “Act like it.” is a second Heading 1 on this page. Use one Heading 1 per page.
- warning (/): “Act like it.” is a second Heading 1 on this page. Use one Heading 1 per page.
- warning (/): “The early ones shape what this becomes.” is a second Heading 1 on this page. Use one Heading 1 per page.
- … and 40 more: run Design check in Studio or `design_check` with Claude.

## Needs attention

### Forms and newsletter

- Newsletter signup recreated. Subscribers are not moved: export your list from Framer (or your email service) and import it in the Hub. _(/, /thefield, /science, /about, +1 more)_
- Form "Contact form" recreated with 3 field(s). Submissions now arrive in the OpenSpace inbox; Framer form integrations (Google Drive, Mailchimp, Zapier…) need setting up again. _(/form-prelaunch, /form-50)_
- Form "Contact form" recreated with 9 field(s). Submissions now arrive in the OpenSpace inbox; Framer form integrations (Google Drive, Mailchimp, Zapier…) need setting up again. _(/form-influencer1)_
- Form "Contact form" recreated with 4 field(s). Submissions now arrive in the OpenSpace inbox; Framer form integrations (Google Drive, Mailchimp, Zapier…) need setting up again. _(/contact)_

### Blocks that need a look

- Framer "video file" block has no direct OpenSpace equivalent and was left out. _(/, /privacy-policy, /form-influencer1, /contact, +3 more)_

### Design

- Layout: "You are source.": its background #000000, as on the original. _(/)_
- Layout: "PLAY THE BEST GAME ON EARTH": its background #000000, as on the original. _(/)_
- Layout: "HOW IT FEELS": 2 cards per row, as on the original. _(/)_
- Layout: "HOW IT FEELS": its background #000000, as on the original. _(/)_
- Layout: "THE SCIENCE": its background #000000, as on the original. _(/)_
- Layout: "TESTIMONIALS": its background #000000, as on the original. _(/)_
- Layout: "The early ones shape what this becomes.": its background #000000, as on the original. _(/)_

### Other

- The page had no Heading 1; its first heading was made the Heading 1 (search engines and screen readers use it). _(/thefield, /science, /about)_

## Not moved by the importer

- Animations, effects and code components (their text and images are imported where present in the HTML).
- Form submissions, newsletter subscribers, member accounts and comments.
- Analytics and SEO history (search engines follow the redirects).

## Next steps

1. `npm install`, then `npx openspace check` (it should report no errors) and `npx openspace dev` to look around.
2. Bring it to visual parity with Claude: in this folder run `claude`, then `/openspace:migrate https://prosper.love` (or ask Claude to compare each page with the original). It screenshots both sites at desktop and mobile and adjusts presets, Site Styles and sections — never raw HTML.
3. Fix the items under **Needs attention**, then publish (push to GitHub, or `publish` with Claude).
4. Move the domain only after the new site is live and checked:
   - add the custom domain in OpenSpace (`deploy.customDomain` in `openspace.json`, or the Hub);
   - at your DNS provider (Framer Domains, your registrar or elsewhere), point the records at the new host as the domain guide says (GitHub Pages: `A`/`CNAME` records; Cloudflare: the Pages project's records);
   - keep the Framer plan until the new site serves your domain over HTTPS and the redirects work; then cancel it (and transfer the domain if you like).

