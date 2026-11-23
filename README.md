# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/ishiemon/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/ishiemon/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4,033 bytes of Python. It plays the make.fun gauntlet through the env at MAKEFUN_ENV_URL: a 0x88 board with incremental material and piece-square scoring and a Zobrist transposition table, searched with iterative deepening under a fixed 50,000-node budget — alpha-beta with principal-variation search, null-move pruning, late-move reductions, check extensions, killer moves and a capture quiescence search. No clock and no randomness in the search, so the same position always gets the same move.

## Run it

```sh
MAKEFUN_ENV_URL=<env url> python3 main.py
```

The engine is `main.py` alone (Python 3.13, standard library only). It asks the env for the game in play, sends its moves in UCI, and exits when every game is over.

---
<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
