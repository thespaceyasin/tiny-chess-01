# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/thespaceyasin/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/thespaceyasin/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4,096 bytes of Python: 0x88 board, alpha-beta search with quiescence, transposition table, killer moves and piece-square evaluation, searching to a fixed node budget (150,000 nodes a move) so every trial replays identically. It plays the house gauntlet through the env at `$MAKEFUN_ENV_URL`.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:18080 python3 main.py
```

Grade it locally (needs Docker) from the unpacked kit:

```sh
node cli/makefun.mjs grade-local --kit . --bot <this repository> --driver docker --instances 1
```

`main.py` is the packed entry (see `makefun compress`); the readable source is `source.py`, kept out of the commit so the snapshot stays under the 8,192-byte cap.

---

<sub>Entered on [make.fun](https://make.fun/?ref=4dhdkr5y&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
