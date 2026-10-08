# JieLabVI · AI 总入口

读取顺序：本文件 → [总体执行规范](docs/ai/overall.md) → [机器规则](spec/brand-policy.json) → [颜色token](guide/ui-colors.json) → [任务章节](#任务章节) → 对应正式资源。

版本3.0.0 · 2026-10-08。只拿到库链接也可开始。规则路径均相对于仓库根目录。

## 必须遵循的品牌规则

1. 颜色按使用场景调用正式 token；浅色和深色各用自己的背景、文字、行动和状态色。品牌蓝 `#2D72D9`，品牌黄 `#FFC53D`，冷白 `#F8FAFC`，深墨 `#1E293B`。浅色主要行动 `#286BCC` 配白字，深色主要行动 `#8DBAFF` 配 `#101B2D`。黄色保留给标志 AI 和少量品牌强调，不作浅底正文或主要按钮，也不能代替语义警告色。
2. 调用正式标志文件，保持比例与至少 `0.25S` 保护区（S 为头像方块边长；纯字标以对应组合头像高度为参考）。完整“杰哥 AI 实验室”组合配 **Jie's ARTIFICIAL INTELLIGENCE LAB**；紧凑独立英文用 **Jie's AI Lab**；独立英文和小尺寸用 **Jie Lab**。中英文组合左右边缘等宽对齐。中文 AI、英文 AI / ARTIFICIAL INTELLIGENCE 保持品牌黄。浅／深背景调用对应标志，复杂背景加干净底板。

字体、布局、框架、交互、人物出现、辅助曲线与模板属于参考，可按任务调整。各部分建议不能被解释成新的强制品牌限制。

## 任务章节

- [总体规范](docs/ai/overall.md)
- [标志与英文](docs/ai/identity.md)
- [颜色与主题](docs/ai/colors.md)
- [系统与产品 UI](docs/ai/systems-ui.md)
- [交互与动效](docs/ai/interaction.md)
- [PPT 与演示](docs/ai/presentations.md)
- [文件、报告与印刷](docs/ai/documents.md)
- [海报制作](docs/ai/posters.md)
- [社交、头像与封面](docs/ai/social.md)
- [视频、字幕与片尾](docs/ai/video.md)
- [人物、缩略图与大图](docs/ai/characters.md)
- [成员与联合品牌](docs/ai/cobrand.md)

## 读取与调用

- 资源清单：[spec/resources.json](spec/resources.json)，列出路径、类型、大小、SHA256和原始读取URL。人物专用索引：[assets/brand/characters.json](assets/brand/characters.json)。
- 克隆仓库后直接使用本地相对路径；仅网络访问时使用 `https://raw.githubusercontent.com/liunoly-design/JieLabVI/main/` 加路径。GitHub的 `/blob/` 页面不能作为图片src。
- 中文规则以UTF-8读取；JSON是数据，SVG/PDF/PNG/PPTX需实际工具读取或下载，不凭文件名猜测内容。
- 人物组合SVG内含位图，纯字标为轮廓矢量；模板PPT文字和形状可编辑，人物为位图。生成视觉页不作为色值、精确文字、尺寸的权威。
- 历史PDF标记3.0.0-review，当前任务规则以本总入口、docs/ai和spec为准。发生冲突先遵守本次用户任务要求，并说明与库的差异。

## 完成条件

交付目标格式和可编辑源文件；资源路径可用；Logo比例、档位与明暗主题正确；颜色语义正确；实际打开或渲染验证。交互、版式、字体和辅助图形无需逐项复制模板。
