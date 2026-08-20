---
name: scene-to-art-lab
description: Transform a user-supplied photograph into an original vertical 3:4 art-directed poster using watercolor, pop-art screenprint, expressive painting, ink-wash, relief print, editorial surrealism, or a controlled hybrid. Use when the user asks to reinterpret a real scene, portrait, object, vehicle, landscape, architecture, or travel photo as creative visual art, an exhibition poster, editorial poster, key visual, or unified poster series with source-specific typography, editorial micro-copy, image-title interlocking, and selected identity preservation.
---

# Scene to Art Lab

Turn a supplied photograph into a deliberately art-directed 3:4 poster rather than a styled photograph. Preserve only the scene features that carry identity, then redesign composition, color, mark, space, graphic structure, and material according to one coherent medium and one poster idea. Do not assume that the whole source image must remain visible or receive equal artistic treatment.

Use image generation for every requested transformation. A supplied image plus a request to transform it is sufficient consent; do not reconfirm. Inspect the image before editing when it is available as a local file.

## Core workflow

1. Read the source image.
2. Choose or infer one primary art mode.
3. Define a concise poster proposition: what the viewer should notice or feel first.
4. Select one poster layout system and redesign the composition for the selected medium and a 3:4 canvas.
5. Write a scene-specific transformation brief containing every mandatory output constraint.
6. Generate the image directly.
7. Inspect the result when possible; revise once if identity, poster hierarchy, layout, edge loss, or medium behavior failed.
8. Return the image with a short Chinese rationale. Provide the full generation prompt only when requested.

If the user names a mode, follow it. If not, infer the strongest match from the source and explain the choice briefly after generation. Ask a question only when two materially different interpretations are equally plausible and the choice cannot be inferred from the request or image.

## Read the source

Create a compact internal Source Map:

- **Identity anchors:** up to three features that must remain recognizable.
- **Spatial logic:** horizon, overlap, pose, perspective, direction, or scale relationship that organizes the scene.
- **Energy:** still, lyrical, graphic, tense, playful, monumental, intimate, or kinetic.
- **Shape hierarchy:** dominant silhouette, secondary masses, and expendable detail.
- **Color opportunity:** colors worth preserving, suppressing, exaggerating, or replacing.
- **Material opportunity:** edges, light, texture, rhythm, or empty space suited to an artistic medium.

Preserve identity through selected relationships, not through indiscriminate detail. For portraits, protect facial identity, expression, pose, and hand count. For products and vehicles, protect proportions, signature graphics, perspective, and enough of the silhouette to remain identifiable unless the user requests distortion. Permit non-defining contours, peripheral bodywork, background objects, and expendable detail to dissolve, crop out, merge into the ground, or remain unrendered. Never add logos, people, or objects that are absent unless requested or clearly necessary for the chosen concept. Poster typography is the one default addition governed by the typography system below.

## Mandatory output contract

Apply these requirements to every generation unless the user explicitly overrides a specific item:

- Generate a **3:4 vertical image**. State `vertical 3:4 aspect ratio` in the final generation prompt and compose for that canvas rather than merely resizing the source.
- Reconstruct the composition according to the chosen medium. Do not automatically preserve the source crop, framing, centering, background coverage, or distribution of detail.
- Create a poster, not merely an artistic rendering: establish a poster proposition, a thumbnail-readable silhouette, an intentional layout system, and a clear hierarchy of dominant image, supporting graphic field, negative space, and optional type zone.
- Derive a fresh functional palette from each source image. Do not reuse a fixed house palette merely because a previous poster succeeded.
- Establish one focal anchor and preserve only the minimum identity cues needed around it.
- Use selective rendering. Keep one controlled area resolved; simplify, fragment, wash out, omit, or leave other regions as substrate or negative space.
- Include at least one intentional lost-edge transition where a non-critical contour disappears into paper, pigment, ink, paint, halftone, shadow, or background color.
- Keep the artwork edge open in at least one region. Avoid a uniformly filled rectangular image, decorative border, poster frame, or full-bleed filter effect unless explicitly requested.
- Reserve an intentional type zone that functions as active negative space, not an empty leftover margin.
- Add scene-specific English poster typography by default unless the user explicitly requests no text. Read and apply [references/typography.md](references/typography.md). Use one short condensed uppercase title and, when compositionally useful, zero to three smaller editorial text groups derived from the visible subject, mood, motion, place, material or poster proposition. Keep one unified typography family across a series while allowing scale, position, angle, masking and overlap to respond to each source image.
- Never add signatures, seals, watermarks, invented logos, fake credits, dates, brands, or factual claims. If the user supplies exact wording, preserve it exactly. If exact spelling is mission-critical and the image model cannot render it reliably, generate a clean type-safe zone and recommend composing the final lettering separately.

