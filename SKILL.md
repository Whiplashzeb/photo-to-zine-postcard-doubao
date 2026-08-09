---
name: photo-to-zine-postcard-doubao
description: Convert one user-provided photograph into a coordinated two-sided 2:3 editorial photo-zine postcard in Doubao Work Task mode. Use when the user asks for a Zine postcard, photo-to-postcard transformation, a minimal collectible travel print, or front-and-back postcard generation from a photo. Preserve the source photograph, create one restrained ink-and-wash visual annotation, extract exactly three source-faithful pigment swatches, and verify both deliverables before claiming completion.
---

# Photo to Zine Postcard — Doubao Edition

## Choose the Doubao surface first

Determine which surface is available before generating:

- **Work Task / installed skill:** follow the complete workflow in this file.
- **Ordinary chat with Image Generation:** read and follow [`references/doubao-dialog.md`](references/doubao-dialog.md). Use its two-pass prompt workflow instead of pasting this entire file into the image prompt.

Do not rely on Image Generation mode to browse a GitHub URL or install a skill. In ordinary chat, explicitly select `图像生成`, `Seedream 4.5`, and `2:3`, upload the source image, and send the compact prompts from the dialogue reference. A repository link may be shared for provenance, but it is not a substitute for the prompt text.

## Creative target

Create an **independent photo-zine page that can function as a postcard**.

Do not create a conventional travel postcard with a watercolor decoration. The intended result uses photographic archiving, editorial typography, negative space, a source-derived visual annotation, and small pigment tests. The photograph remains the evidence; the illustration comments on it.

Treat the following priorities as immutable, in this order:

1. recognizable photo-zine editorial language
2. source photograph preserved unchanged
3. fixed composition and large negative space
4. source-faithful color relationships
5. restrained ink-and-wash annotation
6. exactly three pigment swatches
7. minimal typography used once
8. separate functional back

If a lower-priority choice conflicts with a higher-priority rule, keep the higher-priority rule.

## Visual references

Before generating, inspect these assets visually:

- `assets/reference-front-alpine.png`
- `assets/reference-front-misty.png`
- `assets/reference-back.png`

Use them only for layout, negative space, typography scale, illustration restraint, swatch treatment, paper tone, and back structure. Do not copy their subject matter, titles, numbers, or colors into the new card.

If the generation tool accepts multiple reference images, provide the user's source photo as the content reference and the most relevant asset as the style reference. Keep the source photo authoritative for subject and color. If multiple-image reference is unavailable, translate the rules below into the generation prompt explicitly.

## Output contract

Produce exactly two separate portrait images:

1. `front` — photo-zine editorial face
2. `back` — functional postcard back

Use a `2:3` portrait ratio. Prefer `2048 × 3072` when supported.

Generate and verify the front first. Generate and verify the back second. Never claim that both are complete unless two distinct finished images are visible and attached. If only one image exists, say which image is missing and generate it.

## Step 1 — Analyze the source

Inspect the photograph before writing a generation prompt. Determine:

- its actual aspect ratio
- one source-defining visual motif
- one optional supporting fragment
- the real dominant chromatic color
- the real darkest structural color
- one pale neutral or quiet accent
- a short editorial title of two to four words
- location, date, and index only when supplied or safely derived from the filename

Do not invent a location or date. Leave their values blank when unavailable.

Choose the motif for visual identity, not ease of isolation. Prefer a distinctive ridge, shoreline, water contour, tree cluster, architectural fragment, reflection, window, plant, or other recognizable structure. Do not automatically redraw the entire photograph.

## Step 2 — Lock the front composition

Use one flat, edge-to-edge card canvas. Do not depict a card lying on another background.

### Paper

- warm neutral ivory, approximately `#F5F1E8`
- extremely subtle uncoated paper grain
- no yellow vintage filter
- no dark vignette, shadow, mockup, or rounded outer corners

### Source photograph

- place in the upper `42%–46%` of the card
- use approximately `86%–90%` of the card width
- center horizontally
- preserve the exact source image and its aspect ratio
- do not repaint, retouch, extend, replace, or stylize the photo
- do not crop unless necessary to fit and explicitly permitted
- use only a hairline grey frame and a narrow even paper gap

Do not use a Polaroid frame, thick mat, tape, scrapbook corner, drop shadow, caption strip, or floating photo card.

### Negative space

