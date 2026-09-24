# G — concept capsule

## Premise
The owner's bot scorer rewards "how much of a picture it paints": "A card earns its imagery from what is actually in it — physical words, names, numbers, bodily words, adjectives you could see — and loses it for abstract morphology and concept words." The page sets all copy as continuous text at one size; each word's weight is its picture value.

## Type
- **Crimson Pro** — Jacques Le Bailly / Fonthausen. Primary source: github.com/Fonthausen/CrimsonPro. SIL OFL 1.1, no Reserved Font Name. Embedded subset, full weight range 200–900. Fallback: generic serif only.
- Weight map (the rule, applied word by word):
  - 900 — names and numbers: JustAdev742, the two project names, Kaggle., ARC Prize 2026
  - 800 — bodily words: hands.
  - 700 — physical nouns: TV, table, phones
  - 600 — addresses: joviangame.me, the Cards Against The Humanity address
  - 300 — abstract or vague words: Developing, AI, stuff
  - 200 — function words: The, is the, are the, on
- Old-style figures; lining figures and case forms in "ARC-AGI-3" and "ARC Prize 2026". Case as written.

## Scale, line and space
- One size clamp(30px, 1rem + 3.7vw, 72px); line-height 1.1; measure 15.5em.
- Three paragraphs (host; Cards Against The Humanity; ARC-AGI-3), no space between them; each after the first indented 1.1em. Left aligned, ragged right, no hyphenation.
- Padding: sides clamp(20px, 5.5vw, 96px); top clamp(24px, 7vh, 80px); bottom clamp(48px, 12vh, 128px).

## Colour
- Canvas `#dfe7bf`.
- Primary — all text `#2a1233` — 100% — 13.2 : 1.

## Signature
Weight follows how much of a picture each word paints.

## Invariants
One size. Weight comes only from the picture-value rule, never from emphasis. Continuous paragraphs.

**Allowed variation:** the exact map as copy changes (the rule stays); measure.
**Prohibited normalization:** separate headings; bold names with everything else regular; extra colours; list layout.

## Assumptions and risks
- New copy must be scored by the same rule; borderline words need a recorded decision.
- Weight 200 must never be set below about 20px.

## Round 2 translation
Long-form project text follows the same rule. Links must be distinguishable without new weights; that needs a decision (position, or a second tone if the direction is reopened).