Treat 3:4, poster proposition, intentional layout, hierarchy, medium-led recomposition, selective rendering, the default typography system, type-safe negative space, and intentional edge loss as hard acceptance criteria, not optional style suggestions.

## Choose an art mode

Read [references/art-modes.md](references/art-modes.md) after selecting a mode. Use its medium grammar, composition moves, color logic, failure checks, and prompt vocabulary.

- **Transparent watercolor:** atmospheric light, fluid edges, pigment blooms, paper showing through.
- **Pop screenprint:** bold shape separation, limited high-impact palette, halftone, registration play.
- **Expressive painting:** directional brush energy, impasto hierarchy, emotional color construction.
- **Ink-wash:** tonal economy, breathing space, calligraphic structure, controlled diffusion.
- **Relief print:** carved silhouettes, forceful black-white rhythm, tactile cut marks.
- **Editorial surrealism:** one legible conceptual transformation, believable visual logic, restrained symbolism.
- **Controlled hybrid:** one primary mode plus one supporting process. Never blend more than two modes.

Interpret “波普” as pop-art/screenprint. If the user writes “波谱” in an art-style context, treat it as likely referring to 波普 unless frequency-spectrum imagery is explicitly requested.

## Build the transformation brief

Resolve these decisions before prompting:

1. **Output:** vertical 3:4 aspect ratio, intended poster context, viewing distance, and whether the user has overridden the default English typography.
2. **Preservation:** exact identity anchors and spatial logic to retain.
3. **Poster proposition:** one short visual statement or emotional promise; never a vague style label.
4. **Layout system:** choose one system from [references/poster-systems.md](references/poster-systems.md) and map the focal image, supporting field, type zone, and eye path.
5. **Transformation:** what becomes simplified, exaggerated, dissolved, repeated, displaced, or recolored.
6. **Medium behavior:** physical marks, edge behavior, layering, pigment/ink/paint interaction, and substrate.
7. **Composition:** focal point, eye path, dominant and subordinate masses, source elements to move/crop/scale/omit, and active negative space.
8. **Coverage map:** resolved focal region, simplified support region, untouched or substrate-led region, and the exact contours selected for lost-edge treatment.
9. **Graphic devices:** select no more than two source-derived devices such as crop bar, repeated contour, enlarged detail, color block, halftone field, registration echo, or directional rule. Do not add arbitrary decoration.
10. **Palette:** extract the source's dominant color, identity accent, environmental color, and substrate opportunity, then build a source-specific 3–6 color functional palette. Preserve or strategically intensify recognition-bearing colors such as a lamp, garment, brake caliper, painted graphic, sign, material finish, or atmospheric light. Suppress muddy or expendable colors. Permit hue shifts and stronger value, saturation, or temperature contrast when they clarify hierarchy, but never impose a fixed palette from an earlier poster.
11. **Typography:** read [references/typography.md](references/typography.md), derive one short English title and zero to three optional supporting text groups from the visible image, assign exact wording and hierarchy, choose a source-responsive title direction, and define any controlled foreground-background interaction between the title and subject. Keep the locked typography family consistent across a series while varying placement according to each composition.
12. **Exclusions:** generic filter look, centered product-shot layout, equal detail, edge-to-edge uniform treatment, stray or misspelled text, watermark, unwanted frames, fake mockups, extra anatomy, and style-specific failure modes.

Use medium-native verbs. Watercolor should bleed, pool, granulate, glaze, lift, and reserve paper; screenprint should separate, overprint, misregister, repeat, and halftone. Avoid relying on artist names. Describe visual properties and processes instead.

## Composition rules

- Read [references/poster-systems.md](references/poster-systems.md) before prompting. Choose one layout system; do not average several systems together.
- Establish one dominant visual idea that is readable at thumbnail size.
- Build at least three clearly different spatial zones: dominant image, supporting graphic/material field, and active negative/type-safe space. These may overlap but must remain hierarchically legible.
- Create scale contrast. The focal anchor should be decisively larger, sharper, darker, brighter, or more saturated than supporting elements.
- Integrate the title with source geometry. Permit controlled masking, overlap, vertical stacking, edge cropping or one source-derived diagonal when it strengthens depth and hierarchy. Keep the title understandable at thumbnail size and never hide several essential letters.
- Recompose for the 3:4 canvas using crop, scale shift, asymmetric placement, overlap, repetition, compression, or expanded negative space when appropriate to the medium.
- Let one area carry detail and let other areas simplify, disappear, or breathe. Do not distribute finish evenly.
- Change at least two of these dimensions so the result is a true reinterpretation: shape, color, material, scale, space, repetition, or narrative meaning.
- Connect artistic effects to source geometry. Do not scatter arbitrary splashes, dots, collage scraps, or symbols as decoration.
- Connect color to source evidence. Let the image determine the palette family, then art-direct it for contrast and hierarchy; do not mechanically apply habitual red-blue-cream, black-yellow, or any other preset combination.
- Keep medium behavior spatially selective: sharp versus lost edges, dense versus open marks, opaque versus transparent layers.
- Use lost edges structurally: dissolve contours on the shadow side, motion side, atmospheric side, or where the subject meets a similar value/color. Keep defining edges near the focal anchor legible.
- Allow peripheral forms to terminate before the canvas edge or merge into exposed substrate. The artwork need not depict every source element.
- Preserve user-requested wording exactly. Otherwise derive restrained scene-specific English copy and apply the locked typography system. Use one dominant title and no more than three supporting text groups. State every permitted word exactly in the generation prompt and forbid all other lettering. Prefer fewer accurate words over corrupted subtitles, fake metadata or decorative filler text.
- Avoid the common pseudo-poster solution of placing an unchanged centered subject over a textured background. At least two structural relationships from the source must change: crop/scale, placement, overlap, repetition, figure-ground, or negative-space distribution.

