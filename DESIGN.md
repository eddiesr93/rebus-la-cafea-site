---
name: Rebus la cafea (site)
description: The site typed on the app's crossword keyboard, the one keyboard that has Ă Â Î Ș Ț.
colors:
  case: "#173a2b"
  case-hi: "#1f4836"
  case-deep: "#0f281d"
  case-wall: "#0a1c14"
  on-case: "#f4efe3"
  on-case-2: "#bcd2c5"
  paper: "#f3eee2"
  paper-2: "#e8e1d0"
  ink: "#1c211e"
  ink-2: "#4c534e"
  rule: "#d5ccb8"
  green: "#235a43"
  sage: "#dce8dd"
  solved: "#c7e0cd"
  cap: "#faf6ec"
  cap-hi: "#ffffff"
  cap-wall: "#cbc1ab"
  dia: "#dce8dd"
  dia-hi: "#f0f6f0"
  dia-wall: "#9fb8a6"
  dia-ink: "#1f5640"
  enter: "#fffdf8"
  enter-wall: "#d2c7ae"
  enter-ink: "#173a2b"
  crema: "#f1c66b"
  crema-hi: "#f8dc9c"
  crema-wall: "#b98a30"
  crema-ink: "#2a1f0b"
  error: "#a6291a"
  cell: "#fffdf8"
  block: "#1c211e"
  line: "#b9b3a5"
typography:
  display:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(2.75rem, 6.6vw, 5.75rem)"
    fontWeight: 750
    lineHeight: 0.96
    letterSpacing: "-0.035em"
    fontVariation: "'wdth' 92"
  headline:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(2.125rem, 4.4vw, 3.5rem)"
    fontWeight: 750
    lineHeight: 1.02
    letterSpacing: "-0.03em"
    fontVariation: "'wdth' 94"
  title:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "1.5rem"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.015em"
  legend:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 600
    lineHeight: 1.2
  lede:
    fontFamily: "Rebus Digits, Atkinson Hyperlegible Next, ui-sans-serif, system-ui, sans-serif"
    fontSize: "1.1875rem"
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: "Rebus Digits, Atkinson Hyperlegible Next, ui-sans-serif, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.6
    fontFeature: "lnum"
  label:
    fontFamily: "Rebus Digits, Atkinson Hyperlegible Next, ui-sans-serif, system-ui, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 700
    fontFeature: "tnum"
rounded:
  cell: "6px"
  board: "8px"
  fn: "10px"
  key: "14px"
  clue: "16px"
  deck: "clamp(20px, 3vw, 30px)"
  case: "clamp(28px, 4vw, 56px)"
spacing:
  gutter: "clamp(1rem, 4vw, 3rem)"
  frame: "min(100vw - 2 * gutter, 76rem)"
  rail: "calc(frame / 12) at >= 60rem, 0 below"
  section-gap: "clamp(4.5rem, 10vw, 8rem)"
  key-wall: "7px"
  small-wall: "4px"
  target: "44px"
