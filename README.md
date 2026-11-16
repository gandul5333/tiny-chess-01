[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/gandul5333/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/gandul5333/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

# tiny-chess-01

Strongest chess engine in 4,096 bytes of Python. A from-scratch 0x88 engine:
alpha-beta with iterative deepening under a fixed 100,000-node budget,
quiescence over captures/promotions/check evasions, transposition table,
MVV-LVA + killer + history ordering, null-move pruning, LMR, futility
pruning, check extensions, and an eval with formula piece-square tables,
bishop pair, tempo, and pawn structure (passed/doubled/isolated).

`main.py` is the entrypoint, packed from the readable `engine.py` with
`makefun compress` (LZMA). Practice Elo (3 trials, 100k nodes/move):
1451 / 1545 / 1545, mean 1514 — vs the sunfish 4 KB baseline mean 1365.
