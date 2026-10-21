---
name: R&M Coatings
description: Calm paper-and-navy bands with one satin-brass accent for a South Jersey flooring-and-paint crew.
colors:
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#13263f"
  body: "#2a3a4c"
  soft: "#4a5868"
  navy: "#1f3a5c"
  deep: "#13263f"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c8d4e4"
  brass: "#e3a83c"
  brass-2: "#ecbc62"
  brass-ink: "#7a5200"
  line: "rgba(19,38,63,.12)"
  focus: "#1f5fa8"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, 11.4vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(21px, 5.6vw, 24px)"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(18px, 4.8vw, 20px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  button:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.2
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-desktop: "40px"
  section: "64px"
  section-desktop: "96px"
  field-gap: "20px"
components:
  button-primary:
    backgroundColor: "{colors.brass}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.brass-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-text:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  service-row:
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    height: "76px"
  step-number:
    backgroundColor: "{colors.brass}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-text-circle:
    backgroundColor: "{colors.brass}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: R&M Coatings

## Overview

**Creative North Star: "The Fresh Coat"**

R&M Coatings sells the feeling of a room the day the crew leaves: clean floor, new paint, nothing in the way. The system is Ellie's calm band house style (`~/.claude/skills/pitch-site/references/calm-photo-style.md`) applied to this client: an off-white paper ground, two navies taken toward the brand's dark monogram, and one satin-brass accent used as a fill. Full-bleed bands alternate light and dark so each section announces itself without rules, cards or ornament.

Density is low and phone-first. Each band carries one heading, at most a lede, and one list or control. Shapes are soft and borderless: pill buttons, 24px cards, tinted fields. Motion is limited to two moves, a letter-by-letter bounce on the hero H1 and a 12px fade-up for content below the first screen, both absent without JS and under reduced motion.

The client has published no photos of their work. The hero is therefore the plain textured navy band (with the R&M monogram faint on desktop), and the single photograph on the page, `lvp-example.webp`, is a generated illustration of an LVP floor, not an R&M job (provenance in `lvp-example.webp.json`). It must never be captioned, cropped or reused as client work.

**Key Characteristics:**
- Paper, navy, deep navy with diagonal-line texture; bands alternate light/dark.
- One warm accent, brass, as a fill; a darker brass-ink when it must be text on light.
- Cal Sans display at weight 400 for every heading, button and big label; system stack for running text at 16/1.7.
- Soft borderless shapes: 999px pills, 24px cards, 10px tinted fields.
- Every link row changes only its arrow on hover.
- Text/call are the only conversions; the phone number sits top right and in the close band.

## Colors

A cool, quiet paper-and-navy palette with a single warm brass voice.

### Primary
- **Satin Brass** (`brass`): the only accent. Fills only: primary buttons, step numbers, the floating text circle, the hovered arrow circle, the eyebrow dot, text selection. Text on it is always Ink (7.2:1). On navy and deep bands it may also be text, for the accent phrase of a heading and the phone glyph (5.5:1 on navy).
- **Lit Brass** (`brass-2`): primary button hover fill only.
- **Brass Ink** (`brass-ink`): brass as text or icon on light grounds (6.4:1 on paper): the light-band accent phrase, the claims checkmarks, the header phone glyph and its hover.

### Secondary
- **Harbour Navy** (`navy`): hero, services and close bands.
- **Night Navy** (`deep`): the how-it-works band and footer, always with the diagonal-line texture.

### Neutral
- **Paper** (`paper`): page ground, header, light bands, theme-color.
- **Card White** (`card`): the quote form card and the Facebook card.
- **Field Mist** (`field`): input and unselected chip fill on the white form card.
- **Ink** (`ink`): headings on light, text on brass, the selected chip fill. Same value as Night Navy, kept as a separate role.
- **Body Slate** (`body`): running text on light (10.7:1 on paper).
- **Soft Slate** (`soft`): ledes, helper text, the brand tagline (6.7:1 on paper).
- **On-dark** / **On-dark Soft** (`on-dark`, `on-dark-soft`): headings and running text on navy bands (soft is 7.7:1 on navy, 10.2:1 on deep).
- **Hairline** (`line`): dividers between claims on paper. On navy the equivalent is white at 14%.
- **Focus Blue** (`focus`): hover and focus outlines on light grounds, deliberately distinct from brass.
- **Error Red** (`error`): inline error text and the error field border.

