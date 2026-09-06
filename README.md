# 我的 Codex Skills

这个仓库用于保存和跨设备安装个人 Codex 插件与 skills。

## 已包含插件

### 金字塔沟通 `pyramid-communication`

用于把中文汇报、方案、复盘、述职、周报和演示材料组织成结论先行、上下对应、归类清楚、便于决策的结构。

调用示例：

- `用 $pyramid-communication 重构这份汇报。`
- `用 $pyramid-communication 检查这份方案的逻辑。`
- `用 $pyramid-communication 把这些材料整理成 10 分钟汇报。`

### PRD 写作风格 `prd-writing-styles`

用于沉淀 PRD 写作、需求设计和评审风格，当前包含：

- `product-demand-design`：按终态反推、用户分层、上线前验证、收益/损失推演和 tradeoff 设计或评审需求。
- `luojing-prd-review`：按罗菁式完整性、边界、策略、数据和上线风险审查 PRD。
- `zijun-prd-style`：按子隽式判断链重写或评审 PRD 的背景、竞品分析和方案框架。

调用示例：

- `用 $product-demand-design 评审这份产品方案。`
- `用 $luojing-prd-review 审查这份 PRD。`
- `用 $zijun-prd-style 重写这份 PRD 的背景和方案框架。`
- `按子隽风格帮我把这些材料整理成 PRD 前半部分。`

### Codex Skill 工作流 `codex-skill-workflows`

用于把个人 Codex Skill 的本机可调用版本和 GitHub 长期版本保持同步，当前包含：

- `skill-sync-workflow`：当用户说“更新这个 skill / 同步 skill / 推到 GitHub / 检查 skill 是否一致”时，按固定流程更新本机 `~/.codex/skills` 和 GitHub 仓库。

调用示例：

- `用 $skill-sync-workflow 同步这个 skill 到本机和 GitHub。`
- `更新这个 skill，并同步到我的 GitHub skill 仓库。`
- `检查本机和 GitHub 上这个 skill 是否一致。`

### 思考与人机协作 `thinking-workflows`

用于从零散信息形成有证据边界的判断，并组织人与 AI 分阶段完成复杂认知任务，当前包含：

- `think-deeper`：识别变化、差异、矛盾与断点，建立竞争性解释和证伪条件，形成核心判断与叙事。
- `work-with-ai`：设计人机分工、阶段检查点和成品门槛，避免 AI 直接出成品后陷入反复修补。

调用示例：

- `用 $think-deeper 深挖这些零散信息，形成核心判断。`
- `用 $work-with-ai 规划这个复杂任务的人机协作过程。`
- `先和我一起想清楚，不要直接生成完整文档。`

### AI Builder 动态摘要 `follow-builders`

用于跟踪 AI 领域一线建设者在 X、YouTube 播客和博客中的最新观点，并将长内容整理成易读摘要，当前包含：

- `follow-builders`：读取集中维护的公开 feed，生成 AI 行业动态、人物观点和主题摘要。

调用示例：

- `用 $follow-builders 看看最近 AI builders 在关注什么。`
- `用 $follow-builders 总结最新一期 AI 行业动态。`
- `运行 /ai。`

## 跨设备使用

将整个仓库发布到 GitHub。每台电脑在 Codex 中添加这个仓库对应的插件市场，然后安装需要的插件。安装或升级后，请新建任务以加载最新版技能。
