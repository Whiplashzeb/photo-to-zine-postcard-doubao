# Doubao ordinary-chat workflow

Use this workflow when Work Task skill installation is unavailable or out of quota. It is optimized for Doubao's ordinary `图像生成` mode and intentionally uses two short passes.

## 1. Configure the chat before prompting

1. Start a clean ordinary chat.
2. Select `图像生成`.
3. Select `Seedream 4.5` when available.
4. Set the ratio to `2:3` before sending the prompt.
5. Upload the user's source photograph.
6. Optionally upload one layout reference:
   - use `assets/reference-front-alpine.png` for subjects with clear hard contours
   - use `assets/reference-front-misty.png` for soft, organic, or atmospheric subjects

When two images are uploaded, identify them explicitly in the prompt: image 1 supplies all content and color; image 2 supplies layout, scale, negative space, typography, and print restraint only. Never allow image 2's landscape, title, number, or palette to enter the output.

Do not ask Image Generation mode to read a GitHub link. It does not reliably browse or install skills. Paste the prompt itself.

## 2. Generate the front structure

Replace every bracketed value. Keep this first pass focused on the visual hierarchy.

```text
图1是唯一的内容照片；如果上传了图2，图2只能作为版式和 Zine 气质参考，绝对不要复制图2的景物、标题、编号或颜色。

生成一张单独的 2:3 竖版独立摄影 Zine 明信片正面。整张成品平面铺满画面，不是桌面样机，不要圆角外卡片、阴影、Polaroid、胶带或剪贴簿。

上方放置图1的真实照片，占高度约 44%、宽度约 88%，保持摄影质感、真实颜色和原始比例，不重绘、不扩图、不换图，只加极细灰线和窄纸边。照片下方保留约 16% 高度的连续象牙白留白，不放任何装饰。

下半部采用独立摄影杂志版式：左侧预留档案文字与色点区域；右侧必须清晰出现从图1提取的“[MAIN_MOTIF]”手绘观察笔记，占卡片宽度约 45%。它没有矩形边框，不是第二张照片，不是完整风景画：使用冷灰细墨线、断续轮廓和透明偏干的水彩薄涂，边缘直接消失在纸面，内部保留纸白，颜色只来自图1并略微降低饱和度。

左下档案文字只出现一次：标题“[TITLE]”、斜体 Postcard、LOCATION [LOCATION_OR_BLANK]、DATE [DATE_OR_BLANK]、No. [INDEX]。其下只有一行恰好 3 个小型手绘颜料点，依次为 [CHROMATIC]、[STRUCTURAL]、[QUIET]；三个大小一致、间距均匀、哑光且边缘略不规则。不得出现第四个色点、第二行色点、UI 色块或长条色卡。

纸张为中性暖象牙白，只带极轻微无涂布纸纹。整体气质：independent photography zine、editorial archive、Swiss/Japanese book design、quiet collectible print、large negative space。只输出一张正面图片。
```

## 3. Inspect before accepting

Count and verify the visible result, not the assistant's description:

- one unchanged source photograph at the top
- uninterrupted central negative space
- one clearly visible, unframed ink-and-thin-wash annotation at lower-right
- one metadata block at lower-left
- exactly three pigment dabs in one horizontal row
- no mockup, rounded card, tape, second framed picture, duplicate text, or extra swatches

If all six checks pass, continue to the back. Otherwise send one correction prompt while the previous image remains in the conversation.

## 4. Apply one targeted correction pass

List only the failed items. Use this tested correction structure and delete any clause that already passes:

```text
修改上一张已经生成的 2:3 明信片正面，只修正以下失败项，其他合格部分全部保持不变：

1. 删除右下插画外面的任何矩形边框和第二张图片感。把它改成无边框、轮廓断续、直接消失在纸面上的“[MAIN_MOTIF]”冷灰细墨线＋透明薄水彩观察笔记，仍位于右下方并清晰可见。
2. 左下方现在有 [ACTUAL_COUNT] 个色点，删除多余色点；最终必须恰好只有 3 个，单独一行横向排列，依次为 [CHROMATIC]、[STRUCTURAL]、[QUIET]，不要第二行。
3. 在左下色点上方补回唯一一组小号书籍衬线体档案文字：[TITLE]；下一行斜体 Postcard；LOCATION [LOCATION_OR_BLANK]；DATE [DATE_OR_BLANK]；No. [INDEX]。不要出现任何其他文字。

绝对不要改变上方真实照片、2:3 比例、象牙白纸张和中部大面积留白。直接输出修正后的单张正面。
```

Do not run more than two correction passes. When a correction regresses a previously passing element, name that regression explicitly in the next prompt.

## 5. Generate the back only after the front passes

Keep `图像生成`, `Seedream 4.5`, and `2:3` selected. Start a separate image generation and use:

```text
生成一张与上一张正面配套、但完全独立的 2:3 竖版明信片背面。中性暖象牙白无涂布纸，平面成品，没有样机、圆角外卡片或阴影。

结构固定：内缩极细灰褐外边框；左上角小号宽字距衬线体 POST CARD；中央偏右一条竖向分隔线；右上角一个细线邮票框，框内小字 PLACE / STAMP / HERE；右侧恰好四条地址横线；左侧保留完整大面积书写空间。左下角只出现一次 No. [INDEX]，并加入来自正面“[MAIN_MOTIF]”的极淡细线稿水印，透明度约 4%–7%。

禁止色点、调色板、拼贴、完整插画、额外横向分割线、重复编号、重复 POST CARD 和大面积水印。只输出一张背面图片。
```

Verify that the back is a second distinct image with one divider, one stamp box, exactly four address lines, and one index before reporting completion.
