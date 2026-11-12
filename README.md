# Leta and Mnema

A browser-based 3D horror adventure in the style of PlayStation-era survival horror: fixed camera angles, tank controls, low-poly characters, a 320x240 picture with dithering and VHS grain.

The whole game is one file, [`index.html`](index.html). Three.js is loaded from a CDN; every model and texture is generated in code, so there are no asset files.

## Run

Open `index.html` in a browser, or serve the folder (`python3 -m http.server`) and open it on a phone. An internet connection is needed for Three.js and the UI font.

## Controls

| | Keyboard | Touch |
|---|---|---|
| Move | Arrows / WASD | Left stick |
| Run | Shift | RUN |
| Examine / confirm | E, Enter, Space | ACT, or tap the text box |
| Pause / back | Esc | II |

Tank controls are the default (up/down walk, left/right turn). Settings switches to modern, camera-relative controls and can turn the pixelation off. Progress is saved at the cassette recorder in the bus shelter and restored with Continue.

## Adding content

`index.html` is split into numbered, commented sections. The two extension points are:

- `registerScene(id, def)` - a location: geometry, fixed camera zones, walkable area, colliders, interactables and triggers.
- `registerChapter(id, def)` - which scene a chapter starts in and its opening script.

`createCharacter('mnema')` and `Game.spawnNPC('mnema', x, z, rot, { lines })` are ready for Chapter 1; Mnema is not placed anywhere yet.
