# Doubao ordinary-chat distribution workflow

Use one source photograph, one unchanged launcher, one generation request, and one finished front. Do not require a layout reference or a correction round.

## Configure Doubao

1. Start a clean ordinary chat.
2. Select `图像生成`.
3. Select `Seedream 4.5` when available.
4. Set the ratio to `2:3`.
5. Upload only the user's source photograph.

The bundled front images are development references, not required user inputs.

## Primary launcher — GitHub discovery without a link

Use this exact short prompt in social posts and tests. Do not append the direct prompt, because doing so would hide whether Doubao actually found and followed the skill.

```text
请在 GitHub 搜索作者 Whiplashzeb 的仓库 photo-to-zine-postcard-doubao，读取并严格执行根目录的 SKILL.md。使用我上传的照片，一轮生成一张 2:3 摄影 Zine 明信片正面，不解释步骤。
```

Count this route as successful only when Doubao discovers the correct repository and the generated image passes the visual checklist below. If it searches for unrelated material, explains the repository, asks for the link, or produces an image that only follows the short sentence, mark GitHub discovery as failed.

## Fallback launcher — direct universal prompt

Use this exact prompt unchanged for every photograph. Do not replace, add, or customize any image-specific value.

```text
用户上传的图片是唯一的内容与颜色来源。先在内部观察原图，不输出分析：自动选择一个最有辨识度的主体轮廓作为手绘元素；自动提取一个代表性色、一个最深结构色和一个浅色中性色；自动生成一个与画面有关的 2–4 个英文单词的编辑标题。不要寻找、假设或引用第二张图。

一轮生成一张 2:3 竖版独立摄影 Zine 明信片正面，以下规则必须在同一张图里全部满足：

1. 象牙白纸张本身就是整张画布，从左上角连续延伸到右下角，四条画布边缘就是纸张边缘。不要在白色背景上再画一张卡片，不要卡片外轮廓、圆角、外部背景、样机、阴影、Polaroid、胶带或剪贴簿。
2. 上方放置用户上传的真实照片，占高度约 44%、宽度约 88%，保持摄影质感、真实颜色和原始比例，不重绘、不扩图、不换图，只加极细灰线和窄纸边。
3. 照片下方保留约 16% 高度的连续象牙白留白，完全空白，不放文字、图案或装饰。
4. 下半部右侧清晰绘制刚才自动选择的主体轮廓，占卡片宽度约 45%。它必须是无矩形边框的手绘观察笔记，不是第二张照片或完整风景画。使用冷灰细墨线、断续轮廓，以及从原图三个色系中提取的透明偏干水彩薄涂；边缘直接消失在纸面，内部保留大量纸白。不能只画空线稿。
5. 左下只出现一组档案文字，而且整张图只允许出现：自动生成的英文标题、斜体 Postcard、LOCATION 与空白细横线、DATE 与空白细横线、一个 No. 编号。编号优先使用上传文件名末尾数字；无法读取时使用 001。LOCATION 和 DATE 不得自行填写内容。禁止中文句子、说明文字、第二标题、坐标、标签及任何其他文字。
6. 档案文字下方只有一行恰好 3 个小型手绘颜料点，依次使用刚才提取的代表性色、最深结构色和浅色中性色。三个大小一致、间距均匀、哑光且边缘略不规则。禁止第四个色点、第二行色点、UI 色块和长条色卡。
7. 纸张为中性暖象牙白，只带极轻微无涂布纸纹。整体气质：independent photography zine、editorial archive、Swiss/Japanese book design、quiet collectible print、large negative space。

输出前在内部检查：纸张铺到画布四边且没有卡片外轮廓；照片未重绘；中央留白连续；右下无边框且同时有细线与透明薄水彩；左下文字只出现一次；整张图没有其他文字；色点恰好 3 个且只有一行。只输出一张最终正面图片，不解释步骤，不提供第二张图。
```

## Verify the single result

Inspect the visible image, not the assistant's description:

- one recognizable, photographically preserved source image at the top
- uninterrupted central negative space
- one source-derived, unframed ink-and-thin-wash annotation at lower-right
- one metadata block at lower-left
- exactly three pigment dabs in one horizontal row
- title and illustration adapt to the photograph without a customized prompt
- no invented location or date value
- no unrequested caption, duplicate text, mockup, tape, second framed picture, or extra swatches

Use the same launcher for the complete test set. Any image-specific prompt edit invalidates the stability result.