components:
  key-cap:
    backgroundColor: "{colors.cap}"
    textColor: "{colors.ink}"
    rounded: "{rounded.key}"
    height: "4rem"
  key-diacritic:
    backgroundColor: "{colors.dia}"
    textColor: "{colors.dia-ink}"
    rounded: "{rounded.key}"
    height: "clamp(4.25rem, 8vw, 6.25rem)"
  key-diacritic-pressed:
    backgroundColor: "{colors.crema}"
    textColor: "{colors.crema-ink}"
    rounded: "{rounded.key}"
  key-enter-iso:
    backgroundColor: "{colors.enter}"
    textColor: "{colors.enter-ink}"
    rounded: "{rounded.key}"
    height: "7.75rem"
    width: "17rem"
  fn-key:
    backgroundColor: "{colors.case-hi}"
    textColor: "{colors.on-case}"
    typography: "{typography.legend}"
    rounded: "{rounded.fn}"
    height: "44px"
    padding: "0 0.95rem"
  tag-free:
    backgroundColor: "{colors.cap}"
    textColor: "{colors.ink}"
    typography: "{typography.legend}"
    rounded: "{rounded.fn}"
    padding: "0 0.8rem"
    height: "2.25rem"
  tag-premium:
    backgroundColor: "{colors.dia}"
    textColor: "{colors.dia-ink}"
    typography: "{typography.legend}"
    rounded: "{rounded.fn}"
    padding: "0 0.8rem"
    height: "2.25rem"
  clue-bar:
    backgroundColor: "{colors.sage}"
    textColor: "{colors.ink}"
    rounded: "{rounded.clue}"
    padding: "0.85rem 1.1rem 0.9rem"
  grid-cell:
    backgroundColor: "{colors.cell}"
    textColor: "{colors.ink}"
    rounded: "{rounded.cell}"
    size: "2.5rem"
  grid-cell-typed:
    backgroundColor: "{colors.crema}"
    textColor: "{colors.crema-ink}"
---

# Design System: Rebus la cafea (site)

> Scope: the marketing, support and privacy site (`index.html`, `confidentialitate/`). The iOS app in `../rebus-la-cafea` has its own DESIGN.md and a deliberately different world; nothing here applies to the app, and the app's palette does not bind the site.

## Overview

**Creative North Star: "Tastatura cu diacritice"**

The page is typed on the one keyboard that has Ă Â Î Ș Ț: the app's crossword keyboard, seen once and seen large. A deep green keyboard case bookends the page (header plus first section on top, footer at the bottom, each with a large rounded inner edge), and everything between is warm paper. On that case sit physical keycaps: cream faces with a visible side wall underneath, sage keys for the diacritics, and an ISO inverted-L Enter key that is always the primary action. Crossword grids are drawn as real careuri: ink frame, hairline seams, numbered cells, black blocks.

Density is calm and generous. Text registers to one off-centre rail (the home row): from 60rem up, every heading, paragraph and list starts one-twelfth of the frame in from the left; the large objects (deck, spacebar, screenshots) may run full frame. The page works without JavaScript; the only interaction is CSS (radio keys, `<details>`), and every interaction is a key being pressed.

Rejected by the build: the split hero with a phone mockup, feature-card grids, pricing cards.

**Key Characteristics:**
- Green case top and bottom, paper in the middle; tone changes carry the structure, not boxes.
- Keys have a face, a side wall (a solid bottom border) and a press that eats the wall.
- Crema appears only where a letter is being typed: the pressed key and the target cell.
- Grids are real crossword grids, never decorative pattern.
- One off-centre rail; everything readable sits on it.
- Light and dark follow `prefers-color-scheme`; every token has a dark counterpart.

## Colors

A green-and-paper keyboard with one warm accent, crema, held back for the act of typing.

### Primary
- **Keyboard Case Green** (`case`, with `case-hi` for the lit top of the gradient, `case-deep` for the recessed deck well, `case-wall` for function-key walls): the top and bottom bookends of every page; also the `theme-color`. Text on it is **Case Cream** (`on-case`) and **Lichen** (`on-case-2`) for ledes and secondary lines.
- **Legend Green** (`green`): links, focus rings on paper, clue-direction labels, clue numbers, the success line, FAQ toggles, the scrollbar thumb.

### Secondary
- **Sage Diacritic** (`dia` / `sage`, same value in light): diacritic keycaps (with `dia-hi` face highlight, `dia-wall` side wall, `dia-ink` legend), the clue bar, the active word row in the hero grid, the Premium tag. **Solved Sage** (`solved`) fills the word row once ROȘU is correct.

### Tertiary
- **Crema** (`crema`, `crema-hi`, `crema-wall`, `crema-ink`): the pressed key's face, wall and legend; the cell being typed; the focus ring on the green case; text selection (`crema-hi` on `crema-ink`).

