# D — concept capsule

## Premise
In the game "the address bar only ever carries the table code, because that is the one thing worth scanning or sharing", and the brief asks for the site to link exactly joviangame.me. The address is the page's spine: set sideways up the full height of the left edge, it is the frame everything else hangs from. Everything else is small.

## Type
- **Commissioner** — Kostas Bartsokas. Primary source: github.com/kosbarts/Commissioner. SIL OFL 1.1, no Reserved Font Name. Embedded subset: wght 400–850, FLAR 0–100, VOLM 0–100, slnt pinned at 0. Fallback: generic sans-serif only.
- **Spine (the address):** wght 850, FLAR 0, VOLM 0 — the plainest, most typeable forms; tracking −0.004em.
- **Names:** uppercase, tracking 0.045em, wght 700, FLAR 100, VOLM 60 (flared), case-sensitive forms, balanced lines.
- **Handle:** wght 560, FLAR 0, tracking 0.03em.
- **Sentences:** wght 420, FLAR 30. **Addresses and facts:** wght 420, FLAR 0.

## Scale, line and space
- Spine size = (viewport height − 2 × margin) ÷ 7.12, so its length is ≈ 98% of the height; line-height 1; reads bottom to top (vertical writing mode turned 180°).
- Names clamp(20.8px, 0.95rem + 1.5vw, 36.8px), line-height 1.1. Small text clamp(15px, 0.9rem + 0.2vw, 17px), line-height 1.45.
- Two-column grid: spine column (as wide as the spine's size) and content column (≤ 36rem); gap clamp(20px, 3.4vw, 64px); outer margin clamp(16px, 2.8vh, 36px) top, bottom and left.
- The content column spans the spine's height, with space distributed between its four groups: handle at the top, the last project at the bottom. Name → sentence 0.6rem; sentence → address 0.15rem.

## Colour
- Canvas `#1d2a8a`.
- Primary — the spine `#f3ee9f` — ≈ 65% of ink — 10.0 : 1.
- Secondary — everything else `#bcc4ff` — ≈ 35% — 7.1 : 1.

## Signature
The address as a full-height sideways spine that everything else hangs from.

## Invariants
The address runs the full height of the left edge; it is the only heavy text and the only text in the primary colour; everything else is small.

**Allowed variation:** FLAR/VOLM settings of the names; how groups distribute along the height.
**Prohibited normalization:** turning the address into a horizontal header or logo, shrinking it to a navigation item, letting names compete with it in size.

## Assumptions and risks
- The spine is read with the head turned (one word only).
- On wide, short windows the spine gets small; on tall phones the content column narrows to about 220px.
- Uses writing-mode with a 180° turn for broad browser support.

## Round 2 translation
Every page keeps the spine, which links to joviangame.me. All interactive content lives in the column; nothing else enters the spine's colour.
