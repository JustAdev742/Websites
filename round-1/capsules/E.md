# E — concept capsule

## Premise
The handle "JustAdev742" reads "just a dev". The work it signs is a party game and an agent for an AI benchmark. The page makes the author the smallest text on the page and the work the largest: the names as a tower of single huge words, the handle as a 12px line at the end.

## Type
- **Recursive** — Stephen Nixon / Arrow Type. Primary source: github.com/arrowtype/recursive. SIL OFL 1.1, no Reserved Font Name. Embedded subset: MONO 0–1, CASL 0–1, wght 400–1000; slnt and CRSV pinned at 0. Fallback: generic sans-serif only.
- Three voices of one family:
  - **Names:** MONO 0, CASL 1, wght 1000 (casual, heaviest), tracking −0.012em.
  - **Sentences:** MONO 0, CASL 0, wght 450 (linear).
  - **Developer strings** (handle, addresses): MONO 1, CASL 0, wght 450 (monospaced).
- Case as written.

## Scale, line and space
- Names = content width ÷ 5.3 (so "ARC-AGI-3" nearly fills the width), max 240px; one word per line, no wrapping inside a word; line-height 0.95 (keeps the g of "Against" clear of the h of "The").
- Sentences clamp(15px, 0.88rem + 0.28vw, 18px), line-height 1.4, measure 24em. Address under Cards Against The Humanity 13px. Footer handle and domain 12px — the smallest text.
- Flush left, ragged right. Side margins clamp(16px, 3.2vw, 52px). Name → sentence clamp(16px, 2.2vw, 26px); between works clamp(48px, 9vw, 120px); footer right-aligned after clamp(72px, 14vw, 176px). At desktop the tower is taller than one screen.

## Colour
- Canvas `#ef4b1f`.
- Primary — names `#fff1db` — ≈ 85% of ink — 3.3 : 1 (display sizes only).
- Secondary — sentences `#1c0a05` — ≈ 10% — 5.2 : 1.
- Tertiary — developer strings `#0a1543` — ≈ 5% — 4.7 : 1.

## Signature
A tower of enormous casual words, signed at the bottom right by a 12px monospaced handle.

## Invariants
The handle is the smallest text on every page. Names one word per line at maximum width. Monospace only for the handle and addresses.

**Allowed variation:** tower height; placement of sentences.
**Prohibited normalization:** enlarging the handle into a header or logo; setting names in the linear or mono voice; using the name colour for small text.

## Assumptions and risks
- The name colour passes contrast only at display size.
- Pages are tall; "The" takes its own line as part of the name.

## Round 2 translation
Navigation and headers stay small and monospaced; project names are the large links; the footer signature is the only identity mark.
