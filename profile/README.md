# LowArc

Tools for making games, built to be taken a piece at a time. Two JavaScript engines, one to draw and
one to simulate, are released; a modular game engine and the IDE around it are on the way.

## Winding

A WebGPU rendering engine for the browser. No dependencies, no build step: ES modules, imported as
they are. glTF models with their materials, skins and animations; clustered lights and cascaded
shadows; culling on the GPU; Gaussian splats; and a 2D renderer of sprites, text and tilemaps
beside the 3D one.

[Repository](https://github.com/getlowarc/winding) · [Live demo](https://getlowarc.github.io/winding/demo/) ·
[npm](https://www.npmjs.com/package/winding-engine) · MIT

## Bearing

A physics engine in plain JavaScript, for any renderer, in 3D and in 2D. No dependencies, no build
step, and no WebAssembly: rigid bodies, joints, a character body and raycasts, with the same results
to the bit on every machine. It draws nothing, so Winding, Three.js, Babylon.js, PlayCanvas and Pixi
all read it the same way.

[Repository](https://github.com/getlowarc/bearing) · [npm](https://www.npmjs.com/package/bearing-physics) · MIT

Winding and Bearing are built to work together and need nothing from each other: use either alone.

## LowArc and LowArc Studio

Most game engines are all or nothing. Adopting one means taking its language, its editor, its
project format and its way of thinking together, and wanting one piece means taking all of them.
LowArc is assembled instead of adopted: you choose the modules you want — a drawing surface, audio,
input, whatever else — and those modules are the framework your code is written against. It has no
language of its own and no project format.

[LowArc Studio](https://github.com/getlowarc/lowarc-studio) is the IDE for it, where a project's
modules are put together, its code is edited and a dev build is run and debugged. Apache-2.0.

Early, and honest about it: Studio runs from source on Windows, and nothing is released to download
yet. Releases will live at [lowarc.com](https://lowarc.com) once there is something worth
downloading.
