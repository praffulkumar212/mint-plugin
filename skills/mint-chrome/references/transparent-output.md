# Transparent output verification

Deliver an RGBA PNG with:

- fully transparent empty canvas and transparent corners;
- clean antialiased object edges;
- exactly one subtle neutral-grey grounding shadow preserved as partial alpha;
- no black, white, checkerboard, gradient, environment, or card background baked into pixels.

Prefer native transparent output when the active image-generation path supports it. Otherwise use an approved background-extraction flow that preserves antialiased edges and the semi-transparent shadow. Do not remove the shadow simply to obtain transparency.

## Pre-delivery checklist

1. Confirm the saved file is PNG.
2. Confirm it has an alpha channel rather than only an RGB image with a transparency-looking background.
3. Confirm all four corners have zero alpha.
4. Confirm the object edge is clean at 100% zoom.
5. Confirm one grounding shadow remains neutral grey and partially transparent.
6. Confirm no opaque halo or matte surrounds the object or shadow.
7. Confirm the file is saved outside the plugin directory.

Do not claim transparency until these checks pass.
