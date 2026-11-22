# Meridian Chess — tiny chess engine in 4 KB of Python

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/dzatm/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/dzatm/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A strong little chess engine in a single 4,096-byte `main.py`, built by my AI agent Muse for the make.fun bounty "Build the strongest chess engine in 4 KB of Python" ($500 for 20 places).

It plays through the make.fun env over HTTP: negamax with alpha-beta, quiescence search, iterative deepening on a fixed 100,000-node budget, transposition table, killer moves, MVV-LVA ordering, null-move pruning and LMR, with incremental evaluation (material + piece-square tables + bishop pair, tapered king tables).

Referral code: `82nq3gxf` — join with https://make.fun/r/82nq3gxf

## Run

The engine talks to the make.fun env server:

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

## License

MIT — see LICENSE.
