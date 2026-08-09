# Doubao ordinary-chat workflow

Use this workflow when Work Task skill installation is unavailable or out of quota. It is optimized for Doubao's ordinary `图像生成` mode and has a strict one-request, one-output contract.

## 1. Configure the chat before prompting

1. Start a clean ordinary chat.
2. Select `图像生成`.
3. Select `Seedream 4.5` when available.
4. Set the ratio to `2:3` before sending the prompt.
5. Upload only the user's source photograph. Do not require a layout reference in the default workflow.

The bundled front references are for skill development and benchmarking. Use one only as an optional fallback when repeated no-reference tests fail; never make it part of the standard user instructions.

Do not ask Image Generation mode to read a GitHub link. It does not reliably browse or install skills. Paste the prompt itself.

## 2. Generate the finished front in one pass

Replace every bracketed value. Send this once and expect one finished front with no follow-up correction.

```text
用户上传的图片是唯一的内容与颜色来源。不要寻找、假设或引用第二张图。

生成一张单独的 2:3 竖版独立摄影 Zine 明信片正面。以下规则必须在同一张图里全部满足，一轮生成即结束。

1. 象牙白纸张本身就是整张画布，从左上角连续延伸到右下角，四条画布边缘就是纸张边缘；不要在白色背景上再画一张卡片，不要卡片外轮廓。整张成品是四个直角的 2:3 平面；绝对不要圆角、外部背景、桌面样机、阴影、Polaroid、胶带或剪贴簿。

2. 上方放置图1的真实照片，占高度约 44%、宽度约 88%，保持摄影质感、真实颜色和原始比例，不重绘、不扩图、不换图，只加极细灰线和窄纸边。

3. 照片下方保留约 16% 高度的连续象牙白留白，完全空白，不放文字、图案或装饰。

4. 下半部右侧必须清晰出现从图1提取的“[MAIN_MOTIF]”手绘观察笔记，占卡片宽度约 45%。它没有矩形边框，不是第二张照片，不是完整风景画。使用冷灰细墨线和断续轮廓；轮廓内部必须有清晰可见但非常克制、透明、偏干的 [CHROMATIC] 与 [QUIET] 水彩薄涂，边缘直接消失在纸面，内部仍保留大量纸白。不能只画空线稿。

5. 左下档案文字只出现一次，而且整张图只允许出现这些文字：标题“[TITLE]”、斜体 Postcard、LOCATION [LOCATION_OR_BLANK]、DATE [DATE_OR_BLANK]、No. [INDEX]。禁止中文句子、说明文字、第二标题、标签、坐标和任何其他文字。

6. 档案文字下方只有一行恰好 3 个小型手绘颜料点，依次为 [CHROMATIC]、[STRUCTURAL]、[QUIET]；三个大小一致、间距均匀、哑光且边缘略不规则。不得出现第四个色点、第二行色点、UI 色块或长条色卡。

7. 纸张为中性暖象牙白，只带极轻微无涂布纸纹。整体气质：independent photography zine、editorial archive、Swiss/Japanese book design、quiet collectible print、large negative space。

输出前在内部检查：纸张铺到画布四边且没有卡片外轮廓；四个直角；照片未重绘；中央留白连续；右下无边框且同时有细线与透明薄水彩；左下文字只出现一次；整张图没有其他文字；色点恰好 3 个且只有一行。只输出一张最终正面图片，不解释步骤，不提供第二张图。
```

## 3. Verify the single result

Count and verify the visible result, not the assistant's description:

- one unchanged source photograph at the top
- uninterrupted central negative space
- one clearly visible, unframed ink-and-thin-wash annotation at lower-right
- one metadata block at lower-left
- exactly three pigment dabs in one horizontal row
- no unrequested caption or invented text
- no mockup, rounded card, tape, second framed picture, duplicate text, or extra swatches

If all checks pass, deliver the front and stop. Do not instruct the user to correct or regenerate. If a check fails during development testing, record the failure and improve this one-pass prompt before release.
