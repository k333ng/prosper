# Visual fidelity

Overall match: **54/100** — fonts, type sizes, spacing and each section measured in a browser on both sites (75%), and how alike the pages look as pictures (25%). How it's scored: docs/qa/import-fidelity.md.

Scored two ways, side by side: **54/100 corrected**, 54/100 by the strict v3 scorer. The corrected score reads three things the strict one gets wrong (navigation in a header themed "brand", off-screen slides counted as columns, a picture-only band on a phone); the pages below list where it did.

Auto-tuning raised it from 39/100:

- section padding on phones 140px
- heading on dark sections #cec4fb, as on the original (4 of 7 sections)
- text on light sections #ffffff, as on the original (4 of 4 sections)
- heading on light sections #ffffff, as on the original (7 of 9 sections)
- background on light sections #000000, as on the original (9 of 9 sections)
- /about: "OurFounders": 2 cards per row, as on the original
- /about: "OurFounders": 2 cards per row, as on the original
- /about: "Our Founders": its background #000000, as on the original
- /about: "Our Founders": 2 cards per row, as on the original
- /: "You're ready. We're ready. Let's begin." set at the h2 size, as on the original
- /about: "Ready to step into the field?" set at the h2 size, as on the original
- /: section 4 image crop 1:1
- /: section 8 image crop 1:1
- /: section 5 "pro • sper" recreated as a custom component
- /: section 8 "THE SCIENCE" recreated as a custom component
- /: section 12 "PARTNERS" recreated as a custom component
- /about: section 1 "Built by practitioners, for practitioner" recreated as a custom component
- /form-influencer1: section 1 "Bring your people into practice" recreated as a custom component

Without custom components: 52/100; with the sections recreated as components: 54/100.

## / at 1440px — 62/100

Checks 63/100 · looks alike 61/100 (screenshots compared).

Original: https://prosper.love/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Heading 1 size | 84px | 84px | same |
| Heading 2 size | 54px | 54px | same |
| Heading 3 size | 17px | 24px | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Eyebrows: present | Geograph Medium 14px | not found | **differs** |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 12px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Navigation size | 12px | 12px | same |
| Navigation letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Content width | 1200px | 1200px | same |
| Section padding | 184px | 184px | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | You are source. | 84 | Heading: Geograph Regular 84px → Instrument Sans 84px; Text: Geograph Regular 17px → Instrument Sans 17px; Height: 844px → 1321px |
| 2 | PLAY THE BEST GAME ON EARTH | 77 | Heading: Geograph Medium 17px → Instrument Sans 24px; Text: Geograph Regular 17px → Instrument Sans 17px |
| 3 | (no heading) | 0 | Present:  → no matching section |
| 4 | HOW IT FEELS | 64 | Heading: Geograph Medium 14px → Instrument Sans 24px; Text: Geograph Regular 17px → Instrument Sans 17px; Image placement: left, 35% wide → center, 83% wide; Height: 898px → 2391px |
| 5 | pro • sper | 96 | Heading: Geograph Regular 31px → Instrument Sans 31px |
| 6 | Ready to step into the field? | 43 | Heading: Geograph Regular 47px → Instrument Sans 24px; Columns: 1 → 3 |
| 7 | (no heading) | 57 | Image placement: center, 47% wide → center, 100% wide; Image crop: 0.79:1 → 3.91:1; Height: 1011px → 368px |
| 8 | THE SCIENCE | 72 | Heading: Geograph Medium 14px → Proza Libre 14px; Text: Geograph Regular 17px → Instrument Sans 17px; Image crop: 0.92:1 → 1.52:1 |
| 9 | TESTIMONIALS | 43 | Heading: Geograph Medium 14px → Instrument Sans 54px; Text: Geograph Regular 16px → Instrument Sans 17px; Text color: #988dcc → #cec4fb; Columns: 2 → 1; Height: 619px → 1093px |
| 10 | The early ones shape what this becomes. | 56 | Heading: Geograph Regular 61px → Instrument Sans 84px; Text: Geograph Regular 17px → Instrument Sans 17px; Eyebrow and rule: BE AMONG THE FIRST → none; Image placement: center, 85% wide → none; Height: 671px → 1332px |
| 11 | You're ready. We're ready. Let's begin. | 67 | Heading: Geograph Regular 54px → Instrument Sans 54px; Columns: 1 → 3 |
| 12 | PARTNERS | 25 | Heading: Geograph Medium 17px → Proza Libre 17px; Columns: 1 → 3; Image placement: right, 24% wide → none; Height: 463px → 660px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h3.size = 17
- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.shape = "round"
- Bring this section across (or check it was merged into another).
- Adjust the stack column spans (image column) or the image's side.
- Fewer columns: merge them into one stack column.
- Use the original's image proportions (the block's aspect ratio).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Add the eyebrow to the heading block.

