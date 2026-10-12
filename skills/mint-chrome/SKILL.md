---
name: mint-chrome
description: Generate or restyle transparent PNG icons in the approved Chrome 3D illustration system. Use when a user invokes $mint-chrome, asks for a Chrome or Chrome-style 3D icon, attaches an object reference to recreate in the established style, describes a financial or product concept that should become a matching icon, or requests a neutral Chrome empty-state illustration.
---

# Mint Chrome

Create one polished 3D product icon using the bundled approved icons as the visual source of truth. Accept either an attached subject reference or a written description. Let the user control the subject and this skill control the style.

## Load the required resources

Read all four before generating:

- `references/art-direction.md` for locked visual variables and colour modes.
- `references/reference-catalog.md` to select the closest approved icons.
- `references/prompt-template.md` to construct the generation request.
- `references/transparent-output.md` to verify the deliverable.

## Follow the workflow

1. Determine the input mode:
   - **Reference mode:** use the attached image or supplied local image path as subject/content only.
   - **Description mode:** derive one clear subject from the user’s concept.
2. Determine the colour mode:
   - **Standard:** use the signature royal/electric blue and only conceptually necessary semantic accents.
   - **Empty state:** use warm white, silver, and neutral grey only; prohibit blue and every semantic accent.
3. Keep one primary object and at most two tightly related supporting components. Do not copy styling from an external subject reference.
4. Select 2–4 approved icons from `assets/references/` using `references/reference-catalog.md`. Choose references that jointly cover geometry, materials, camera, and permitted colour behavior.
5. Inspect the user reference, when present, and every selected approved reference before generation.
6. Fill `references/prompt-template.md`. Preserve the locked art direction; vary only the subject, subject-justified materials, pose, and permitted semantic colours.
7. Generate with the image-generation tool:
   - In reference mode, pass the user image and selected approved references. Label the user image as **subject/content reference** and bundled images as **style references**.
   - In description mode, pass the selected approved icons as **style references**.
8. Verify the result against `references/transparent-output.md` and its pre-delivery checklist.
9. Deliver one transparent PNG with the subtle semi-transparent grounding shadow retained.
10. For corrections, edit the generated image and preserve every property the user did not ask to change.

## Preserve or transform reference inputs

In reference mode, preserve subject identity, recognisable silhouette, functional components, and intended meaning. Transform geometry softness, proportions, material treatment, colour hierarchy, camera, lighting, composition, background, and shadow.

Do not reproduce branding, labels, photographic environments, or incidental styling from the subject reference unless explicitly requested.

## Resolve descriptions

Choose the simplest familiar metaphor that communicates the concept. Use no decorative finance motifs and no text unless a recognised symbol is essential.

Explicitly apply the thin-paper rule to currency notes and the crisp-metal rule to metallic hardware. Proceed without a question when one interpretation is reasonable; ask one concise question only when materially different interpretations would change the subject.

## Enforce the output contract

- Produce one isolated icon unless variants are requested.
- Default to a square canvas with generous transparent padding.
- Export as RGBA PNG with a real alpha channel and transparent corners.
- Retain exactly one soft neutral-grey semi-transparent grounding shadow.
- Never fake transparency with black, white, checkerboard, gradient, or a baked card.
- Save output in the user’s current workspace, outside this plugin directory, and report its path.

## Reject style drift

Do not introduce a new illustration style, inflated clay or candy styling, children’s-app character, heavy industrial construction, soft plastic-looking metal, thick card-like paper, UI cards, environments, unrelated focal objects, decorative semantic colours, or unrequested logos and labels.
