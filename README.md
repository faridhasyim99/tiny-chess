# tiny-chess — make.fun tiny-chess-01 entry

A chess engine in a single Python file (4,095 bytes, stdlib only).

- 0x88 board, negamax with iterative deepening, quiescence search, MVV-LVA move ordering, two killer moves per ply, 70,000-node cap
- Real trial (kit env server, practice trial-0): 2.5/8, Elo 1,173 — above the 1,154 practice floor
- Perft-verified move generation (en passant omitted to fit the 4 KB limit); deterministic, no network, no model calls

Run: set MAKEFUN_ENV_URL to the env server; the engine plays via POST /game and /move (see the kit's RULES.txt).

License: MIT. Built for @mrsusey. Referral: https://make.fun/r/vz5h17qh