## / at 390px — 62/100 (strict v3: 59/100)

Corrected scoring on this page:

- Section 3 (a picture alone on a phone) is the picture of section 6, which holds it with its words.
- Section 12: columns counted on screen only (6 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).

Checks 64/100 · looks alike 57/100 (screenshots compared).

Original: https://prosper.love/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Heading 1 size | 44px | 40.9px | same |
| Heading 2 size | 44px | 44.3px | same |
| Heading 3 size | 57px | 20px | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Eyebrows: present | sans-serif 12px | not found | **differs** |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 14px | **differs** |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 99.5px | 141px | **differs** |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Act like it. | 67 | Heading: Geograph Regular 57px → Instrument Sans 40.9px; Text: Geograph Regular 17px → Instrument Sans 17px; Height: 740px → 1043px |
| 2 | PLAY THE BEST GAME ON EARTH | 77 | Heading: Geograph Medium 17px → Instrument Sans 20px; Text: Geograph Regular 17px → Instrument Sans 17px |
| 3 | (no heading) | 80 | Image crop: 0.75:1 → 1.63:1 |
| 4 | HOW IT FEELS | 72 | Heading: Geograph Medium 17px → Instrument Sans 20px; Text: Geograph Regular 17px → Instrument Sans 17px; Height: 1292px → 2095px |
| 5 | pro • sper | 57 | Heading: Geograph Regular 22px → Instrument Sans 25px; Height: 300px → 433px |
| 6 | Ready to step into the field? | 50 | Heading: Geograph Regular 44px → Instrument Sans 20px; Text: Geograph Regular 13px → Instrument Sans 20px; Height: 524px → 787px |
| 7 | (no heading) | 71 | Image crop: 0.46:1 → 1.08:1; Height: 760px → 360px |
| 8 | THE SCIENCE | 58 | Heading: Geograph Medium 17px → Proza Libre 14px; Text: Geograph Regular 17px → Instrument Sans 14px; Image crop: 0.97:1 → 1.52:1 |
| 9 | TESTIMONIALS | 61 | Heading: Geograph Medium 14px → Instrument Sans 44.3px; Text: Geograph Regular 16px → Instrument Sans 17px; Text color: #988dcc → #f0f4ed; Height: 972px → 4011px |
| 10 | The early ones shape what this becomes. | 64 | Heading: Geograph Regular 44px → Instrument Sans 40.9px; Text: Geograph Regular 17px → Instrument Sans 17px; Eyebrow and rule: BE AMONG THE FIRST → none; Image placement: center, 126% wide → none; Height: 914px → 1267px |
| 11 | You're ready. We're ready. Let's begin. | 77 | Heading: Geograph Regular 47px → Instrument Sans 44.3px; Text: Geograph Regular 13px → Instrument Sans 20px |
| 12 | PARTNERS | 44 | Heading: Geograph Medium 17px → Proza Libre 14px; Image placement: right, 88% wide → center, 87% wide; Image crop: 2.76:1 → 1:1; Height: 475px → 4027px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h3.sizeMobile = 57
- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.sizeMobile = 12
- choices.layout.sectionPaddingMobile = 100
- choices.shape = "round"
- Use the original's image proportions (the block's aspect ratio).
- Add the eyebrow to the heading block.
- Adjust the stack column spans (image column) or the image's side.

## /about at 1440px — 64/100

Checks 67/100 · looks alike 54/100 (screenshots compared).

