# Generation prompt template

Fill the bracketed fields and remove unused alternatives. Keep every locked requirement.

```text
Use case: stylized-concept
Asset type: transparent 3D product icon for Chrome
Colour mode: [STANDARD or EMPTY STATE]

Primary request:
Create one isolated 3D icon representing [SUBJECT AND INTENDED MEANING].
[PRIMARY OBJECT AND UP TO TWO TIGHTLY RELATED SUPPORTING COMPONENTS].

Input images:
- User image, when present: subject/content reference only. Preserve identity,
  recognisable silhouette, functional components, and meaning; do not inherit style.
- Approved Chrome icons: canonical style references. Match their shared geometry,
  materials, colour hierarchy, camera, lighting, and rendering character.

Style and geometry:
Premium, mature Chrome product illustration for a stock-broking experience.
Use a compact readable silhouette, restrained bevels, moderate rounding, and clean
construction. Avoid gamified, inflated, candy-like, toy-like, and children’s-app styling.

Materials:
[SUBJECT-APPROPRIATE MATERIALS]. Use broad controlled highlights, realistic material
separation, and restrained texture. Render metal as crisp, hard, and reflective with
controlled edge highlights, never soft or plastic. Render every currency note or paper
element as a thin flexible sheet with minimal edge thickness; build stacks only from
plausible individually thin sheets. Never create thick tiles, padded cards, or slabs.

Colour:
[STANDARD: Use warm white, silver, grey, and signature royal/electric blue. Add
SEMANTIC COLOUR only to COMPONENT because REASON; otherwise add no accent colours.]
[EMPTY STATE: Use warm white, silver, and neutral grey only. No blue and no semantic
or decorative accent colours. Communicate through form, pose, depth, and value.]

Camera and composition:
Use a soft front three-quarter product view with slight elevation and mild long-lens
perspective. Keep [MEANING-BEARING FACE OR COMPONENT] clearly visible. Optically centre
one object or tightly related group at roughly 60–75% of a square canvas with generous
transparent padding. Avoid top-down isometric and wide-angle views.

Lighting:
Use bright diffused upper-left/front studio illumination, gentle fill, clean midtones,
subtle ambient occlusion, broad highlights, and controlled specular edges.

Output:
Return an RGBA PNG with true transparency and transparent corners. Retain exactly one
soft neutral-grey semi-transparent grounding shadow beneath the object as partial alpha.
Do not bake in white, black, checkerboard, gradient, card, or environment backgrounds.

Avoid:
Text, logos, clutter, extra finance motifs, unrelated objects, hard shadows, dramatic
lighting, noisy texture, excessive mechanical detail, glossy plastic everywhere,
unapproved colours, thick paper, and soft plastic-looking metal.
```

## Targeted edit

```text
Edit only [REQUESTED CHANGE]. Preserve the subject, silhouette, camera, materials,
colour mode, lighting, composition, transparent background, and grounding shadow unless
explicitly changed. Do not add new objects, labels, or colours.
```