Keep the central area deliberately empty. Preserve at least `14%–18%` of card height as uninterrupted ivory space between the photograph and lower editorial content. This silence is a primary Zine device, not unused space to fill.

### Lower editorial area

- metadata block: lower-left
- main visual annotation: lower-right or lower center-right
- optional supporting fragment: one only, no more than `25%` of the main annotation
- three pigment swatches: one horizontal row below the metadata

The annotation may occupy about `45%–56%` of card width and `18%–26%` of card height. It must remain subordinate to the photograph and must not become a second full poster.

## Step 3 — Draw the visual annotation

Create a **selective editorial field-note illustration**, not a finished landscape painting.

Required character:

- fine graphite or cool-grey ink structure
- transparent watercolor or thin gouache washes
- broken, incomplete contours
- irregular feathered edges fading into paper
- visible ivory gaps inside and around the motif
- simplified detail while keeping the source silhouette recognizable
- source-faithful hue relationships at slightly reduced saturation
- quiet, observational, archival, and hand-made

The drawing should feel like a visual note extracted from the photograph and printed beside it. It must not sit inside a rectangular painted background.

Avoid:

- heavy wet watercolor
- muddy washes or dark pools of paint
- thick black outlines
- glossy digital painting
- photorealistic repainting
- anime, cartoon, storybook, or concept-art rendering
- full-bleed illustration rectangles
- high saturation or arbitrary color changes
- a second complete copy of the source photo

## Step 4 — Preserve source color

Extract color from the source, not from generic travel-poster palettes.

Use the source photograph's true relationships:

1. `chromatic` — the most characteristic colored feature
2. `structural` — the deepest natural dark that organizes the image
3. `quiet` — a pale neutral, sky tone, mineral tone, paper-adjacent color, or restrained accent

Apply those same three color families to the illustration. Reduce saturation slightly for an uncoated printed-paper feeling, but do not shift blue water to turquoise, green vegetation to teal, warm stone to orange, or neutral whites to yellow unless the source actually contains those hues.

Do not add rainbow colors, fashionable complementary colors, or a stronger accent just to make the image more decorative.

## Step 5 — Render exactly three pigment swatches

Create exactly **three** separate pigment dabs in one horizontal row.

Each swatch must be:

- approximately `4%–5%` of card width
- equal in visual size
- separated by a small even gap
- a circle, soft square, or compact brush dab with slightly irregular hand-painted edges
- flat and matte, with subtle pigment variation only
- unlabeled

Order them `chromatic → structural → quiet`.

Do not use UI rectangles, rounded app chips, gradients, glossy samples, a continuous palette bar, large blocks, more than three colors, or an extra outline around the group. A pale swatch may use one hairline edge only when needed to remain visible against the paper.

Count the swatches immediately before accepting the image. Any count other than three requires regeneration.

## Step 6 — Use restrained editorial typography

Use a quiet classic book-serif hierarchy similar to an independent photography journal.

Allowed text, once each:

- one title
- optional italic `Postcard` or `Postcard Study`
- `LOCATION`
- `DATE`
- one `No. 0XX` index

Use thin rules below LOCATION and DATE when their values are blank. Keep all typography inside the lower-left metadata block. The title should be noticeable but never large or promotional.

Do not repeat the title, location, date, index, or labels elsewhere. Do not add descriptive copy, coordinates, keywords, credits, badges, logos, or pseudo-English. Do not invent visible field values.

## Step 7 — Generate the front

Use Seedream 4.5 when it is explicitly available. Use the source photo as an image reference, not merely as a textual description.

Build the prompt with the following order:

1. declare `editorial photo-zine page`, not travel postcard
2. lock the canvas, photo bounds, and negative space
3. name the chosen source motif
4. describe the fine ink-and-thin-wash treatment
5. state the three source-derived color families
6. lock swatch count and shape
7. provide the exact allowed text
8. append the forbidden styles

Use this prompt skeleton and replace every bracketed value:

