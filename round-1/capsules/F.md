# F — concept capsule

## Premise
The ARC-AGI-3 agent perceives game frames through "exact grid perception: components, diffs, scale detection" and tracks entities with roles ("static/hud/avatar"). The page is built on an exact character grid: one monospaced face, every size an integer multiple of the base, every position a whole number of base cells and rows. Colour marks role, as in the entity tracker.

## Type
- **Commit Mono** — Eigil Nikolajsen. Primary source: github.com/eigilnikolajsen/commit-mono. SIL OFL 1.1, no Reserved Font Name. Embedded subset: upright, wght 400–600. Fallback: generic monospace (keeps the grid, not the forms).
- Kerning and ligatures off; tracking 0; every character exactly 0.6em. Case as written.
- Names and the avatar handle wght 600; everything else wght 400.

## Scale, line and space
- Base b = 14px (< 760px), 15px (760–1179px), 16px (≥ 1180px).
- Sizes: 1× (sentences, HUD), 2× (names), k× for the avatar handle with k = 3 / 4 / 6 by breakpoint. Line-height 1.5 of each size, so every line is a whole number of base rows.
- Margins 3ch (narrow) or 6ch. Vertical order: 2 rows, HUD row (handle left, domain right), 1 row, avatar, 3 rows, entity grid. Entity columns 36ch, gap 4ch, row gap 3 rows; they flow 3 / 2 / 1 across by width. Inside an entity: name, 1 row, sentence, address.

## Colour
- Canvas `#e8e8e2`.
- Primary — entities (project names) `#1b2a5c` — ≈ 30% of ink — 11.1 : 1.
- Secondary — static (sentences) `#24502f` — ≈ 20% — 7.5 : 1.
- Tertiary — HUD (handle at 1×, joviangame.me, the address, ARC Prize 2026) `#8b3a0e` — ≈ 15% — 6.3 : 1.
- Accent — avatar (handle at k×) `#b0135a` — ≈ 35% — 5.5 : 1.

## Signature
The handle at 1× directly above its exact integer upscale, both starting on the same column; each large character covers exactly k base cells.

## Invariants
Integer scales only; grid units only (ch and rows); four colours map to four roles; one monospaced face.

**Allowed variation:** k per breakpoint; number of entity columns.
**Prohibited normalization:** non-integer sizes, proportional type, colour used for decoration, a dark terminal canvas.

## Assumptions and risks
- Monospace can read as a generic developer look; the integer-scale relationship and the role colours carry the difference.
- In Round 2 every new state needs a role, not a new colour.

## Round 2 translation
Size every component in base cells and rows. Focus and hover change role colour or grid position, never size by a fraction. The avatar role can mark the viewer's current place.
