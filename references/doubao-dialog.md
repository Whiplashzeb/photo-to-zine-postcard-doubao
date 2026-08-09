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
4. 下半部右侧清晰绘制刚才自动选择的主体轮廓，占卡片宽度约 45%。它是直接画在纸上的开放式手绘观察笔记，不是第二张照片或完整风景画。使用冷灰细墨线、断续轮廓，以及从原图三个色系中提取的透明偏干水彩薄涂；边缘自然消失在纸面，内部保留大量纸白。不能只画空线稿。下半部不画任何矩形边框，不画包围插画或文字的线框，不画左右分隔竖线，不画上下分隔横线；整张图中唯一允许的直线只有照片的极细边线，以及 LOCATION、DATE 后各一条短横线。
5. 左下只出现一组档案文字。整张图的文字严格只有 5 项，各出现 1 次：自动生成的英文标题；斜体 Postcard；LOCATION 与空白短横线；DATE 与空白短横线；No. 加一个编号。编号优先使用上传文件名末尾数字，无法读取时使用 001。LOCATION 和 DATE 保持空白。第 5 项之后不再出现任何编号或文字。
6. 档案文字下方优先只出现一行 3 个小型手绘颜料点，依次使用代表性色、最深结构色和浅色中性色。大小一致、间距均匀、哑光且边缘略不规则；不要第二行色点、UI 色块或长条色卡。
7. 纸张为中性暖象牙白，只带极轻微无涂布纸纹。整体气质：independent photography zine、editorial archive、Swiss/Japanese book design、quiet collectible print、large negative space。

输出前在内部检查：下半部边框和分隔线为 0；文字项目只有 5 项且各出现 1 次；颜料点保持一行、颜色来自原图。再检查照片未重绘、中央留白连续、右下同时有细墨线与透明薄水彩。只输出一张最终正面图片，不解释步骤，不提供第二张图。
```

## Verify the single result

Inspect the visible image, not the assistant's description:

- one recognizable, photographically preserved source image at the top
- uninterrupted central negative space
- one source-derived, unframed ink-and-thin-wash annotation at lower-right
- one metadata block at lower-left
- one compact horizontal row of source-derived pigment dabs; three are preferred, and a few extra matching dabs are acceptable
- title and illustration adapt to the photograph without a customized prompt
- no invented location or date value
- no unrequested caption, duplicate text, mockup, tape, second framed picture, or extra swatches

Use the same launcher for the complete test set. Any image-specific prompt edit invalidates the stability result.

For an eight-image release check, accept the baseline when at least six results are visually strong. Extra matching dabs are a minor variance; a missing source photo, missing Zine composition, or no generated image remains a failure.
