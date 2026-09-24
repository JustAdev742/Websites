# Evidence capsule — Round 1

Withheld from the first visual encounter. Shared by all ten directions.

## Subject
A hub website for **JustAdev742** (GitHub handle) that links the owner's Cards Against The Humanity site, names their game engine (Jovian Engine), and shows their ARC-AGI-3 work on Kaggle. The brief asks for the site to "link exactly joviangame.me" and to be "the best you can".

## Facts used (functional research, text only)
- **Cards Against The Humanity** — repo `JustAdev742/cards-against-the-humanity`. README: "Cards Against Humanity for a living room. Put the TV on the big screen, everyone else joins from their phone." Page description: "Play Cards Against Humanity in your living room. The TV is the table, phones are the hands." Played at `https://joviangame.me/cards-against-the-humanity/`. No game server (WebRTC peer to peer, four-letter room codes); the Card Czar turns answers over one at a time and "each card writes itself into the black card on the TV as it is read out, so the whole room is reading the same joke at the same time"; the address bar "only ever carries the table code, because that is the one thing worth scanning or sharing". Bot scoring rules written by the owner: "Register clash. A prim setup with an indecent answer"; "How much of a picture it paints … physical words, names, numbers, bodily words, adjectives you could see". Unofficial, non-commercial fan implementation; card text CC BY-NC-SA 2.0 from Cards Against Humanity LLC.
- **joviangame.me** — custom domain (CNAME) of `JustAdev742/JustAdev742.github.io`; its root currently serves only a README. Project sites are served beneath it.
- **Jovian Engine** — the owner's game engine. The owner asked: "please don't do the Jovian engine website". Name only: no link, none of its website's text, figures or claims. (Its page text was read once for facts before that instruction; nothing from it is used.)
- **ARC-AGI-3** — repo `JustAdev742/Arc-Agi-3-Kaggle-comp`, "ARC Prize 2026 – ARC-AGI-3 agent", Kaggle competition `kaggle.com/competitions/arc-prize-2026-arc-agi-3`. One local model drives a persistent Python REPL that holds the game state, writes and verifies a per-game world model, plans against it and sends actions. Perception: "exact grid perception: components, diffs, scale detection"; entity roles "static/hud/avatar"; shortest-path planning; scored on action efficiency relative to humans. Research discipline: hypothesis, fixed evaluation, keep or revert; research log "one entry per change, newest at the bottom".
- **Last push dates (GitHub, UTC)** — J.O.V.I.A.N.Game 2026-03-27; Project-Jovian 2026-08-15; cards-against-the-humanity 2026-09-20; Arc-Agi-3-Kaggle-comp 2026-09-24 00:04; Websites 2026-09-24 07:02.
- **Handle** — "JustAdev742" reads "Just a dev" + 742.

## Working copy (provisional, identical in A–J)
1. JustAdev742
2. joviangame.me
3. Cards Against The Humanity
4. The TV is the table, phones are the hands.
5. joviangame.me/cards-against-the-humanity
6. Jovian Engine
7. My game engine.
8. ARC-AGI-3
9. Developing AI stuff on Kaggle.
10. ARC Prize 2026

Lines 4 and 5 are the owner's own copy and URL. Line 7 and line 9 paraphrase the brief ("my game engine", "developing ai stuff in kaggle arc-agi-3"). Line 10 is the competition's name. Nothing else is invented; no real name is used.

## Tensions worth keeping
- "Just a dev" versus a game engine and an AGI benchmark.
- A rude party game and careful research on the same page.
- A hub whose best evidence argues against hubs ("There is no server keeping a directory").

## Source boundary
- **Allowed:** the owner's repositories (README text, file structure, dates), the brief, the domain setup, the benchmark's published mechanics.
- **Prohibited:** other designers, galleries, portfolio sites, templates, UI kits, design tokens, icon libraries, Google Fonts or other platform house styles as input, the Jovian Engine website, the official Cards Against Humanity visual identity, AI-generated imagery.
- **Fonts:** chosen from written requirements; open-source, taken from each foundry's own repository; licences in `../licenses/`.

## Boundaries
- No claims about users, uptime, compliance or scale.
- Text contrast ≥ 4.5:1 for small text, ≥ 3:1 for display text only.
- No imitation of the official Cards Against Humanity black-and-white card identity.
