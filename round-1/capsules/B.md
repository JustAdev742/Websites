# B — concept capsule

## Premise
The owner's bot README defines the joke as a register clash: "A prim setup with an indecent answer … a voice putting on a smile is a voice worth ruining." The page stages a courteous, symmetrical setup voice and lets oversized, blunt, lowercase answers land through it. Every item is ordered setup → answer, as a card is read.

## Type
- **Cormorant Garamond** (roman + italic) — Christian Thalmann / Catharsis Fonts. Primary source: github.com/CatharsisFonts/Cormorant. SIL OFL 1.1, no Reserved Font Name. Embedded subset pinned at wght 500 (small caps and case forms kept).
- **Anybody** — Tyler Finck / Etcetera Type Co. Primary source: github.com/Etcetera-Type-Co/Anybody. SIL OFL 1.1, no Reserved Font Name. Embedded subset pinned at wdth 150, wght 900.
- Fallbacks: generic serif / sans-serif only.
- **Setup voice (prim):** Cormorant. Sentences in italic; the handle, the addresses and "ARC Prize 2026" in all small caps, tracking 0.2em (0.2em left padding re-centres the tracked line), old-style figures.
- **Answer voice:** Anybody extended black, lowercase via text-transform, for the three project names only.

## Scale, line and space
- Small caps clamp(17px, 0.98rem + 0.3vw, 20px), line-height 1.5. Header address (italic) clamp(18px, 1rem + 0.4vw, 22px).
- Setups clamp(20.8px, 1.08rem + 0.95vw, 30px), line-height 1.28, measure 21em, balanced, centred.
- Answers: size = measure ÷ 12.9 (so "cards against" fills ≈ 96% of the measure); under 700px, measure ÷ 8.7 (one word per line). Line-height 0.86; 1.04 under 700px (keeps the g of "against" clear of the h of "the"). Tracking −0.004em. Flush left.
- Page sides clamp(16px, 2.8vw, 44px); top clamp(44px, 9vh, 96px); rounds separated by clamp(72px, 15vh, 160px); setup → answer clamp(14px, 2.2vw, 29px); answer → address clamp(16px, 2.2vw, 26px).
- The prim voice sits on a centre axis; answers break the axis from the left margin to nearly the right margin.

## Colour
- Canvas `#f5e5e1`.
- Primary — answers `#cc2418` — ≈ 75% of ink — 4.5 : 1 (display sizes only).
- Secondary — setup sentences and handle `#5a3651` — ≈ 18% — 8.3 : 1.
- Tertiary — addresses (joviangame.me, the Cards Against The Humanity address, ARC Prize 2026) `#7a5468` — ≈ 7% — 5.2 : 1.

## Signature
A small, centred, courteous line immediately followed by a blunt lowercase answer filling the width.

## Invariants
Two voices only. The answer always follows its setup. Answers lowercase, extended, black, flush left, near full measure. The prim voice always small and centred.

**Allowed variation:** which prim lines are italic or small caps; round spacing.
**Prohibited normalization:** title-casing or centring answers, shrinking answers to heading size, raising the prim voice to the answers' scale, a third family, using the answer colour for small text.

## Assumptions and risks
- Lowercasing renders "ARC-AGI-3" as "arc-agi-3"; confirm the owner accepts it.
- The premise comes from the owner's README, not from the official brand; it must not drift toward the official black-and-white card identity.
- The answer colour passes contrast only at display size.

## Round 2 translation
The names are the links and land as answers; each project page opens with its setup line. Interface text belongs to the prim voice; the answer voice never appears below display size.