```text
生成一张 2:3 竖版的独立摄影 Zine 内页，同时可以作为明信片正面。它不是旅行纪念明信片，不是 Polaroid，不是剪贴簿，也不是“照片下面放一幅水彩画”。整张图是平面的单张成品，不要展示桌面、投影、圆角卡片或样机。

上方嵌入用户提供的真实照片，占画面高度约 44%、宽度约 88%，居中。保持原照片内容、色彩、比例和摄影质感不变，不重绘、不扩图、不换图、不美化。只加极细灰色边线与均匀窄纸边；禁止厚相框、胶带和阴影。

照片下方保留约 16% 画面高度的连续象牙白留白，绝对不要填充装饰。

下半部左侧是唯一一组极简档案文字；右侧是从原照片提取的“[MAIN_MOTIF]”视觉注释。视觉注释不是完整风景画：使用细冷灰墨线控制结构，叠加透明、克制、偏干的水彩薄涂；轮廓断续，边缘自然消失在纸面，内部保留大量纸白，像独立摄影杂志中的手绘观察笔记。保持原照片真实轮廓和色彩关系，整体轻、薄、安静、低饱和。禁止厚重水彩、油画感、数字插画感、完整矩形画布、黑粗线和高饱和。

颜色只允许围绕原照片提取的三个色系：[CHROMATIC]、[STRUCTURAL]、[QUIET]。不得自行增加互补色或改变冷暖关系。

左下方只出现一行三个小型颜料试色点，顺序为 [CHROMATIC]、[STRUCTURAL]、[QUIET]。必须恰好三个，大小一致、间距均匀、哑光、边缘略有手工颜料的不规则感；禁止 UI 色块、长条色卡、渐变和第四个颜色。

文字只允许出现一次：标题“[TITLE]”、斜体“Postcard”、LOCATION、DATE、No. [INDEX]。LOCATION 和 DATE 未提供内容时只保留标签和细横线。禁止重复标题、重复字段、说明文字、关键词、坐标、徽章或装饰标签。

纸张为中性暖象牙白，只有极轻微的无涂布纸纹。整体气质：independent photography zine、editorial archive、Swiss/Japanese book design、quiet collectible print、large negative space。
```

## Step 8 — Verify the front

Inspect the actual generated image. Regenerate the front when any item fails:

- source photo was changed, repainted, replaced, or heavily cropped
- photo looks like a Polaroid, scrapbook, or floating card
- negative space is missing or filled
- the lower-right visual annotation is missing, too faint to read, or materially smaller than specified
- illustration looks like a second complete painting instead of an annotation
- illustration sits inside a visible rectangle, frame, card, or second image boundary
- illustration colors do not match the source relationships
- swatch count is not exactly three
- swatches look like UI components rather than pigment dabs
- metadata is duplicated, invented, or placed more than once
- added modules, decorations, frames, captions, or logos appear

Attempt up to two targeted regenerations. In a correction prompt, name only the failed rules and say that all passing parts must remain unchanged.

## Step 9 — Generate the back separately

After the front passes, generate a new separate image using this structure:

- same `2:3` ratio and neutral ivory paper
- one hairline outer border inset from the edge
- `POST CARD` in small widely spaced serif capitals at upper-left
- one thin vertical divider slightly right of center
- one thin rectangular stamp box at upper-right with small `PLACE / STAMP / HERE`
- exactly four thin address lines on the right
- large completely blank writing area on the left
- one source-derived line-art watermark at lower-left at `4%–7%` opacity
- the same `No. 0XX` index once at lower-left

Do not add swatches, palettes, collage, illustration blocks, extra horizontal dividers, duplicate indices, or decoration that reduces writing space.

Use this prompt skeleton:

```text
生成一张独立的 2:3 竖版明信片背面，必须是与正面分开的第二张图片。沿用正面的中性暖象牙白无涂布纸张和极细灰褐线条，整体平面、克制、没有样机和阴影。

结构固定：内缩极细外边框；左上角小号宽字距衬线体“POST CARD”；中央偏右一条竖向分隔线；右上角一个细线邮票框，框内小字 PLACE / STAMP / HERE；右侧恰好四条地址横线；左侧保留完整大面积书写空间。

左下角只放一次 No. [INDEX]，并加入一个来自正面主元素“[MAIN_MOTIF]”的极淡线稿水印，透明度约 4%–7%，只能位于左下区域，不影响书写。

禁止色块、调色板、拼贴、完整插画、额外横向分割线、重复编号、重复 POST CARD、装饰图标和大面积水印。
```

## Step 10 — Verify delivery

Before the final response, confirm visually:

- two distinct images exist
- both are portrait `2:3`
- the first is the front and contains the unchanged source photo
- the second is the functional back
- front has exactly three swatches
- front metadata appears once
- back has one divider, one stamp box, four address lines, and one index

Report completion only after every item passes. Mention any unavoidable model or tool limitation plainly rather than describing an image that does not exist.
