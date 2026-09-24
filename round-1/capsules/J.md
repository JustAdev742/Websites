# J — concept capsule

## Premise
ARC-AGI-3 agents are scored on how few actions they need compared with people, and the owner's planner searches for the shortest path to a goal. The page is a planned route from the start (the handle) to the goal (ARC-AGI-3, the game still being solved): each block sits exactly one fixed step right of the previous one and one row down, with no wasted moves.

## Type
- **League Spartan** — The League of Moveable Type. Primary source: github.com/theleagueof/league-spartan. SIL OFL 1.1, no Reserved Font Name. Embedded subset: wght 400–700. Fallback: generic sans-serif only.
- Names wght 700, tracking −0.012em, balanced lines; supporting lines wght 400. Case as written.

## Scale, line and space
- Names clamp(28px, 1rem + 3.3vw, 68px), line-height 1.02, measure 13em — every name the same size, because every move costs the same.
- Supporting lines clamp(16px, 0.94rem + 0.25vw, 19px), line-height 1.4, measure 28em.
- Step = clamp(24px, 10vw, 152px); block n is indented n steps. Vertical gap between blocks clamp(24px, 4.5vh, 52px). Page sides clamp(16px, 4vw, 64px); top clamp(24px, 6vh, 72px); bottom clamp(48px, 12vh, 112px).

## Colour
- Canvas `#dcd2f0`.
- Secondary — the path (start and intermediate steps) `#2d2358` — ≈ 70% of ink — 9.7 : 1.
- Primary — the goal block `#0b6638` — ≈ 30% — 4.9 : 1.

## Signature
A staircase of equal moves that ends at a goal in a different colour.

## Invariants
A fixed step unit; always right and down; equal name sizes; the goal colour only on the goal.

**Allowed variation:** step size; order of the intermediate steps.
**Prohibited normalization:** aligning blocks to one edge; varying name sizes; colouring intermediate steps.

## Assumptions and risks
- On narrow phones the step shrinks to 24px and the path becomes subtle.
- "Goal = ARC-AGI-3" is an interpretation (the current, unfinished work) that the owner may not share.

## Round 2 translation
Navigation behaves as moves along the route; the current page takes the goal colour; the path to it is the trail back.
