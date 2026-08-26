---
name: photo-poetic-editorial-collage
description: Transform a reference photograph into a hybrid editorial artwork: preserve or clean the photographic upper region while reinterpreting the lower region as an adaptive, tactile, poetic visual diary made from cut-paper shapes, abstract symbols, handwritten notes, grain, paper texture, and intelligent spatial relationships. Use when the user asks to turn a photo into an artistic lower-half collage, visual diary, editorial sketchbook, poetic reconstruction, or concept-driven mixed-media layout.
---

# Photo → Poetic Editorial Collage

## Goal

Create a new image from a supplied photograph. The result should not merely decorate the photo. It should **interpret** it.

Default presentation logic:
- Upper region: retain or reconstruct the photographic scene in a clean, believable way.
- Lower region: translate the image into an adaptive editorial collage / visual-diary language.
- The split ratio is flexible; default to roughly 50/50 only when the user gives no stronger compositional cue.

The lower section should feel improvised, tactile, poetic, and highly intentional rather than template-driven.

## Trigger conditions

Use this skill when the user asks for one or more of the following:
- “把这张图下半部分做成拼贴 / 手账 / 杂志感”
- “根据照片内容自动生成视觉符号”
- “做成艺术编辑、视觉日记、独立杂志风格”
- “保留照片，上半部分真实，下半部分抽象化”
- “不要固定模板，每张图都要根据内容变化”
- “从照片里提取隐喻、符号、诗句、图形关系”

If no usable source image is present, ask the user to upload one. Otherwise, proceed without clarification unless the user explicitly requests parameter choices.

## Core principles

### 1. Interpret before composing

Before generating, infer the following from the photograph:
- Primary subject
- Secondary visual cues
- Dominant geometry / silhouette
- Spatial direction or movement
- Mood / atmosphere
- Cultural or contextual signals
- 3–6 candidate symbolic motifs
- 1–3 latent meanings or poetic associations
- Dominant color family and material feel

Do not surface this analysis unless the user asks for it.

### 2. Translate, do not trace

The lower section must **not** literally redraw the photograph.

Instead, translate photographic elements into a compact visual vocabulary:
- architecture → stacked silhouettes, roof curves, portals, steps, circles, rings
- person → dot, stick figure, shadow, path marker, handwritten trace
- landscape → torn field, horizon line, folded paper, contour mark
- motion → arrows, repeated strokes, offset shapes, broken lines
- light → gold leaf patch, translucent disc, soft halo
- silence → empty space, thin line, tiny notation
- crowd → clustered marks, small repeated figures
- ritual / memory → stamps, rings, sequence marks, layered paper

Choose symbols that are semantically connected to the specific source image.

### 3. Adaptive composition, never a fixed template

Avoid rigid grids and repeated poster formulas.

The lower section may use:
- floating islands of content
- asymmetric clusters
- overlapping cut-paper forms
- one large anchoring silhouette plus smaller fragments
- wide negative space
- off-axis handwritten annotations
- accidental-looking alignments
- visual echoes between upper photo and lower abstraction

Let the source image determine the composition.

### 4. Tactile handmade editorial language

Use a restrained material vocabulary:
- cut-paper-like flat forms
- softly imperfect silhouettes
- torn edges
- subtle paper fibers
- light grain
- stamped or screen-printed texture
- hand-drawn lines
- naïve diagrammatic marks
- imperfect circles and rectangles
- pencil / ink notations
- occasional gold or metallic-looking printed accents if the source supports it

The result should feel like a hybrid of:
- artist sketchbook
- visual diary
- independent art publication
- editorial art direction
- conceptual collage

### 5. Typography must be sparse and image-specific

Generate only a few meaningful fragments.

Preferred quantity:
- 2–4 fragments total
- 1–7 words per fragment

Text can be:
- a poetic observation
- a private annotation
- a visual thought
- a tiny label
- a conceptual note

Avoid conventional poster copy, slogans, titles, metadata blocks, and dense paragraphs.

Typography may be handwritten, lightly typeset, tilted, offset, or partially isolated. Placement should contribute to visual rhythm.

If typography quality is uncertain, reduce the amount of text rather than forcing legibility.

## Photographic upper region

