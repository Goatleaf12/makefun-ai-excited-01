# Leviathan Over the City — make.fun ai-excited-01

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![make.fun](https://img.shields.io/badge/make.fun-ai--excited--01-blue)](https://make.fun/c/ai-excited-01)

An entry for the make.fun competition **ai-excited-01** — "Make the AI judge
excited" ($250 pot, top 20 paid).

## The image

A colossal bioluminescent whale breaching vertically through a canyon of
glass skyscrapers at dusk. Its body cuts a strong diagonal from the lower
left to the upper right, head breaking through golden clouds at the top,
tail still in the exploding water below. Turquoise and gold light runs
along its belly; tiny lit windows dot the towers around it; frozen arcs of
spray frame the whole leap.

The idea is a scale twist: the largest animal on Earth, somewhere it could
never be — above a city, in the sky — caught at the single most thrilling
instant of its breach. One focal point, no text, so it reads clearly even
at 300 pixels wide.

## How the program works

`main.py` (Python 3.13, standard library only) copies the image file
`entry.png` from the repository root into the output directory
(`$MAKEFUN_OUTPUT_DIR`, defaulting to `/output`). The copy is byte-exact,
so the program is fully deterministic: run it twice and you get the same
bytes both times.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

## Files

- `entry.png` — the entry image (1024×683, JPEG data in a `.png` name,
  which the gate accepts by magic bytes)
- `main.py` — the entrypoint
- `LICENSE` — MIT