### Neutral
- **Paper** (`paper`) and **Paper Shade** (`paper-2`): the page between the case bookends; `paper-2` is the struck-through "mods" chips and screenshot placeholders.
- **Ink** (`ink`) and **Ink Muted** (`ink-2`): body text and secondary text/captions/meta.
- **Rule** (`rule`): 1px dividers for clue lists, ledger rows, FAQ items; also the wall of the struck "mods" chips.
- **Keycap Cream** (`cap`, `cap-hi`, `cap-wall`): the spacebar and the "Gratuit" tags. **Enter Cream** (`enter`, `enter-wall`, `enter-ink`): the ISO Enter key and the skip link.
- **Grid** (`cell`, `block`, `line`): crossword cells, black squares, and the 1px seam colour that shows between cells.
- **Error Red** (`error`): wrong-letter feedback, the "!" mark on a wrong cell, and the strike-through on the "mods" chips. Never used as decoration.

### Named Rules
**The Crema Is Typing Rule.** Crema marks only the key being pressed and the cell receiving the letter (plus focus on the green case and text selection, both acts of pointing). Never a section background, never a badge, never a heading colour.

**The Two Bookends Rule.** Case green appears as the top case and the bottom case of a page, not as alternating section bands. Pages between them sit on paper.

**The Dark Twin Rule.** Every colour token is redefined in the `prefers-color-scheme: dark` block (case darkens, paper becomes near-black `#121412`, keycaps become dark green-grey, `green` lifts to `#8cc2a2`, `error` to `#ff9f8e`). New colours must be added as tokens with a dark value, never as literals.

## Typography

**Display Font:** Bricolage Grotesque, variable 200–800, width 75–100% (fallback `ui-sans-serif, system-ui`)
**Body Font:** Atkinson Hyperlegible Next, 400–700 plus italic (same fallbacks)
**Digits:** "Rebus Digits", a `unicode-range` face that maps 0–9 to Bricolage, stacked first in the body family

**Character:** Bricolage is the keycap legend and the headline voice: tight, slightly condensed, heavy. Atkinson is for reading, chosen for older readers. Its slashed zero reads as „Ø” in Romanian copy, so digits in running text come from Bricolage.

### Hierarchy
- **Display** (750, `clamp(2.75rem, 6.6vw, 5.75rem)`, 0.96, width 92%, -0.035em): the hero H1 only, max 13ch. The spacebar H2 uses a sibling (760, `clamp(2.25rem, 5.6vw, 4.75rem)`, 0.98, width 90%) and the privacy H1 another (750, `clamp(2.25rem, 5vw, 3.75rem)`, 1.0, width 92%).
- **Headline** (750, `clamp(2.125rem, 4.4vw, 3.5rem)`, 1.02, width 94%, -0.03em): section H2s.
- **Title** (650–700, 1.375–1.625rem, -0.015em): clue-list H3s, support H3s, privacy H2s (1.5rem/700).
- **Legend** (600–700, 0.9375rem in Bricolage): function keys, tags, chips, Enter-key secondary line; the Enter key's strong line is 1.3125rem/700. Diacritic key legends are `clamp(1.75rem, 3.6vw, 2.875rem)`/600.
- **Lede** (400, 1.1875rem, 1.55): hero lede (34ch), section intros (46ch), promise body.
- **Body** (400, 1.0625rem, 1.6, lining numerals): paragraphs at 40–68ch; FAQ answers 65ch, privacy paragraphs 68ch.
- **Label** (700, 0.875rem, tabular numerals, sentence case): clue directions („1 Orizontal · 4 litere”) with an arrow icon, in `green`. Meta lines at 0.875–0.9375rem in `ink-2`.

### Named Rules
**The Legend Rule.** Anything that is a key, tag, chip, grid letter or heading speaks Bricolage; anything you read for more than a line speaks Atkinson.

**The No Slashed Zero Rule.** Keep "Rebus Digits" first in the text stack so numbers in Romanian copy never render Atkinson's slashed zero.

