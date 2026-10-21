# R&M Coatings — handoff at ~60%

**Live:** https://10elizabethbell.github.io/rmCoatings/ · **Repo:** https://github.com/10elizabethbell/rmCoatings · **Built:** 2026-10-21 from Muse brief of 2026-10-21 (FB group ad, New Jersey Small Business Network) · **Call Sheet:** site set

## What's built
- One page, calm band style: paper header (R&M monogram from their Facebook logo + "R&M Coatings / Performance. Defined.", tap-to-call (856) 281-5820 top right) → navy hero → "Recent job" Sicklerville write-up (paper) → "What we do" service rows (navy) → How it works (deep navy) → quote form (paper) → close with big number (navy) → footer.
- Palette: the logo is black on white, so the navies are the house navies (#1f3a5c, #13263f) and the accent is a satin brass (#e3a83c fills, #7a5200 as text on light). Text on brass is navy.
- Hero: plain textured navy band (no client photos exist anywhere). On desktop (≥1024px) the R&M monogram sits large and faint (7%) in the empty right half, never behind text.
- Motion: hero H1 letter bounce-in, `.rise` fade-up below the first screen, floating text circle (hidden on the hero and while the form is on screen). All content shows at once with reduced motion or no JS (checked).
- Contact: header number (`tel:`), hero "Text us" (`sms:` with a pre-filled body), floating circle (same text), quote form that composes a text (job chip, name, rooms, town). Under the button: "Rather talk? Call the number just below." (the close band's big number); if Messages doesn't open, a "Copy the message" fallback appears. Tapping a service row pre-selects the matching chip. The footer holds the name and Facebook only (the number was cut there so it never shows twice on one phone screen next to the close band).
- Facebook: "See more of our work on Facebook" card under the Sicklerville job, plus the footer.
- **One generated example photo** (`lvp-example.webp`) under the service rows (phone) / under the heading (desktop): an empty room with new LVP. It is an example of the service, never labelled or implied as their job.
- og.png (1200x630) for the Facebook link preview; favicon and home-screen icon from the monogram.

## Assumptions I made
- **"South Jersey" in the H1** is inferred from the 856 area code and the Sicklerville job. The brief only says the job was in Sicklerville (and that it's not their home address). Swap for their real area once known.
- **They accept texts.** The brief says "unknown". Text is offered next to the call number, never alone; the form's fallback line gives the number to call.
- **"We" voice** (they're an LLC and the ad says "We ripped out…").
- **Promise line** "We don't stop at the walls: ceilings, trim and doors get a fresh coat too." is my wording, grounded in their "nearly every surface… ceilings to walls, trim, and doors". "Your home could be next." is theirs.
- **Services** split into five rows from the one job description: luxury vinyl plank, carpet removal, walls and ceilings, trim and doors, whole-home refresh. Nothing beyond flooring and interior paint is claimed.
- **How it works** (tell us → we quote → we do the work) is assumed; cut it if the owner works differently.
- **Close heading** "Call R&M Coatings." and the form eyebrow "Takes a minute" are mine.
- **Brass accent** is my pick; the logo has no colour.

## Placeholders and gaps
- No photos of their work (the ad was text-only; Facebook profile not readable). The page has no photo section.
- No email (so none in the footer), no hours, no owner name, no service area, no reviews, no licence/insurance claims (none made on the page).
- **Generated images:**

  | File | Where | Prompt | Date | Model |
  |---|---|---|---|---|
  | `lvp-example.webp` | Services section | "Realistic interior photo, natural daylight: a freshly installed warm oak luxury vinyl plank floor in an empty living room of a modest suburban New Jersey home, clean white baseboards and freshly painted light greige walls, a white interior door, no furniture, no people, no text, shot at eye level, true-to-life colors, real estate photography" | 2026-10-21 | local z-image-turbo (mflux, seed 7) via `genimg --local` — **not** gpt-image-1: OpenAI credits were exhausted (429 `credit_balance_exhausted`) |

  Provenance is in `lvp-example.webp.json`. Swap for a real R&M job photo as soon as one exists. A second (paint/trim close-up) wasn't generated.
- Not to be confused with R&M Family Contracting (different Sicklerville business).

## Questions for the owner
- Before/after photos of the Sicklerville job (and others)? They'd replace the text-only "Just finished" section with real proof.
- Do you take texts at 856-281-5820?
- Which towns do you cover? Owner's first name(s) — who will the customer deal with?
- Anything beyond floors and interior paint (exterior paint, coatings, epoxy — the name says "Coatings")?
- Licensed/insured? Email to put in the footer?

## Ideas not built (yours to pick)
- **Before/after slider** for the Sicklerville job once photos arrive; then a photo hero under the navy overlay.
- **Runner-up worlds for an opt-in signature motion:** (1) a paint roller you drag across the hero that lays a fresh coat over a scuffed wall (best fit); (2) planks of LVP clicking into place along the hero's bottom edge as you scroll; (3) carpet peeling back to reveal plank; (4) a cut-in brush line drawing along the section edges.
- Impeccable flags kept because they're your calm-style choices: eyebrow pills (craft floor bans them), the diagonal band texture (detector `repeating-stripes-gradient`, suppressed for index.html in `.impeccable/config.json`), the bounce easing on the H1, the same `.rise` entrance on every section. Also suppressed: `flat-type-hierarchy` (it only counts the fixed 14–20px UI sizes; headings are fluid 30–80px).
- Finish reviewer ideas not taken: close heading "Your home could be next." (kept as the hero's bold line instead, to avoid repeating it); Facebook card "See our page on Facebook" (kept "more of our work" per your Facebook rule).
- After the hero, the only visible contact is the text circle (the header isn't sticky). If texting turns out not to work, make the circle a call button or drop it.

## Not verified
- Real-device touch, real SMS handoff on iOS/Android and inside Facebook's in-app browser.
- Frame rate of the bounce-in on old phones.

- Form field fill (#e6ecf5) against the white card is about 1.19:1, the same as the calm-style fix on other builds. It passes for text, but the field edges are faint. Give the fields a 1px #9aa8bb border if you want them to meet WCAG 1.4.11.
