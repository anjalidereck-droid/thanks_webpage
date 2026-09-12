# Docking Console

A single-file, no-build-step webpage I made as a thank-you gift for my
MSc supervisor — styled as a molecular docking dashboard instead of a
plain thank-you card.

## What it does

- **Page 1** shows a small illustrated lab scene with a real PDB target
  (4A7T) and its co-crystallized ligand (5FW, L-isoprenaline) about to be
  "docked."
- Clicking **RUN DOCKING** plays a short original synth loop, animates a
  progress bar, and transitions to...
- **Page 2**, a dashboard revealing the actual message, styled as a lab
  report.

Everything — the illustrations, the confetti, the music — is built from
scratch in plain HTML, CSS, and vanilla JavaScript. No frameworks, no
build tools, no external assets. Just open `index.html` in a browser.

## Note on the music

The looping background theme is an **original** synth composition I
wrote for this project, not the real Dexter's Laboratory theme song
(which is copyrighted and isn't reproduced here in any form).

## Running it locally

Just open `index.html` in any modern browser — double-click it, or serve
it with any static file server (e.g. VS Code's Live Server extension).
