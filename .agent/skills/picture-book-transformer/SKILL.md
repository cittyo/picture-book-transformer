---
name: picture-book-transformer
description: 将用户上传的任何角色、物体或图片转换为治愈系颗粒感日式绘本风插画（支持全平台AI自适应：具备生图能力时直接出图，纯文本环境自动输出适配Midjourney/SD的专业提示词方案）。
---

# Picture Book Transformer (Universal Agent Skill)

将输入的图片或角色提取特征后，转化为具有细腻噪点、冷压水彩纸肌理、文创手账排版风格的治愈系日式绘本插画。

## 适用场景 (When to Use)
- 用户上传了图片（角色立绘、宠物、日常物品、涂鸦草图等），要求转成绘本风、颗粒质感、蜡笔插画或日系治愈风。
- 用户直接丢图并附带“转绘本风”或类似指令。

## 视觉风格核心公式 (Style DNA)
1. **材质质感**：
- 细密噪点与颗粒喷枪效果（Dense stippling noise / Grain texture）。
- 粉蜡笔与彩色铅笔揉擦过渡（Soft crayon & colored pencil shading）。
- 冷压粗纹水彩纸底纹（Cold press watercolor paper texture）。
- 孔版印刷（Risograph）微透叠质感，杜绝光滑 3D 渲染与塑料反光。
2. **排版与细节**：
- 极简留白构图，主体饱满居中。
- 周围点缀细小杂色噪点颗粒与手绘四角星芒。
- 沿主体轮廓环绕微缩英文字符排版（Text wrapped around contour）。
- 画面底部附带 1-2 行复古打字机字体（Typewriter font）简短治愈英文文案。
3. **色彩调性**：
- 柔和温暖的对比色，避免高饱和荧光色。

## 全平台自适应执行工作流 (Workflow)

收到用户图片后，首先提取核心特征（主体、配色、服装、标志性细节、表情）。随后根据当前 AI 平台能力自动分流：

### 分支 A：当前环境
直接调用当前环境的图像生成能力输出成图，提示词核心构成：
`Children's picture book illustration style, [提取出的主体与细节描述], dense stippling noise, grainy texture, soft crayon and colored pencil shading, cold press watercolor paper texture, risograph print aesthetic, minimalist composition with ample white space, floating tiny particles and subtle sparkle stars, curved typewriter text wrapped around contour, warm healing atmosphere, retro aesthetic --ar 3:4`

### 分支 B：当前环境（如纯文本助手、代码编辑器终端）
绝对不要直接报错拒绝！请自动基于用户的图片，直接输出完整的，方便用户直接复制到 Midjourney、即梦、Stable Diffusion 等平台一键生成：
1. **主体特征分析**：简明列出提取出的核心视觉元素。
2. **Midjourney / 通用英文 Prompt**：完整的英文生图提示词（带权重与参数）。
3. **中文模型 Prompt**：适用于中文绘画工具的完整中文指令。
4. **垫图与反向提示词建议**：提供负面提示词及垫图权重说明。
