# C — concept capsule

## Premise
In the game the Czar turns answers over one at a time and each card "writes itself into the black card on the TV as it is read out, so the whole room is reading the same joke at the same time". The page is a script read aloud by one voice: one typeface, one size, one weight, one colour. Hierarchy is carried only by pauses, measured in lines of silence.

## Type
- **Linden Hill** (regular) — Barry Schwartz / The League of Moveable Type. Primary source: github.com/theleagueof/linden-hill. SIL OFL 1.1 with Reserved Font Name "Linden Hill"; the embedded WOFF2 subset is a Modified Version renamed "R1C Serif" inside the file, as the licence requires. The font's own name table also carries an MIT notice. Fallback: generic serif only.
- Default old-style figures; standard ligatures; case as written; no italic, no small caps.

## Scale, line and space
- One size: clamp(24px, 1rem + 2.1vw, 42px); line-height 1.34 (one line, L = 1.34em); measure ≤ 22em.
- Pauses: opening 3L; within a card, name → description 1L (a breath); description → address 0.5L; next card 5L; end 5L. Consecutive lines with no pause: the handle and the domain.
- Line breaks follow speech: "The TV is the table," / "phones are the hands." The address may break after the slash or at hyphens. No hyphenation.
- One left-aligned column, left edge at clamp(20px, 24vw, 448px), right padding 20px, ragged right.

## Colour
- Canvas `#3b0f1a`.
- Primary — the voice `#f5d9c7` — 100% of text — 12.3 : 1.

## Signature
Nothing changes size or weight; five-line silences separate the cards.

## Invariants
One size, one weight, one colour. Spacing only in whole or half line units. Breaks at spoken phrase boundaries.

**Allowed variation:** pause lengths within the unit system; column offset.
**Prohibited normalization:** bold or larger names, a second colour, collapsing pauses into ordinary paragraph spacing.

## Assumptions and risks
- Names are marked only by position and silence; long pages mean scrolling through silence.
- The face has one weight; Round 2 states (hover, focus, current page) must also avoid new sizes and weights.

## Round 2 translation
Every screen is a script. Links read as spoken lines; states use pause, position or — only if reopened — a second tone.