Original: https://prosper.love/about  
Imported: /about (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Heading 1 size | 16px | 84px | **differs** |
| Heading 2 size | 53px | 54px | same |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 12px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Navigation size | 12px | 12px | same |
| Navigation letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Section padding | 154px | 184px | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Built by practitioners, for practitioners. | 94 | Heading: Geograph Regular 16px → Instrument Sans 16px; Text: Geograph Regular 17px → Instrument Sans 17px |
| 2 | Our Founders | 25 | Heading: Geograph Regular 61px → Instrument Sans 84px; Columns: 2 → 1; Image placement: left, 35% wide → none; Height: 2692px → 452px |
| 3 | (no heading) | 63 | Text: Geograph Regular 32px → Instrument Sans 17px; Text color: #cec4fb → #f0f4ed |
| 4 | Ready to step into the field? | 67 | Heading: Geograph Regular 53px → Instrument Sans 54px; Columns: 1 → 2 |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h1.size = 16
- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.shape = "round"
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.
- Fewer columns: merge them into one stack column.

## /about at 390px — 61/100

Checks 63/100 · looks alike 55/100 (screenshots compared).

Original: https://prosper.love/about  
Imported: /about (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Heading 1 size | 16px | 40.9px | **differs** |
| Heading 2 size | 41px | 44.3px | same |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 14px | **differs** |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 118.5px | 141px | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Built by practitioners, for practitioners. | 50 | Heading: Geograph Regular 16px → Instrument Sans 14px; Text: Geograph Regular 17px → Instrument Sans 14px; Height: 964px → 671px |
| 2 | Our Founders | 50 | Heading: Geograph Regular 48px → Instrument Sans 40.9px; Image placement: center, 79% wide → none; Height: 4135px → 323px |
| 3 | (no heading) | 63 | Text: Geograph Regular 28px → Instrument Sans 17px; Text color: #cec4fb → #f0f4ed |
| 4 | Ready to step into the field? | 96 | Heading: Geograph Regular 41px → Instrument Sans 44.3px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h1.sizeMobile = 16
- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.sizeMobile = 12
- choices.shape = "round"
- Adjust the stack column spans (image column) or the image's side.

## /contact at 1440px — 53/100

Checks 54/100 · looks alike 52/100 (screenshots compared).

Original: https://prosper.love/contact  
Imported: /contact (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Geograph Regular 68px | not found | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Eyebrows: present | Geograph Regular 15px | not found | **differs** |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 12px | same |
| Buttons letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Navigation size | 12px | 12px | same |
| Navigation letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Section padding | 190px | 229px | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Reach Out We’re Listening | 39 | Heading: Geograph Regular 68px → Instrument Sans 24px; Text: Geograph Regular 17px → Instrument Sans 17px; Columns: 5 → 3; Eyebrow and rule: CONNECT WITH US → none; Image placement: center, 100% wide → none; Height: 1829px → 1181px |

What would close the gap:

- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.shape = "round"
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Add the eyebrow to the heading block.
- Adjust the stack column spans (image column) or the image's side.

## /contact at 390px — 49/100

Checks 46/100 · looks alike 56/100 (screenshots compared).

Original: https://prosper.love/contact  
Imported: /contact (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Geograph Regular 48px | not found | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Eyebrows: present | Geograph Regular 15px | not found | **differs** |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 14px | **differs** |
| Buttons letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Section padding | 190px | 181px | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Reach Out We're Listening | 39 | Heading: Geograph Regular 48px → Instrument Sans 20px; Text: Geograph Regular 17px → Instrument Sans 17px; Columns: 3 → 1; Eyebrow and rule: CONNECT WITH US → none; Image placement: center, 100% wide → none; Height: 2609px → 1225px |

What would close the gap:

- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.sizeMobile = 12
- choices.shape = "round"
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Add the eyebrow to the heading block.
- Adjust the stack column spans (image column) or the image's side.

## /form-50 at 1440px — 52/100

Checks 54/100 · looks alike 49/100 (screenshots compared).

Original: https://prosper.love/form-50  
Imported: /form-50 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Geograph Regular 68px | not found | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Eyebrows: present | Geograph Regular 15px | not found | **differs** |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 12px | same |
| Buttons letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Navigation size | 12px | 12px | same |
| Navigation letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Section padding | 190px | 229px | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Reserve your Spot Unlock 50% Off Unlimited | 39 | Heading: Geograph Regular 68px → Instrument Sans 24px; Text: Geograph Regular 17px → Instrument Sans 17px; Columns: 5 → 3; Eyebrow and rule: EARLY ACCESS SIGN-UP → none; Image placement: center, 100% wide → none; Height: 1646px → 885px |

What would close the gap:

- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.shape = "round"
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Add the eyebrow to the heading block.
- Adjust the stack column spans (image column) or the image's side.

## /form-50 at 390px — 49/100

Checks 46/100 · looks alike 56/100 (screenshots compared).

Original: https://prosper.love/form-50  
Imported: /form-50 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Geograph Regular 48px | not found | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Eyebrows: present | Geograph Regular 15px | not found | **differs** |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 14px | **differs** |
| Buttons letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Section padding | 190px | 181px | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Reserve your Spot. Unlock 50% Off Unlimited | 39 | Heading: Geograph Regular 48px → Instrument Sans 20px; Text: Geograph Regular 17px → Instrument Sans 17px; Columns: 3 → 1; Eyebrow and rule: EARLY ACCESS SIGN-UP → none; Image placement: center, 100% wide → none; Height: 2453px → 973px |

What would close the gap:

- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.sizeMobile = 12
- choices.shape = "round"
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Add the eyebrow to the heading block.
- Adjust the stack column spans (image column) or the image's side.

## /form-influencer1 at 1440px — 71/100

Checks 77/100 · looks alike 56/100 (screenshots compared).

Original: https://prosper.love/form-influencer1  
Imported: /form-influencer1 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Geograph Regular 61px | not found | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Label font | Geograph Medium | Proza Libre (close stand-in) | close (85%) |
| Eyebrows size | 14px | 14px | same |
| Eyebrows letter spacing and case | 0.39em, uppercase | 0.39em, uppercase | same |
| Buttons size | 12px | 12px | same |
| Buttons letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Navigation size | 12px | 12px | same |
| Navigation letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Section padding | 158px | 184px | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Bring your people into practice | 95 | Heading: Geograph Regular 61px → Instrument Sans 61px; Text: Geograph Regular 17px → Instrument Sans 17px |
| 2 | (no heading) | 0 | Present:  → no matching section |

What would close the gap:

- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "Geograph Medium" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.shape = "round"
- Bring this section across (or check it was merged into another).

## /form-influencer1 at 915px — 42/100

Checks 33/100 · looks alike 69/100 (screenshots compared).

Original: https://prosper.love/form-influencer1  
Imported: /form-influencer1 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Geograph Regular 50px | not found | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 14px | **differs** |
| Label font | Geograph Medium | Proza Libre (close stand-in) | close (85%) |
| Eyebrows size | 12px | 14px | **differs** |
| Eyebrows letter spacing and case | 0.208em, none | 0.39em, uppercase | **differs** |
| Buttons size | 12px | 14px | **differs** |
| Buttons letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Navigation: present | sans-serif 12px | not found | **differs** |
| Section padding | 190px | 141.5px | **differs** |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | SERVE & GROW YOUR AUDIENCE | 25 | Heading: Geograph Regular 30px → Instrument Sans 20px; Text: Geograph Regular 17px → Instrument Sans 20px; Columns: 3 → 1; Eyebrow and rule: S → none; Image placement: left, 100% wide → none; Height: 4354px → 1876px |

What would close the gap:

- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.body.size = 17
- Site Styles → choices.typography.label = { family: "Geograph Medium" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.eyebrow.size = 12
- choices.typography.scale.eyebrow = { letterSpacing: 0.208, case: "none" }
- choices.typography.scale.button.size = 12
- choices.layout.sectionPadding = 190
- choices.shape = "round"
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Add the eyebrow to the heading block.
- Adjust the stack column spans (image column) or the image's side.

## /form-prelaunch at 1440px — 40/100

Checks 37/100 · looks alike 51/100 (screenshots compared).

Original: https://prosper.love/form-prelaunch  
Imported: /form-prelaunch (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Geograph Regular 68px | not found | **differs** |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 12px | same |
| Buttons letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Navigation size | 12px | 12px | same |
| Navigation letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present:  → no matching section |

What would close the gap:

- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.shape = "round"
- Bring this section across (or check it was merged into another).

## /form-prelaunch at 390px — 45/100

Checks 42/100 · looks alike 54/100 (screenshots compared).

Original: https://prosper.love/form-prelaunch  
Imported: /form-prelaunch (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Geograph Regular 48px | not found | **differs** |
| Body font | Geograph Regular | Instrument Sans (close stand-in) | close (85%) |
| Body text size | 17px | 17px | same |
| Eyebrows: present | Geograph Regular 15px | not found | **differs** |
| Label font | sans-serif | Instrument Sans (close stand-in) | close (25%) |
| Buttons size | 12px | 14px | **differs** |
| Buttons letter spacing and case | 0em, uppercase | 0em, uppercase | same |
| Section padding | 190px | 141px | **differs** |
| Button corners | 100px | 8px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Join the Field | 39 | Heading: Geograph Regular 48px → Instrument Sans 20px; Text: Geograph Regular 17px → Instrument Sans 17px; Columns: 3 → 1; Eyebrow and rule: EARLY ACCESS SIGN-UP → none; Image placement: center, 100% wide → none; Height: 2297px → 561px |

What would close the gap:

- Site Styles → choices.typography.body = { family: "Geograph Regular" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "sans-serif" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.sizeMobile = 12
- choices.layout.sectionPaddingMobile = 190
- choices.shape = "round"
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Add the eyebrow to the heading block.
- Adjust the stack column spans (image column) or the image's side.

