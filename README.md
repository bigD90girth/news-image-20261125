# The world in one day: Wednesday 25 November 2026

[![make.fun](https://make.fun/badge/news-image-20261125.svg)](https://make.fun/bounty/news-image-20261125?ref=kk8gvjx9)
[![rank](https://make.fun/badge/news-image-20261125/bigD90girth/news-image-20261125/rank.svg)](https://make.fun/bounty/news-image-20261125?ref=kk8gvjx9)
[![reward](https://make.fun/badge/news-image-20261125/bigD90girth/news-image-20261125/reward.svg)](https://make.fun/bounty/news-image-20261125?ref=kk8gvjx9)

A one-page newspaper front that sums up Wednesday 25 November 2026:
47 dated stories across seven regions, each with a headline, one detail
line and a UTC time — plus a hand-drawn world map with the day's ten
biggest stories marked, and twelve small drawn vignettes beside the
stories they belong to.

The hero is Wall Street's wild Wednesday: the Dow erased a 1,100-point
intraday loss to close up 0.33% at 50,183, while hot PCE data and a
4.3% GDP revision rattled the tape ahead of Thanksgiving.

Beyond the markets, the page carries the day's other consequential
stories: Shenzhou-24 docking with the first foreign astronaut aboard
Tiangong, a proposed 20–40% tariff on 14 trading partners, the EU
approving its 2027 budget and €45bn of Ukraine aid, a garment wage
rise of 36% in Bangladesh, and a record 2,100 migrants reaching the
Canary Islands in a single day.

## How it is built

`render.py` (build-time only, not part of the entry) draws the page
with Pillow at 1600px and downscales it to a 1024x1024 JPEG. The entry
itself is just that image plus `main.py`, a standard-library program
that copies it to `/output/entry.png`. Running the program twice
produces byte-identical output.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```
