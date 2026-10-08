# JieLabVI · 杰哥 AI 实验室规范与资源库

版本 **3.0.0** · 2026-10-08。本库是当前 VI 结果交付：人可以阅读和下载；AI 可以读取规则、颜色 token、标志和模板，继续制作系统、交互、PPT、文件、海报、社交与视频。

## 从这里开始

- **人阅读**：[总体规范](docs/human/overall.md)，再按下表选择物料。
- **AI 阅读**：[AI-README.md](AI-README.md) → [总体 AI 规范](docs/ai/overall.md) → 对应任务章节。
- **机器调用**：[品牌规则 JSON](spec/brand-policy.json)、[资源清单](spec/resources.json)、[颜色 JSON](guide/ui-colors.json)。
- **视觉预览**：下载本库后打开 [index.html](index.html)；或运行 `python3 -m http.server 8781`，访问 `http://localhost:8781/`。GitHub直接渲染Markdown，HTML需本地服务打开；仓库未配置在线Pages站点。

## 按物料阅读

| 部分 | 人阅读规范 | AI 阅读规范 |
|---|---|---|
| 总体规范 | [人阅读](docs/human/overall.md) | [AI 执行](docs/ai/overall.md) |
| 标志与英文 | [人阅读](docs/human/identity.md) | [AI 执行](docs/ai/identity.md) |
| 颜色与主题 | [人阅读](docs/human/colors.md) | [AI 执行](docs/ai/colors.md) |
| 系统与产品 UI | [人阅读](docs/human/systems-ui.md) | [AI 执行](docs/ai/systems-ui.md) |
| 交互与动效 | [人阅读](docs/human/interaction.md) | [AI 执行](docs/ai/interaction.md) |
| PPT 与演示 | [人阅读](docs/human/presentations.md) | [AI 执行](docs/ai/presentations.md) |
| 文件、报告与印刷 | [人阅读](docs/human/documents.md) | [AI 执行](docs/ai/documents.md) |
| 海报制作 | [人阅读](docs/human/posters.md) | [AI 执行](docs/ai/posters.md) |
| 社交、头像与封面 | [人阅读](docs/human/social.md) | [AI 执行](docs/ai/social.md) |
| 视频、字幕与片尾 | [人阅读](docs/human/video.md) | [AI 执行](docs/ai/video.md) |
| 人物、缩略图与大图 | [人阅读](docs/human/characters.md) | [AI 执行](docs/ai/characters.md) |
| 成员与联合品牌 | [人阅读](docs/human/cobrand.md) | [AI 执行](docs/ai/cobrand.md) |

## 最重要的规则

品牌强制约束只有**颜色和 Logo**。完整中文配最长英文 **Jie's ARTIFICIAL INTELLIGENCE LAB**，紧凑独立英文 **Jie's AI Lab**，独立英文与小尺寸 **Jie Lab**。正式标志直接调用；AI 保持黄色；浅深主题按语义 token 配色。字体、布局、框架、交互、人物和辅助曲线均为可调整参考。

## 资源入口

| 文件夹 / 文件 | 用途 |
|---|---|
| `docs/human/` | 分任务的人阅读规范 |
| `docs/ai/` | 分任务的AI执行规范与任务提示 |
| `spec/` | 机器规则、资源索引与校验信息 |
| `assets/brand/` | 标志SVG/PDF/PNG、人物六款大图和缩略图、头像、正式回环 |
| `assets/fonts/` | 字体及OFL文件 |
| `assets/icons/` | 可选图标资源 |
| `assets/visuals/` | 九张生成视觉参考，不代替正式文字与token |
| `templates/` | 可编辑HTML、四页PPTX、`exports/` 中PNG与打印PDF |
| `guide/` | 23页完整规范、3页UI规范、交互配色演示、人物预览 |
| `ui/` | Ant Design主题和接入示例，依赖安装后可按原构建脚本使用 |

[人物六款尺寸与路径](assets/brand/characters.json) · [23页规范PDF](guide/brand-manual.pdf) · [UI规范PDF](guide/ui-colors.pdf) · [可编辑PPTX](templates/jie-lab-template.pptx)

## 只拿到仓库链接时如何使用

把 https://github.com/liunoly-design/JieLabVI 发给制作人员或AI，并指定任务。例如：

> 读取这个仓库的AI-README.md、总体规范和PPT章节，为杰哥AI实验室制作【主题】演示。正式调用标志和主题颜色，交付可编辑PPTX与PDF，并验证版式。

不能克隆的AI可以先读取 [AI 总入口原始文本](https://raw.githubusercontent.com/liunoly-design/JieLabVI/main/AI-README.md)，再按仓库根相对路径拼接原始文件URL。二进制资源应下载使用，不把GitHub文件预览页当图片地址。需要长期固定版本时使用Git提交SHA替代URL中的main。

## 文件性质与维护

本库包含当前结果和使用所需资源，不包含旧版包、工作截图、临时构建缓存或原始访谈资料。生成视觉页为示意；正式规则以本库总体、分任务规范、JSON token和原生资产为准。现有PDF内部保留3.0.0-review标记，仓库组织版本为3.0.0；本次只整理规则与入口，不重新改变VI视觉。

更新时同步人读、AI读和spec入口；见 [维护方法](MAINTENANCE.md)。字体许可见各OFL，品牌和人物不因公开仓库而自动获得商标或商业授权；见 [资源使用说明](USAGE.md)。
