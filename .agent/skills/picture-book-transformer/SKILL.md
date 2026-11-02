name: picture-book-transformer
description: 将用户上传的任何角色、物体或图片一键重绘为治愈系颗粒感日式绘本风插画。使用场景包括：用户上传图片并要求转成绘本风、颗粒质感、蜡笔插画、日式治愈插画，或直接丢图要求转换特定画风。
Picture Book Transformer
将输入的图片或角色提取特征后，直接重绘为具有细腻噪点、冷压水彩纸肌理、文创手账排版风格的治愈系日式绘本插画。

适用场景 (When to Use)
用户上传了图片（角色立绘、宠物、日常物品、涂鸦草图等），希望转换为绘本插画。

用户要求添加“颗粒感”、“粉蜡笔揉擦”、“Risograph 印刷感”或“日系治愈绘本风”。

视觉风格公式 (Style Formula)
材质质感：

细密噪点与颗粒喷枪效果（Dense stippling noise / Grain texture）。

粉蜡笔与彩色铅笔揉擦过渡（Soft crayon & colored pencil shading）。

冷压粗纹水彩纸底纹（Cold press watercolor paper texture）。

孔版印刷（Risograph）微透叠质感，杜绝光滑 3D 渲染与塑料反光。

排版与细节：

极简留白构图，主体饱满居中。

周围点缀细小杂色噪点颗粒与手绘四角星芒。

沿主体轮廓环绕微缩英文字符排版（Text wrapped around contour）。

画面底部附带 1-2 行复古打字机字体（Typewriter font）简短治愈英文文案。

色彩调性：

柔和温暖的对比色，避免高饱和荧光色。

工作流 (Workflow)
分析输入图片中的核心特征（造型、主色调、配饰、表情）。

调用绘图工具生成图像，提示词模板如下：
Children's picture book illustration style, [主体特征描述], dense stippling noise, grainy texture, soft crayon and colored pencil shading, cold press watercolor paper texture, risograph print aesthetic, minimalist composition with ample white space, floating tiny particles and subtle sparkle stars, curved typewriter text wrapped around contour, warm healing atmosphere, retro aesthetic --ar 3:4

输出结果并保留原作的核心辨识特征。
