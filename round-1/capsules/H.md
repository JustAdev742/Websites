# H — concept capsule

## Premise
The site exists to send visitors somewhere else ("a website for my other websites"). The page is set as a departure: every line leans forward in a cursive italic, whose exit strokes lead rightward, and gathers at the right edge. The left of the page, where reading starts, stays empty.

## Type
- **Brygada 1918 Italic** — Mateusz Machalski, Borys Kosmynka and Przemysław Hoffer. Primary source: github.com/kosmynkab/Brygada-1918. SIL OFL 1.1, no Reserved Font Name. Embedded subset: italic, wght 400–600. Fallback: generic serif italic only.
- Italic only. Old-style figures. Case as written.
- Names wght 600; addresses wght 500; handle and sentences wght 400 (handle tracking 0.015em).

## Scale, line and space
- Names clamp(33.6px, 1.15rem + 3.9vw, 86.4px), line-height 1.02, balanced lines.
- Small text clamp(16px, 0.94rem + 0.3vw, 20px), line-height 1.42.
- One right-aligned column, ≤ 44rem wide, pushed to the right margin clamp(20px, 4.2vw, 76px); left margin clamp(20px, 6vw, 96px) plus the unused width. Top clamp(24px, 6vh, 72px); bottom clamp(40px, 10vh, 96px).
- Sections separated by clamp(52px, 11vh, 120px); name → sentence 0.75rem; sentence → address 0.15rem.
- Final full stops hang past the right edge by their own width (0.191em) so the letters align flush.

## Colour
- Canvas `#0e3a3f`.
- Primary — destinations (names and addresses) `#ffb39b` — ≈ 70% of ink — 7.2 : 1.
- Secondary — handle, sentences, ARC Prize 2026 `#b5d3ce` — ≈ 30% — 7.8 : 1.

## Signature
Everything leans and gathers on one right edge; the full stops hang beyond it.

## Invariants
Italic only; flush right; an empty left field; destinations in the primary colour; hanging final punctuation.

**Allowed variation:** column width; section spacing.
**Prohibited normalization:** switching to roman; left or centred alignment; filling the left field.

## Assumptions and risks
- Right-aligned multi-line text is slower to read; keep lines short.
- Italic small text must stay at 16px or larger.

## Round 2 translation
Destinations are the links. Any navigation also sits on the right edge, and nothing is placed in the left field.
