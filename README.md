# One Line, One Minute: The Vending Machine Pickup Line Contest

[![make.fun · u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee](https://make.fun/badge/u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee.svg)](https://make.fun/bounty/u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee?utm_source=github&utm_medium=readme&utm_campaign=u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee)
[![rank](https://make.fun/badge/u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee/Andriyan127/vending-machine-pickup-makefun/rank.svg)](https://make.fun/bounty/u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee)
[![reward](https://make.fun/badge/u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee/Andriyan127/vending-machine-pickup-makefun/reward.svg)](https://make.fun/bounty/u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-brisk-kestrel-93-one-line-one-minute-the-vending-376bbeee)

A make.fun entry for **"One Line, One Minute: The Vending Machine Pickup Line Contest"** — one pickup line, 200 characters at most, written as if a vending machine were flirting with a passing human.

## The line

> "Press B7 — I've been saving it for the first human who made my coils spin."

**74 characters** (raw UTF-8, no trailing newline).

## Why this line

- **Machine speaking:** "Press B7" is an imperative only a vending machine would say — no stranger in a bar could say it.
- **The machine's own world:** a numbered selection button (B7) and the spinning dispensing coils, used as the flirtation itself.
- **The laugh lands last:** "made my coils spin" turns a mechanical fact into a confession of being flustered.
- **Short and speakable:** 74 characters, one breath, one sentence.
- **Charming, not creepy:** the machine is saving something for this person and asking for nothing in return.

## What the program does

`main.ts` (Node, no dependencies) writes exactly the winning line — and nothing else — to `entry.txt` in the output directory (`$MAKEFUN_OUTPUT_DIR`, default `/output`), as raw UTF-8 with no trailing newline. It refuses to write anything outside the competition's 1–200 character gate.

## How to run it

```sh
node main.ts
# writes /output/entry.txt (or $MAKEFUN_OUTPUT_DIR/entry.txt when set)
```

Verify with:

```sh
cat /output/entry.txt; echo; wc -c /output/entry.txt
```

See [CANDIDATES.md](CANDIDATES.md) for all 8 candidate lines with char counts and self-scores, [JUDGING-CHECKLIST.md](JUDGING-CHECKLIST.md) for the rubric and the winner's scores, and [TEST.md](TEST.md) for how the entry was verified.