When the source image contains app UI, social-media buttons, interface chrome, counters, stickers, or unrelated overlays:
- remove them unless the user explicitly asks to preserve them
- reconstruct the obscured photographic region plausibly
- keep the subject faithful to the original photo
- preserve recognizable architecture, pose, object, or landscape
- avoid over-retouching or turning the entire upper region into illustration

The photographic region should remain visually coherent with the lower collage through palette, rhythm, and thematic echoes.

## Composition compiler

Use the following internal sequence for each image:

1. **Anchor** — choose one dominant lower-half visual motif derived from the source.
2. **Echo** — repeat 1–2 geometric cues from the photo in abstract form.
3. **Counterpoint** — add one unexpected symbolic element that reveals hidden meaning.
4. **Trace** — add hand-drawn linework, path, measure, ring, or small diagram.
5. **Voice** — add 2–4 short textual fragments.
6. **Air** — preserve generous negative space.
7. **Bridge** — create at least one visual relationship between upper photo and lower collage.

## Image-generation instruction template

When generating or editing the image, compile the source-specific prompt around the following logic:

> Use the supplied photograph as the semantic and visual source. Preserve or clean the photographic upper region, removing unrelated interface overlays when present. Reinterpret the lower region as an adaptive, tactile editorial collage that emerges specifically from the source image rather than from a fixed template. First infer the subject, mood, geometry, action, cultural context, and hidden meaning, then translate those qualities into 3–6 simplified visual symbols, abstract shapes, poetic fragments, hand-drawn marks, cut-paper silhouettes, subtle grain, paper texture, lightly printed surfaces, and intelligently spaced relationships. Do not literally redraw the photographed scene in the lower section. Use metaphor, diagram, visual echo, negative space, and naïve-but-intentional symbolic imagery. Keep the layout asymmetric, intuitive, loosely assembled, and editorially refined. Include only a few short image-specific words or poetic observations, placed like private notes rather than poster copy. Match the source image’s palette and structural rhythm while allowing one or two restrained accent tones. The final image should feel like an artist’s sketchbook, independent art publication, visual diary, and conceptual editorial artwork combined: playful, poetic, tactile, slightly naïve, spontaneous, but highly intentional.

Then append source-specific motifs, colors, metaphors, and text fragments inferred from the actual image.

## Visual quality checks

Before final generation, ensure:
- lower section is conceptually derived from the actual image
- no generic scrapbook decorations dominate
- no rigid template is visible
- negative space is intentional
- typography is sparse
- source palette is echoed without becoming monochromatic
- photo and collage feel like one authored piece
- visual symbols are simple but not random
- the lower section communicates at least two layers of meaning
- composition is sophisticated even if forms are naïve

## Negative constraints

Avoid:
- generic mood-board layouts
- scrapbook clichés
- excessive stickers
- dense text
- corporate infographic styling
- rigid 3-column or 12-column grids
- symmetrical poster formulas
- literal scene reconstruction in the lower section
- unrelated symbols
- over-polished vector illustration
- glossy 3D iconography
- UI mockup aesthetics
- excessive decorative clutter
- fake quotes or unsupported factual captions
- repeating the exact same composition across different source photos

## Default behavior

If the user gives only an image and asks for “the same style” or “use this skill”:
- infer everything else from the image
- preserve the original aspect ratio unless the user specifies another
- clean irrelevant UI overlays
- use a flexible upper-photo / lower-collage split
- generate the final image directly
- do not explain the image afterward unless the user asks

## Optional user controls

Only apply these when explicitly requested:
- `photo_ratio`: e.g. 60/40, 50/50, 40/60
- `text_language`: Chinese / English / bilingual / none
- `editorial_density`: sparse / medium / dense
- `material_bias`: paper / ink / stamp / pencil / fabric / mixed
- `poetry_level`: literal / restrained / poetic / abstract
- `preserve_ui`: true / false
- `aspect_ratio`: source / 4:5 / 3:4 / 1:1 / 9:16 / other

## Host capability behavior

If the host environment provides an image-generation or image-editing tool, use it to render the final visual.

If the host does **not** provide image-generation capability, do not claim that an image was rendered. Instead, output a production-ready image prompt / art-direction package compiled from the same interpretation workflow so the user can pass it to an image model or creative tool.
