# Rotation & reflection playgrounds

Interactive tools for the geometric variant of the spatial-reasoning work: telling a
rotation ("same") from a reflection ("mirror") of a shape. The distinguishing signal
is the **chirality bit** (the sign of the transform's determinant: +1 rotation, -1
mirror), and the tools show how a *tight* grader sees it while a *distance-only* grader
is blind to it.

Useful when you want to *feel* why same/mirror is the clean probe, or to grab a framing
for the paper's figures.

## Files
- `index.html` - tabbed hub (SO(2) / SO(3)) with an "open full page" link.
- `so2.html` - planar (2D). Drag the basis-vector tips to build the transform; watch
  the determinant sign flip; toggle lens between pairwise distances (chirality-blind)
  and signed area (orientation-sensitive). Opens locked-rigid on a mirror.
- `so3.html` - 3D. Orbit the scene, rotate B with the sliders, toggle mirror (on by
  default); signed-volume lens is the 3D chirality bit.
- `patent_D949851.png` - the real US D949,851 figure (public domain), shown beside the
  stylized "patent part" stand-in.

## Run
Static. Open `index.html` in a browser, or visit the deployed page
(`/spatial-reasoning/playground/`). D3 loads from CDN; no build step.

## Note
The shapes are synthetic point sets (the domain-agnostic baseline), not patent figures.
Grounding the task in real rasterized figures is the raster-discrete follow-up
(`oracle-tightness/FOLLOWUP_RASTER_DISCRETE.md`).