## Layout

Single column frame: `min(100vw - 2 × gutter, 76rem)` centred, gutter `clamp(1rem, 4vw, 3rem)`. Sections are separated by `section-gap` (`clamp(4.5rem, 10vw, 8rem)`) of open paper, not by rules or boxes.

**The rail.** At 60rem and up, `--rail` = frame / 12 and all text blocks (section heads, lists, ledger, support grid, privacy document) start on it. Below 60rem the rail collapses to 0. Large objects (hero deck, spacebar, screenshots row) may span the full frame; the spacebar's own padding aligns its heading back to the rail.

Responsive steps (observed): 26rem (header tightens), 48rem (ISO Enter gets its stem, screenshot row becomes a 1.3fr + 3×1fr grid aligned to the rail, clue list goes two columns, footer goes two columns), 60rem (rail on; hero deck becomes three columns board | clue + keys | Enter; support becomes contact (sticky) + FAQ at 1 : 1.75). Under 48rem the hero grid shows only its answer row so clue, keys and Enter stay above the fold, and the screenshot row becomes a horizontal snap scroller at 66% per card.

Tap targets are at least 44px (header keys, brand, footer links, email link, FAQ summaries at 3.5rem).

## Elevation & Depth

Depth is physical and keyboard-like: a keycap is lifted by its **side wall** (a solid bottom border in the key's darker wall colour, 7px on large keys, 4px on small ones) plus a soft drop below and a 1px top highlight. The deck the keys sit in is the opposite, an inset well. Everything else (paper sections, lists, FAQ) is flat and divided by 1px rules.

### Shadow Vocabulary
- **Key drop** (`0 14px 20px -10px rgb(0 0 0 / 0.5)` with `inset 0 1px 0 rgb(255 255 255 / 0.55)`): keycaps and the ISO Enter at rest. On press: `0 6px 10px -6px rgb(0 0 0 / 0.5)`.
- **Deck well** (`inset 0 3px 8px rgb(0 0 0 / 0.45), inset 0 -1px 0 rgb(255 255 255 / 0.06)`): the recessed tray on `case-deep` holding grid, clue, keys and Enter.
- **Spacebar lift** (`0 26px 40px -24px rgb(28 33 30 / 0.55)` + top highlight): the large no-ads key.
- **Object on paper** (`0 2px 4px rgb(28 33 30 / 0.08), 0 26px 44px -26px rgb(28 33 30 / 0.55)`): screenshots. Grids use `0 16px 28px -14px rgb(0 0 0 / 0.65)`; ledger tags `0 8px 12px -10px rgb(28 33 30 / 0.5)`.

### Named Rules
**The Wall Is the Press Rule.** Pressing a key moves the face down by `wall − 2px` and shrinks the wall to 2px (90ms, `cubic-bezier(0.16, 1, 0.3, 1)`). A selected key stays half-pressed (wall 3px). Depth is spent on keys, never on content containers.

## Shapes

Soft, keycap-rounded corners at a fixed ladder: grid answers 6px, grid frame 8px (with a 1.5–2px ink border and 1px seams), function keys and tags 10px, keycaps and Enter 14px, clue bar 16px, deck `clamp(20px, 3vw, 30px)`, spacebar `clamp(20px, 3vw, 28px)`, screenshots `clamp(22px, 3vw, 36px)`, and the case bookends' inner edge `clamp(28px, 4vw, 56px)` (bottom corners of the top case, top corners of the bottom case). Keycap faces are dished with a radial gradient from the highlight at the top centre. The ISO Enter is an inverted L built from a wide top and a narrower stem (74% width) on the right.

## Components

### Keycaps (signature)
Tactile, heavy, unmistakably pressable.
- **Shape:** 14px radius, 7px side wall, dished radial-gradient face.
- **Diacritic key:** sage face, green legend in Bricolage 600; height `clamp(4.25rem, 8vw, 6.25rem)`; five in a row. The Ș key carries the home-row nub (a short 3px bar at 35% opacity).
- **Pressed/selected:** crema face, crema wall, crema-ink legend, wall reduced to 3px.
- **Hover:** face highlight brightens toward white. **Focus:** 3px crema outline, 3px offset (on the case).
- **Behaviour:** CSS-only radio inputs; the matching cell pops in (260ms scale from 0.6). Wrong letters show red feedback and a "!" in the cell; the right one fills the word row with `solved`.

### ISO Enter key (primary action)
The only primary button. Enter-cream face, `enter-ink` text: a bold 1.3125rem line („Descarcă gratuit”) over a 0.9375rem line („din App Store”), with the return-arrow icon on the stem. Below 48rem it collapses to a single wide key with the icon inline. Focus ring is crema on the case, green on paper. Used in the hero, after the Premium ledger and in the footer, always as the App Store link.

### Function keys (navigation)
Header navigation as a row of small dark-green keys: 44px tall, 10px radius, 4px `case-wall` wall, Bricolage 600 at 0.9375rem, `on-case` text; press moves 2px. „Confidențialitate” hides under 48rem. Footer navigation is plain underlined links on the case.

### Spacebar
The no-ads promise as one wide keycap: cream face, `clamp(8px, 1.2vw, 12px)` wall, spacebar lift, H2 inside. One per page; it carries one truth.

### Crossword grid
Real careuri: ink border, `line` seams 1px, `cell` faces, `block` squares, small clue numbers at 0.32em in the top-left of numbered cells, letters in Bricolage 600 sized to the container (`9cqi`). The inline **answer strip** (2.5rem cells, 6px radius) shows feature answers next to a length label („Orizontal · 5 litere”).

### Clue bar
Sage panel, 16px radius: direction label with arrow icon, clue text in Bricolage 550 at `clamp(1.25rem, 2.2vw, 1.5rem)`, feedback line beneath.

### Tags and struck chips
Small keycaps (10px radius, 4px wall, Bricolage 600–650 at 0.9375rem): „Gratuit” on cap cream, „Premium” on sage. The no-ads "mods" are paper-2 chips with a `rule` wall and a 2px `error` strike-through.

### Lists, ledger, FAQ
Flat rows separated by 1px `rule` lines. Ledger rows ≥3.75rem with the tag at the right. FAQ uses native `<details>`; summary in Bricolage 600 1.125rem, a green plus that rotates 45° when open (220ms).

### Icons
Inline SVG sprite, 24px viewBox, stroke 2.2 (2.4 on Enter), round caps and joins, no fill, `currentColor`. Arrows for direction, return arrow for Enter, check/cross for feedback, plus for FAQ, envelope for email.

## Do's and Don'ts

### Do:
- **Do** make every action a key: face, side wall, press that consumes the wall (90ms, `cubic-bezier(0.16, 1, 0.3, 1)`).
- **Do** use the ISO Enter key for the App Store link and nothing else as a primary button.
- **Do** keep crema for the pressed key, the typed cell, focus on the case and selection only.
- **Do** register all reading text to the rail at 60rem and up.
- **Do** draw grids as real crossword grids with real Romanian words from the app.
- **Do** quote Romanian with „…” and keep digits in Bricolage via "Rebus Digits".
- **Do** keep interaction CSS-only and give every animation a reduced-motion fallback (state changes stay, movement goes).
- **Do** add a dark value for every new colour token.

### Don't:
- **Don't** use crema as a section fill, badge or heading colour.
- **Don't** add a second accent hue to the system; error red is feedback only.
- **Don't** wrap paper content in cards or shadowed boxes; depth belongs to keys, the deck, grids and screenshots.
- **Don't** put a phone mockup beside the hero headline, build feature-card grids, or show pricing cards (no price appears on the site at all).
- **Don't** add JavaScript, webfonts from a CDN, or any external resource.
- **Don't** reuse the app's DESIGN.md palette here, or this site's world in the app.
