# Test Report — Vending Machine Pickup Line

## What was verified

1. **Program runs cleanly** — `node main.ts` (Node v24.22.1, no dependencies) exits 0 and prints `Wrote 74 characters to /output/entry.txt`.
2. **Output is exactly the winning line** — `/output/entry.txt` contains byte-for-byte:
   `Press B7 — I've been saving it for the first human who made my coils spin.`
3. **Character gate (1–200)** — the line is **74 characters** (Python `len(decode('utf-8'))`), well inside the gate.
4. **No trailing newline** — file is 76 bytes; the em dash (—) is 3 UTF-8 bytes, so 74 chars = 76 bytes, confirming no extra bytes.
5. **`MAKEFUN_OUTPUT_DIR` respected** — running with `MAKEFUN_OUTPUT_DIR=/tmp/mf-test-out` wrote the identical file there (`/tmp/mf-test-out/entry.txt`, 76 bytes, exact match confirmed by Python comparison).
6. **Default output dir** — with the env var unset, the program writes to `/output/entry.txt` as required.

## Commands run (24 Nov 2026)

```sh
MAKEFUN_OUTPUT_DIR=/tmp/mf-test-out node main.ts
cat /tmp/mf-test-out/entry.txt
wc -c < /tmp/mf-test-out/entry.txt   # 76
node main.ts                          # default /output
wc -c < /output/entry.txt            # 76
```

All checks passed. The entry is valid for the gate (UTF-8 text, 1–200 characters, not only whitespace).
