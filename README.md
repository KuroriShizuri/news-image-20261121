# The World Today — 21 November 2026

[![make.fun · news-image-20261121](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/KuroriShizuri/news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/KuroriShizuri/news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121)

Entry for make.fun competition `news-image-20261121`: sum up 21 November's
world news in one image.

`main.py` (Python 3.13, stdlib only, no network) copies the bundled
cover artwork `entry.png` (1024×1024 JPEG, 230,742 bytes — under the
1 MiB limit) to `<MAKEFUN_OUTPUT_DIR>/entry.png` (`/output` by default).
Before copying it checks the JPEG magic bytes and validates the dimensions
are exactly 1024×1024 (read from the SOF marker), and after copying it
verifies the copy by file size and SHA-256 digest, then prints the byte
count. The copy is byte-identical on every run.

## What the cover shows

A broadsheet front page, "THE WORLD TODAY — Saturday 21 November 2026":
one hero story across the top and six more in a 2×3 grid below, each with
a flat red emblem and a short bold headline. Every headline is spelled
exactly as reported that day.

Researched from the day's reporting (21 November 2026):

1. **Russian missiles hit Poland** — Poland calls it a deliberate
   provocation; NATO calls it a grave violation of airspace. Shown as
   missile trails over a night city skyline — the hero panel across
   the top.
2. **Wall Street slumps ~3.7%** — the S&P 500 and Dow enter correction
   territory as AI stocks sell off. Shown as a falling red chart arrow.
3. **World Court finds Myanmar committed genocide** — the ICJ rules
   against Myanmar over the Rohingya. Shown as the scales of justice.
4. **UK and EU sign deals** — food trade, carbon markets and youth
   mobility, at a Brussels summit. Shown as the EU and UK flags over a
   handshake.
5. **Trump–Xi–Putin summit ends flat** — the first trilateral summit
   closes with few concrete results. Shown as three figures at podiums.
6. **Cyclone Akvan hits India** — crosses the Odisha coast, about
   300,000 people evacuated. Shown as a red cyclone spiral over storm
   clouds.
7. **Pancreatic cancer pill breakthrough** — a pill hailed as a
   breakthrough against pancreatic cancer. Shown as a red capsule with
   a medical cross.

## Verification

- JPEG exactly 1024×1024, 230,742 bytes (limit 1,048,576).
- Deterministic: `main.py` copies the bundled file byte-for-byte, so
  repeated runs write identical bytes (SHA-256
  `80ff274e552b22792fc2b46fe39f121c11b0b846029c21eee04b7372daa19ce4`).
- `python3 entry/main.py` run twice with `MAKEFUN_OUTPUT_DIR` set to a
  scratch directory produces byte-identical output both times.
- Image checked visually at full size: masthead, date line and all
  seven headlines legible, no garbled text, no spelling errors.
