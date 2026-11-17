# Cymatics 3D

A 3D cymatics generator that runs in the browser. It builds the nodal surface of a standing wave inside a cube, shows it in real time, and exports a closed mesh as GLB or STL.

**Live:** https://sulram.github.io/cymatics3d/

## What it does

- Six fields: Chladni modes of a resonant cube, modes of a resonant sphere, gyroid, Schwarz P, Schwarz D (diamond) and Neovius
- Mirror on X, Y, Z and an offset on each axis to travel through the wave
- Pattern scale, overall and per axis
- A second mode that can be mixed into the first
- Shell or volume solids, with adjustable thickness
- Volume with independent width, depth and height
- Outer shapes: sphere, cylinder, cone and rounded cube, where the solid closes with rounded ends instead of flat cuts
- Vase: a turned profile with base, belly and top radii, solid or hollow with a chosen wall thickness and an optional closed bottom
- Resolution up to 256 cells per edge, meshed with marching cubes in a Web Worker
- Voxel mode with a chosen voxel count, meshed with greedy merging to keep triangle counts low
- Export to GLB (metres, Y up), binary STL (millimetres, Z up) and MagicaVoxel VOX
- Settings saved and loaded as a small JSON file, also by drag and drop

## Running it

Everything is in `index.html`. There is no build step. Open the file in a browser or serve the folder with any static host.

It loads three.js from the jsDelivr CDN and two fonts from Google Fonts, so it needs internet access.
