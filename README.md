# Medea — three versions side by side

A phone-first reader for comparing **three versions of Ljubomir Đurković's _Medea_**:

1. **Your English translation** (the reading translation from the website)
2. **Paula Gordon's English translation** (Reading Version 6, 2014–2016, © Paula Gordon)
3. **The Montenegrin original** (_Medeja_, © 2013 Ljubomir Đurković)

The three texts are shown as **stacked, scene-synced panes**. Pick a scene at the top
and all three jump to it; tap a pane's title bar to expand it for focused reading, tap
again to share the view three ways. On wide screens (tablet / desktop / landscape) the
panes become three side-by-side columns automatically.

## Why scene-by-scene (not line-by-line)

The two English translations render Đurković's central device differently. In the
original — and in your translation — **Medea's lines are spoken without her name**, her
voice running unattributed through the others' speech (set off here by a faint margin
rule). Paula Gordon instead **labels them MEDEA**. Because of this the versions don't
align word-for-word, so they're kept in step by **scene**, the one structure all three
share.

## Features

- Stacked synced panes on phones; three columns on wide screens
- Scene picker + ‹ › navigation (arrow keys on desktop)
- Tap a pane title to expand/focus it; show/hide any pane
- Light / dark theme, adjustable text size
- "Align the other panes" — tap any line to scroll the other two to the matching spot
- Installable (Add to Home Screen) and works offline (PWA)

## Running locally

It's a static site. From this folder:

```
python3 -m http.server 8000
```

then open <http://localhost:8000/>. Add `?read` to the URL to skip the intro.

## Deploying

Any static host works (GitHub Pages, Netlify, etc.). For GitHub Pages, push this
folder to a repo and enable Pages on the branch root — `.nojekyll` is already included.

## Source

All text is bundled inside `index.html` (in the `#DATA` script block), so the site is
fully self-contained and offline-capable. The English/Montenegrin/Russian parallel data
was taken from the existing _Sabrane drame_ reader; Paula Gordon's English was extracted
from her reading-version PDF.
