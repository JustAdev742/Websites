# A — concept capsule

## Premise
Cards Against The Humanity is played with the TV as the shared table, read from across a room, and phones as private hands, read at arm's length ("Put the TV on the big screen, everyone else joins from their phone"; "The TV is the table, phones are the hands."). The page carries those two reading distances and nothing between them: shared text sized for the far distance, private text for the near one, at the ratio of the distances — about 2.4 m to 0.3 m, so 8 : 1.

## Type
- **Truculenta** — Iván Castro, Eva Sanz and Omnibus-Type. Primary source: github.com/Omnibus-Type/Truculenta. Licence: SIL OFL 1.1, no Reserved Font Name; web embedding allowed. Embedded as a WOFF2 subset (Latin; opsz 12–72, wdth 100–110, wght 400–600). Fallback: generic sans-serif only; not proof of the direction.
- **Far text (the table):** the three project names only. opsz 72, wdth 110, wght 560, tracking +0.004em, title case as written. "ARC-AGI-3" uses case-sensitive forms.
- **Near text (the hands):** everything else. opsz 12, wdth 100, wght 430, old-style figures.
- No third size, weight or style exists.

## Scale, line and space
- Near: clamp(13px, 0.7rem + 0.28vw, 15px), line-height 1.45, measure ≤ 21em.
- Far: 8 × near, capped at 16.5vw (on a 390px phone the ratio falls to ≈ 5 : 1; "two sizes only" holds at every width). Line-height 0.98; 0.3em between names; lines of at most 13 characters: "Cards Against / The Humanity", "Jovian Engine", "ARC-AGI-3".
- Page: full-viewport grid. Table at the top; an empty band (min 16vh, grows to fill) between; hands pinned to the bottom as one row of four blocks (two columns under 760px, one under 430px). Side margins clamp(20px, 4.4vw, 72px); top clamp(20px, 4.5vh, 56px); bottom clamp(20px, 4vh, 48px). Left aligned, ragged right. No overlap, no cropping.
- Seat order in the hands row: host (JustAdev742, joviangame.me), then the three projects in the table's order.

## Colour
- Canvas `#1a1512`.
- Primary — far text `#d5e3f7` — ≈ 75% of text ink — 13.9 : 1.
- Secondary — near text `#c8a17a` — ≈ 25% — 7.6 : 1.
- Rule: the shared far text is the brightest thing on the page; private text is warmer and dimmer.

## Signature
Only two sizes, 8 : 1 apart; the empty band between them stands for the distance across the room.

## Invariants
Two sizes only. Names only at the far size. The empty band between far and near. The far text is the most luminous colour.

**Allowed variation:** band height; seats per row at small widths; which fact sits in which hand.
**Prohibited normalization:** adding a middle size (subheads, labels), weight emphasis inside the hands, centring the table, filling the band.

## Assumptions and risks
- Working copy is provisional (see EVIDENCE.md).
- Each hand pairs with its name by order and content only; if unclear, move each hand under its name rather than adding labels.
- 8 : 1 comes from typical distances, not the owner's room.

## Round 2 translation
Keep exactly two text sizes on every screen. Links and focus states use colour, luminance or position — never a third size. On a TV-sized screen the far size may grow while the near size stays at hand size.
