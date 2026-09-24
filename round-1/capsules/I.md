# I — concept capsule

## Premise
The ARC-AGI-3 research log keeps "one entry per change, newest at the bottom". The page orders its entries by when each last changed on GitHub — Jovian Engine (oldest), Cards Against The Humanity (2026-09-20), ARC-AGI-3 (2026-09-24), this site at joviangame.me (newest) — and grows downward: each newer entry is set larger, so the weight sits on the bottom edge and the last line is the address.

## Type
- **Montagu Slab** — Florian Karsten. Primary source: github.com/floriankarsten/montagu-slab. SIL OFL 1.1, no Reserved Font Name. Embedded subset: wght 400–460, full optical-size range 16–144. Fallback: generic serif only.
- Optical size follows rendered size automatically. Names wght 450; supporting lines wght 400. Case as written.

## Scale, line and space
- Newest entry size x = min(content width ÷ 7.6, 160px). Each older entry is divided by r (r = 2 at ≥ 720px, 1.5 below): 160 / 80 / 40 / 20px at desktop; the oldest never below 16px.
- Supporting lines = max(15.2px, 0.3 × entry size). Names line-height 1.02; supporting 1.35.
- The column is anchored to the bottom margin; the space above the oldest entry is empty. Gap before each entry = 0.55 × its size. Left aligned. Margins clamp(16px, 3.2vw, 52px); bottom clamp(16px, 3vw, 40px).
- In the newest entry the handle comes first and the address last.

## Colour
- Canvas `#0d1521`.
- Tertiary — oldest entry `#8195ae` — ≈ 5% of ink — 6.0 : 1.
- Secondary — middle entries `#d8c6a2` — ≈ 35% — 10.9 : 1.
- Primary — newest entry (JustAdev742, joviangame.me) `#ffb347` — ≈ 60% — 10.3 : 1.

## Signature
Size and colour follow recency; the site's own address is the last and largest line.

## Invariants
Order by real last-change date; newest at the bottom and largest; content anchored to the bottom.

**Allowed variation:** the ratio r; how colour bands map to recency as entries are added.
**Prohibited normalization:** reordering by importance; anchoring to the top; equalizing sizes.

## Assumptions and risks
- The order changes whenever a repository is pushed; it must be regenerated.
- Jovian Engine's date uses the older of its two repositories.
- At desktop the oldest entry is set at 20px.

## Round 2 translation
Compute the order from GitHub push dates at build time. New entries enter at the bottom and push the others up and smaller.
