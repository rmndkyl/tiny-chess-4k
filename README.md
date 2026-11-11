# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/rmndkyl/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/rmndkyl/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB Python chess engine: a 0x88 board with per-colour piece lists, alpha-beta
with a Zobrist transposition table, null-move pruning, late move reductions,
killer and history move ordering, quiescence with stand-pat, and a tapered
piece-square evaluation. The engine is stored as an lzma payload unpacked at
startup, so the whole thing fits in 4,096 bytes as committed.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8000 python main.py
```

It speaks the env protocol: `POST /game` for the game in play, then `POST /move`
with a UCI move until the env answers `done`.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
