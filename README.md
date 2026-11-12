# What the Fog Kept

A story-driven, low-poly (PS1-style) third-person adventure in a single HTML file.
Ronnet, who has felt nothing since childhood, walks through the abandoned city of
Calder's Rest to her father's grave. On the way she meets Amy, who says she is lost.

## Play

Open `index.html` in a desktop browser (Chrome, Edge, Firefox). An internet
connection is needed to load Three.js from a CDN. Everything else — models,
textures, music and sound — is generated in code.

| Key | Action |
| --- | --- |
| W A S D | Move |
| Shift | Run (loud) |
| C | Sneak (quiet) |
| E | Interact |
| F | Ask Amy to wait / follow |
| Mouse drag, arrow keys, wheel | Look around, zoom |
| Space / Enter / click | Advance dialogue; 1–3 or ↑↓ pick a choice |
| Esc | Pause |

Progress is saved at the start of each chapter (browser local storage).

## Chapters

1. **The Last Stop** — the rainy night city.
2. **Vesper Park** — the Listeners, who hear rather than see.
3. **Saint Orrin Primary** — the Smilers, who move only when unseen.
4. **Calder's Rest Central** — the Commuters, and the tram out.
5. **The Outskirts** — grey fog, the old house, the Keeper.
6. **Where It Stopped Hurting** — the grave, the truth, and one choice with two endings.

## Development notes

The whole game lives in `index.html`. Appending `?chapter=<id>` to the URL
(`city`, `park`, `school`, `station`, `outskirts`, `cemetery`) starts directly in
that chapter, which is handy for testing.