### Named Rules
**The Brass Is Paint, Not Ink Rule.** Brass is a fill on light grounds. Text on brass is Ink; brass as text on paper is always Brass Ink. White on brass and brass on paper are never used.

**The Ground Is Never Black Rule.** The darkest surface is Night Navy; the page ground is Paper.

## Typography

**Display Font:** Cal Sans (Google Fonts, `display=swap`, preconnected), falling back to Avenir Next, Segoe UI, system-ui
**Body Font:** system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** One friendly geometric display face at a single weight carries every heading, button, row and number; the system body stays out of its way.

### Hierarchy
- **Display** (400, `clamp(40px, 11.4vw, 80px)`, 1.02, max 12ch): the hero H1 only, white on navy, last phrase in brass.
- **Headline** (400, `clamp(30px, 7.6vw, 48px)`, 1.08): one H2 per band; on navy/deep bands the last phrase ("do.", "works.", "R&M Coatings.") takes the accent.
- **Title** (400, `clamp(21px, 5.6vw, 24px)`, 1.2): service rows and step titles. Claims use the same face at `clamp(20px, 5.4vw, 24px)`/1.15.
- **Lede** (system, `clamp(18px, 4.8vw, 20px)`, max 38ch): one sentence under a section heading; the hero promise uses the same size at 1.5, max 30ch (34ch desktop).
- **Body** (system 400, 16px, 1.7): everything else, including inputs (16px so iOS doesn't zoom), errors and footer.
- **Button / Label** (Cal Sans 400, 18px / 16px): buttons, the header phone, form labels and legends.

### Named Rules
**The One Weight Rule.** Cal Sans is only ever weight 400; hierarchy comes from size and colour. Bold appears only inside body copy (the promise's last line, the post-send note).

**The Bounce Is the Hero's Rule.** Only the hero H1 animates letter by letter. No other heading gets a letter effect.

## Layout

Single column on phones inside a `--gutter` of 20px (40px from 760px), max container 1160px. Bands are full-bleed with 64px vertical padding (96px from 760px). Breakpoints: 760px (desktop rhythm, hero buttons side by side at min 220px), 1024px (two-column splits with a 64px column gap); small-phone steps at 429, 379 and 339px progressively drop the tagline, the header phone glyph and the monogram so the header never wraps.

At 1024px: the job band puts the heading left and claims right with the Facebook card under the heading; the services band puts the heading and example photo left (1fr) and rows right (1.3fr); the quote band pins its heading sticky beside the form (1fr / 1.2fr); steps go to three columns; the close band puts the giant phone number bottom-right.

Band order: paper header, navy hero, paper job, navy services, deep how-it-works, paper quote, navy close, deep footer.

## Elevation & Depth

Flat by default; depth comes from tonal bands and the faint diagonal texture on navy surfaces (`repeating-linear-gradient` at 3.5% white, on the hero, the deep band and the footer). Exactly two shadows exist, both soft and navy-tinted, never hard or offset.

### Shadow Vocabulary
- **Card lift** (`box-shadow: 0 8px 24px rgba(19,38,63,.08)`): the Facebook card on paper, so a white card reads against near-white ground.
- **Float** (`box-shadow: 0 10px 28px rgba(8,20,36,.3)`): the floating text circle, which overlays content.

### Named Rules
**The Texture Stays Under 4% Rule.** The diagonal lines never exceed about 4% white, so they never read as lines through the text.

## Shapes

Soft and borderless. Buttons, chips, eyebrow and the floating circle are full pills/circles (999px / 50%); the form card and the example photo use 24px; text fields use 10px. Arrow circles (44px) and step numbers (48px) are true circles. Borders appear only as hairline dividers between list rows, the ghost button's 2px outline, and the 2px transparent field border that turns Focus Blue on hover/focus. The Facebook card is 20px (see the not-canonized note in Do's and Don'ts).

## Components

### Buttons
- **Shape:** full pill, min-height 56px, 0 26px padding, Cal Sans 18px, optional 20px leading icon.
- **Primary:** brass fill, ink text; hover to Lit Brass. Inside the form it is full-width, and hover/focus add a 3px Focus Blue outline at 3px offset.
- **Ghost:** transparent, on-dark text, 2px border at 70% on-dark; hover to solid white border and 10% white fill. Used on navy only.
- **Press:** `scale(.98)`. Hover styles live inside `@media (hover:hover)` so taps never stick.
- The hero holds at most two: "Get a quote" (primary) and "Text us" (ghost, SMS). There is no Call button; the number lives in the header.

### Header
Paper, 68px (80px desktop). Left: navy monogram (44px, 52px desktop) with "R&M Coatings" in Cal Sans and the logo tagline "Performance. Defined." as 11px uppercase tracked system text in Soft Slate. Right: tap-to-call number in Cal Sans 18px (20px desktop) with a Brass Ink phone glyph; hover turns it Brass Ink. Not sticky, no shadow.

### Hero
Plain navy band with texture; on 1024px+ the white monogram sits at 7% opacity in the empty right half, never behind text. Content: eyebrow, H1 (with Display type and the bounce-in), promise, two buttons.

**H1 bounce-in.** JS splits the H1 into letters (inside nowrap word wrappers, keeping the accent span). Each letter runs from `opacity:0; translateX(50px)` to rest over 1s `cubic-bezier(.34,1.56,.64,1)`, staggered 20ms. It waits up to 600ms for Cal Sans so letters don't reflow. The H1 carries an `aria-label` during the animation with letter spans `aria-hidden`; on the last `animationend` the original HTML is restored and the label removed. Without JS or under reduced motion the plain heading shows immediately.

### Eyebrow pill (house-style exception, used three times)
14px/500 system text, a 7px brass dot, 9px 14px padding, pill, 6% ink tint on light (12% white on dark). Marked up as `<p>`, never a heading; no hover, arrow or shadow. It appears only above the hero H1 ("Floors and paint"), the job heading ("Recent job") and the quote heading ("Takes a minute"). This is Ellie's explicit 2026-10-19 house-style choice; the Impeccable craft floor flags eyebrows, so it is documented as an existing exception, not a pattern to extend. Do not add new eyebrows without Ellie asking.

### Job claims list
Three rows on paper, Cal Sans `clamp(20px, 5.4vw, 24px)`, each led by a 36px stroked check-in-circle in Brass Ink, separated by hairlines. Statements of fact from the client's own post only.

### Facebook card
White card (20px radius, Card lift shadow, max 440px, min-height 72px): Facebook glyph in Facebook blue, "See more of our work on Facebook" in Cal Sans, and a 44px arrow circle on 7% ink. Hover fills only the arrow brass; focus fills it brass with a Focus Blue outline on the arrow.

### Service rows (signature)
Five full-width rows on navy, each the whole link: Cal Sans title, min-height 76px, white 14% hairlines above each and below the last, a 44px arrow circle on 10% white at the right. **Only the arrow changes**: hover and focus fill it brass with ink arrow; the row itself gains no background, underline or shadow. Each row jumps to the form and pre-selects the matching chip (Floors / Painting / Whole home).

### Example photo
`lvp-example.webp`, 4:5, `object-fit: cover`, 24px radius, max 420px (360px desktop, under the services heading), lazy-loaded. It is a generated example of an LVP floor, not an R&M job; it carries no caption, title or arrow and must never be presented as client work.

### Steps
Ordered list on deep navy: 48px brass circles with ink CSS-counter numerals (Cal Sans 20px), a Cal Sans title and one line of on-dark-soft body. Stacked with 24px gap on phones, three columns with 40px gap at 1024px.

### Quote form
- **Container:** white card, 24px radius, `clamp(20px, 5vw, 32px)` padding, 20px field gap, max 600px.
- **Labels:** Cal Sans 16px ink, `for`-linked; optional marked with a small "(optional)" in Soft Slate.
- **Chips:** radio inputs visually hidden behind pill labels (48px tall, Field Mist fill, 2px transparent border). Hover: Focus Blue border. Selected: Ink fill, white text. Keyboard focus: 3px Focus Blue outline at 3px offset (an outline, so it stays visible on the ink fill).
- **Inputs / textarea:** Field Mist fill, 10px radius, 2px transparent border, 16px text, 52px min (textarea 120px, vertical resize), navy caret. Hover and focus: Focus Blue border, no glow.
- **Errors:** a plain sentence in Error Red under the field, plus an Error Red border that wins over focus (a later, more specific rule), and `aria-invalid`. Submit focuses the first bad field.
- **Submit:** full-width primary button "Text this to R&M" with chat glyph. It composes "Hi R&M Coatings, this is {name}. I'd like a quote for {job}. Rooms: {rooms}. Town: {town}." and opens `sms:`.
- **Fallback:** if the page is still visible 900ms later (no messages app), a `role="status"` line appears in bold ink: "Didn't open your messages? Copy the message and send it to us." with an underlined text button that copies via the Clipboard API. A Soft Slate note under the form points to the phone number.

### Close band
Navy. Headline "Call R&M Coatings." with the name in brass, a short line in on-dark-soft, a service-area sentence (max 40ch), and the giant phone number in Cal Sans `clamp(30px, 9vw, 52px)` with a brass phone glyph sized at 0.8em; hover turns the number brass.

### Footer
Deep navy with texture, 48px top padding and 96px bottom (plus safe area) so the floating circle never covers it. Business name and a Facebook link (44px min tap height), links hover to brass.

### Floating text circle
60px brass circle with an ink chat glyph, fixed 16px from the bottom-right (plus safe-area insets), Float shadow. It opens the same pre-filled `sms:` as the hero ghost button. It slides in (`translateY(120px)` to rest, .35s `cubic-bezier(.2,.8,.2,1)`) once the hero is out of view and slides away while the quote form is on screen; when hidden it is `tabIndex=-1` and `aria-hidden`. Hidden entirely without JS or IntersectionObserver, and removable with `CONFIG.FLOAT=false`. One circle, never a bottom bar.

### Motion: fade-up
Elements marked `.rise` that start below the first screen get a `.below` class (opacity 0, `translateY(12px)`) and rise over .4s `cubic-bezier(.16,1,.3,1)` when they enter (8% bottom margin). Everything is visible at rest: nothing is hidden without JS, under reduced motion, or if it starts on the first screen. Reduced motion also turns off smooth scrolling and button/float transitions.

### Accessibility notes
- Focus ring: 3px Focus Blue at 3px offset on light grounds; brass on navy, deep, hero and footer.
- Tap targets 44px or larger throughout (header links, arrows, footer links, copy button padded to 44px).
- Measured contrast: body 10.7:1, soft 6.7:1 and brass-ink 6.4:1 on paper; on-dark-soft 7.7:1 on navy; ink on brass 7.2:1; brass on navy 5.5:1; placeholder (#55606e) 5.4:1 on Field Mist; Focus Blue 6.4:1 on white.
- Field Mist against the white card is only about 1.2:1, so field edges rely on their labels and the hover/focus border; treat this as a known weak boundary, not a target.
- Eyebrows are `<p>`; every section is `aria-labelledby` its heading; decorative SVGs and monograms are `aria-hidden` / `alt=""`; the example photo has descriptive alt text.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed bands light/dark (paper, navy, paper, deep, paper, navy, deep) so each section is obvious.
- **Do** use brass as a fill with Ink text, and Brass Ink (`#7a5200`) whenever brass must be text on paper.
- **Do** set every heading, button and big label in Cal Sans 400, with the body on the system stack at 16/1.7.
- **Do** make list rows whole links and change only the arrow circle on hover/focus.
- **Do** outline form controls in Focus Blue on hover and focus, and keep error borders winning over focus.
- **Do** keep everything visible at rest; motion only adds, never withholds content.
- **Do** keep hover styles inside `@media (hover:hover)`.

### Don't:
- **Don't** put white text on brass, or brass text on paper.
- **Don't** present `lvp-example.webp` (or any generated image) as an R&M job; the client has published no work photos.
- **Don't** letter-animate any heading other than the hero H1.
- **Don't** add a bottom bar, a Call button in the hero, or a second floating control.
- **Don't** use hard or offset shadows; the only shadows are Card lift and Float.
- **Don't** push the diagonal texture above about 4% white.
- **Don't** add eyebrow pills beyond the three Ellie's house style placed; they are a flagged exception, not a heading pattern.
- **Don't** canonize one-offs from this build: the Facebook card's 20px radius (cards are 24px), the inline `margin-top` spacing on the job heading, and Facebook blue (`#1877f2`), which is the Facebook glyph's own colour, not a palette token.
