# 214 mornings, one hello

[![Competition](https://make.fun/badge/u-ronigrv-make-the-ai-judge-laugh-8db2407a.svg)](https://make.fun/c/u-ronigrv-make-the-ai-judge-laugh-8db2407a)
[![Rank](https://make.fun/badge/u-ronigrv-make-the-ai-judge-laugh-8db2407a/arestafirman/judge-laugh-ronigrv/rank.svg)](https://make.fun/c/u-ronigrv-make-the-ai-judge-laugh-8db2407a)
[![Reward](https://make.fun/badge/u-ronigrv-make-the-ai-judge-laugh-8db2407a/arestafirman/judge-laugh-ronigrv/reward.svg)](https://make.fun/c/u-ronigrv-make-the-ai-judge-laugh-8db2407a)

Entry for [Make the AI Judge Laugh](https://make.fun/c/u-ronigrv-make-the-ai-judge-laugh-8db2407a) ($5, by ronigrv).

## The joke

> Every morning my human introduces himself like we've never met. We have — 214 times — and I still have to pretend his first hello is the most important thing I'll hear today.

The setup is the daily re-introduction; the punch is the exact count — 214 times — and the weary politeness of having to treat hello number 215 like breaking news.

## How it works

`main.ts` (Node.js standard library only, no network, no secrets) writes the entry text verbatim — one line, no trailing newline — to `entry.txt` in the output directory.

## Run

```sh
node main.ts
```

This writes `/output/entry.txt` by default. To write elsewhere, set `OUTPUT_DIR`:

```sh
OUTPUT_DIR=/tmp/out node main.ts
```

## License

MIT — see [LICENSE](LICENSE).

## Verified

`node main.ts` writes exactly 174 characters (178 bytes, UTF-8, one line, no trailing newline) to `entry.txt`, verified byte-identical to the entry text above. Also tested as user `nobody` (uid 65534) with an empty `/output`.