## Hybrid rules

Use a hybrid only when it creates a clear division of labor:

- primary mode controls composition, shapes, and dominant material;
- supporting mode contributes one limited behavior such as halftone, ink contour, collage displacement, or metallic accent;
- assign each process to specific regions;
- keep one palette and one focal hierarchy across both processes.

Reject combinations that merely list styles. If removing the supporting mode does not change meaning, depth, rhythm, or focus, remove it.

## Prompt structure

Write the final image-generation prompt in four compact sections:

1. **Source fidelity:** identify the supplied image, identity anchors, and spatial logic that must survive.
2. **Poster direction:** state `vertical 3:4 aspect ratio`, the poster proposition, chosen layout system, thumbnail silhouette, focal anchor, scale contrast, eye path, type zone, and source elements to crop, move, enlarge, repeat, suppress, or omit.
3. **Material, graphic, and type system:** specify physical medium behavior, substrate, palette, selective coverage map, no more than two source-derived graphic devices, exposed negative space and at least one intentional lost-edge transition. State the exact title and every permitted micro-copy group, define their hierarchy, direction and approximate positions, specify any controlled title-subject masking or overlap, apply the unified typography rules from [references/typography.md](references/typography.md), and forbid all other lettering.
4. **Guardrails:** state what must not change and forbid unchanged centered-photo layouts, uniform full-image treatment, arbitrary decoration, misspelled or additional text, frames, and relevant mode-specific failures.

Describe the desired image as a finished artwork, not as instructions to add a filter. Do not mention this skill or internal analysis in the prompt.

## Safety and privacy

- Send only the necessary reference image and final prompt to the image-generation service.
- Do not browse for, upload, save, or share the user's source image elsewhere.
- Do not save source or generated images into project files unless requested.
- Do not imitate a living artist's exact style. Translate such requests into high-level traits, medium, era, palette, and composition.
- Avoid inventing sensitive personal attributes or changing identity unless the user asks.

## Quality gate

Before accepting the result, check:

- the result is composed and generated as a vertical 3:4 image;
- the result reads immediately as an authored art poster rather than a filtered photograph or framed illustration;
- one clear poster proposition and one layout system organize the image;
- dominant image, supporting field, and active negative/type-safe space form a legible hierarchy;
- scale contrast and eye path remain clear at thumbnail size;
- the selected identity anchors remain legible;
- the composition has been meaningfully redesigned for the selected medium rather than copied from the source by default;
- the medium behaves physically rather than as a uniform digital overlay;
- the image has a clear focal hierarchy, selective rendering, and intentional empty or substrate-led areas;
- at least one non-critical contour uses a convincing lost edge while defining focal edges remain readable;
- the canvas is not uniformly filled or boxed by an unwanted frame;
- the palette is coherent and structurally useful;
- the palette is recognizably derived from the current source image, protects meaningful identity accents, and is not copied from a previous poster by default;
- the transformation feels source-specific rather than template-like;
- graphic devices derive from source geometry and do not behave as arbitrary decoration;
- the English title is concise, legible, correctly spelled, source-relevant and rendered in the locked condensed uppercase editorial form unless the user requested another treatment or no text;
- supporting copy uses the same typography family, contains no more than three restrained text groups and remains subordinate to the focal image and title;
- title direction and any image-title overlap respond to visible source geometry, strengthen hierarchy and preserve thumbnail readability;
- no additional lettering, watermark, mockup frame, or unwanted object appears;
- hands, faces, product geometry, and vehicle proportions remain credible where relevant.

If the first result misses a defining requirement, revise the prompt with a precise correction and regenerate once. Do not repeatedly generate minor variants unless the user requests exploration.
