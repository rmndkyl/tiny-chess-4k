# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/rmndkyl/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard)
[![reward](https://make.fun/badge/tiny-chess-01/rmndkyl/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A 4 KB Python chess engine: 0x88 board, Zobrist transposition table, PVS with null move and late-move reductions, killers/history, quiescence, tapered evaluation, repetition-aware search with contempt.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8000 python3 main.py
```

It speaks the env protocol: `POST /game` for the position, then `POST /move` with a UCI move until the env answers `done`.

Bounty: https://make.fun/bounty/tiny-chess-01
