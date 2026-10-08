# 维护方法

1. 更新总体与对应任务的人读和AI规范，保持必须规则只有颜色与Logo。
2. 更新正式资源与guide预览，替换资产时保持路径稳定或更新所有引用。
3. 同步spec/brand-policy.json与assets/brand/characters.json；重建spec/resources.json的文件大小、SHA256与URL。
4. 检查Markdown和HTML本地引用、人物透明通道、PDF/PPT打开、UI主题与移动端。
5. 提交一个说明具体变化的Git提交；需要固定版本时把链接中的main换成提交SHA。

机器索引记录当前结果文件；不索引自身，避免哈希循环。文档索引与资源索引分开，资源位于assets、templates、guide、ui和design-tokens文件。
