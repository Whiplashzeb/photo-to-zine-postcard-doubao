---
name: photo-to-zine-postcard-doubao
description: Convert one user-provided photograph into a 2:3 editorial photo-zine postcard front in Doubao. Use when the user asks for a Zine postcard, photo-to-postcard transformation, or a minimal collectible photo print generated in Work Task or ordinary Image Generation chat. Preserve the source photograph, create one restrained ink-and-wash visual annotation, extract exactly three source-faithful pigment swatches, and verify the finished front before claiming completion.
---

# Photo to Zine Postcard — Doubao Edition

## Choose the Doubao surface first

Determine which surface is available before generating:

- **Work Task / installed skill:** follow the complete workflow in this file.
- **Ordinary chat with Image Generation:** read and follow [`references/doubao-dialog.md`](references/doubao-dialog.md). Test its link-free GitHub discovery launcher first; use its direct single-pass prompt only as the fallback.

Do not assume Image Generation mode can browse GitHub. Verify that capability with the short discovery launcher instead of hiding the full prompt in the same message. If discovery fails, switch the published user instructions to the direct universal prompt. In either path, explicitly select `图像生成`, `Seedream 4.5`, and `2:3`, upload one source image, send one unchanged prompt, and expect one final front.

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

If a lower-priority choice conflicts with a higher-priority rule, keep the higher-priority rule.

## Visual references

In Work Task or another surface that can load bundled assets, inspect these assets visually:

- `assets/reference-front-alpine.png`
- `assets/reference-front-misty.png`

Use them only for layout, negative space, typography scale, illustration restraint, swatch treatment, and paper tone. Do not copy their subject matter, titles, numbers, or colors into the new card.

In ordinary Image Generation chat, upload only the user's photograph by default and translate the rules below into the prompt explicitly. Treat a bundled front asset as an optional development fallback only when repeated no-reference benchmarks fail. If a fallback style image is used, keep the source photo authoritative for subject and color.

## Output contract

Produce exactly one portrait image: `front` — the finished photo-zine editorial face.

Use a `2:3` portrait ratio. Prefer `2048 × 3072` when supported.

Never claim completion unless one finished front image is visible and passes the front verification checklist.

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
- the paper extends exactly to all four canvas edges; do not draw a separate card silhouette or outer background
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

Inspect the actual generated image against these failure conditions:

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

Ordinary chat has a one-request, one-output contract. Do not ask the user to send a correction prompt and do not make a second image part of the expected workflow. Put every hard constraint into the first generation prompt. If the visible output still fails, report the failed check plainly for skill iteration rather than claiming success.

After the front passes, deliver that single image and stop. Mention any unavoidable model or tool limitation plainly rather than describing an image that does not exist.
