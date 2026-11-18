# Deterministic 4 KB Chess Engine

A compact chess engine built for [make.fun's tiny-chess-01](https://make.fun/bounty/tiny-chess-01) bounty.

![make.fun badge](https://make.fun/badge/tiny-chess-01.svg)
[![rank](https://make.fun/badge/tiny-chess-01/ZiramBayam/makefun-tiny-chess-v2/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/ZiramBayam/makefun-tiny-chess-v2/reward.svg)](https://make.fun/bounty/tiny-chess-01)

`main.py` is the entire engine: Python 3.13 standard library only, under 4,096 bytes. It parses each FEN from scratch, searches a fixed node budget with alpha-beta, quiescence, a transposition table, killers and piece-square evaluation, and keeps no state between moves. No clock, no randomness, no external data — repeated runs play byte-identical games.

Move generation was verified against standard perft positions.
