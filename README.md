# Xufeng's Codex Skills

这个仓库一方面保存我在真实 AI 产品工作中反复使用、复盘并沉淀下来的 Skills，另一方面收录我日常工作中会使用的开源社区 Skills。它既是我的跨设备工作台，也是一套可安装、可继续迭代的 AI 产品工作方法。

## 精选 Skills

以下 5 个 Skill 最能代表我目前的工作沉淀。它们不是通用 Prompt 模板，而是从真实的信息追踪、产品判断、竞品分析、PRD 写作和研发协作中提炼出的可复用工作流。

| Skill | 它解决什么问题 | 核心产出 |
| --- | --- | --- |
| [`ai-frontier-digest`](plugins/work-derived-skills/ai-intelligence/skills/ai-frontier-digest/SKILL.md) | AI 信息很多，但二手转述、重复新闻和营销噪音让人难以形成判断 | 基于一手来源、按北京时间自然日核验的高信噪比中文图文简报 |
| [`decision-driven-competitive-analysis`](plugins/work-derived-skills/product-thinking/skills/decision-driven-competitive-analysis/SKILL.md) | 竞品研究容易变成产品清单、功能罗列和截图堆积 | 围绕待决策问题组织的竞品证据、机制比较、迁移边界与验证建议 |
| [`engineering-prd-review`](plugins/work-derived-skills/prd-writing-styles/skills/engineering-prd-review/SKILL.md) | PRD 在研发细评现场才暴露状态、边界、数据和责任问题 | 细评就绪度、研发阻塞项、责任归属和可直接补回 PRD 的规则 |
| [`prd-strategic-framing`](plugins/work-derived-skills/prd-writing-styles/skills/prd-strategic-framing/SKILL.md) | PRD 有很多需求细节，却没有讲清为什么做、为什么这样做和这期做什么 | 从背景、证据和产品判断到方案选择、阶段范围与验证逻辑的叙事链 |
| [`executive-product-judgment`](plugins/work-derived-skills/product-thinking/skills/executive-product-judgment/SKILL.md) | 团队容易停留在局部执行和正向指标，忽略最终结果、产品主线与机会成本 | 主要矛盾、价值传导断点、因果审计及继续、调整、验证或停止建议 |

## AI 产品经理的日常工作流

这部分按真实工作任务组织，不区分 Skill 是自己沉淀还是来自开源社区。它是一张按需导航图，不是每个项目都必须从头走到尾的固定流程。

### 1. 获取行业与外部信号

- `ai-frontier-digest`：扫描并核验当天真正重要的 AI 模型、产品与 Builder 一手动态。
- `follow-builders`：持续追踪 AI Builder、播客和博客内容。

### 2. 从材料中形成判断

- `signal-to-judgment`：把杂乱反馈、研究和数据转成问题、解释、证伪条件和有边界的判断。
- `executive-product-judgment`：在需求、方案、实验复盘或方向选择中识别主要矛盾、业务结果和机会成本。
- `grilling` / `grill-me`：通过逐轮追问暴露计划中的未决问题、依赖和隐含假设。

### 3. 判断一个具体需求是否值得进入方案阶段

- `product-decision-review`：在需求进入 PRD、设计或开发前，判断用户问题、受益与受损群体、证据、取舍和最短验证路径。

### 4. 用外部证据减少产品决策的不确定性

- `decision-driven-competitive-analysis`：围绕一个真实待决策问题选择样本、比较同一段用户任务，并明确竞品证据的迁移边界。

### 5. 组织方案和 PRD 的判断链

- `prd-strategic-framing`：讲清为什么做、为什么选择这种方案、本期做什么以及结果如何解释。
- `human-ai-collaboration-design`：为复杂研究、分析、规划和写作设计人机分工、检查点与最终责任。

### 6. 快速制作界面或原型

- `frontend-design`：在 Vibe Coding 中建立更明确的主题、字体、色彩和版式方向，减少模板化设计。

### 7. 在正式研发细评前补齐需求

- `engineering-prd-review`：从系统行为和实现边界检查 PRD 是否已达到可设计、可估时、可开发、可测试的程度。

### 8. 汇报、评审和推动决策

- `pyramid-communication`：把方案、复盘、报告和演示材料组织成结论先行、层级清楚的表达。

### 9. 把新的经验继续沉淀成能力

- `skill-creator`：创建、修改、评测和迭代 Skill。
- `find-skills`：先检查社区是否已有合适能力，再决定安装、适配或自己创建。

## 全部 Skills

仓库文件按来源分成两类：

```text
plugins/
├── external-skills/       # 从 GitHub 和开源社区收集或适配的 Skills
└── work-derived-skills/   # 从日常工作与真实项目复盘中沉淀的 Skills
```

### 从日常工作中沉淀

| Skill | 什么时候使用 | 它会帮助你得到什么 |
| --- | --- | --- |
| [`ai-frontier-digest`](plugins/work-derived-skills/ai-intelligence/skills/ai-frontier-digest/SKILL.md) | 系统了解今天、昨日或指定日期真正重要的 AI 动态 | 经过白名单扫描、反向查漏和原文核验的中文图文简报 |
| [`product-decision-review`](plugins/work-derived-skills/prd-writing-styles/skills/product-decision-review/SKILL.md) | 一个具体需求进入 PRD、设计或开发前 | 需求准入判断、用户分层、证据缺口、主方案和最短验证路径 |
| [`prd-strategic-framing`](plugins/work-derived-skills/prd-writing-styles/skills/prd-strategic-framing/SKILL.md) | PRD 的背景、目标、判断链、方案框架或阶段边界不清楚 | 一条解释为什么做、为什么这样做、这期做什么的战略叙事 |
| [`engineering-prd-review`](plugins/work-derived-skills/prd-writing-styles/skills/engineering-prd-review/SKILL.md) | PRD 已基本完成、正式研发细评之前 | 细评就绪度、研发阻塞项、责任边界与可直接补回 PRD 的规则 |
| [`decision-driven-competitive-analysis`](plugins/work-derived-skills/product-thinking/skills/decision-driven-competitive-analysis/SKILL.md) | 竞品研究正在滑向产品清单、功能罗列或截图堆积 | 围绕待决策问题组织的证据、机制比较和迁移边界 |
| [`executive-product-judgment`](plugins/work-derived-skills/product-thinking/skills/executive-product-judgment/SKILL.md) | 需要从业务负责人视角判断需求、方案、上线结果或模糊方向 | 主要矛盾、价值传导、因果审计、机会成本和明确决策建议 |
| [`signal-to-judgment`](plugins/work-derived-skills/thinking-workflows/skills/signal-to-judgment/SKILL.md) | 面对杂乱材料、反馈、研究或数据，难以形成核心观点 | 关键信号、竞争性解释、证伪条件和有证据边界的判断 |
| [`human-ai-collaboration-design`](plugins/work-derived-skills/thinking-workflows/skills/human-ai-collaboration-design/SKILL.md) | 与 AI 完成复杂研究、分析、方案或写作 | 人机分工、推进阶段、检查点、决策责任与成品门槛 |
| [`pyramid-communication`](plugins/work-derived-skills/pyramid-communication/skills/pyramid-communication/SKILL.md) | 汇报、方案、复盘或演示材料逻辑松散 | 结论先行、上下对应、归类清楚的沟通结构 |

### 从 GitHub 和开源社区收集

这些 Skills 用于补充通用能力。安装和对外分发前仍应分别核对原始来源、许可证、运行环境与 Codex 兼容性。

| Skill | 什么时候使用 | 它会帮助你得到什么 |
| --- | --- | --- |
| [`find-skills`](plugins/external-skills/codex-skill-workflows/skills/find-skills/SKILL.md) | 想知道是否已有可安装的 Skill 能解决当前任务 | 搜索、核验并安装合适的社区 Skill |
| [`skill-creator`](plugins/external-skills/codex-skill-workflows/skills/skill-creator/SKILL.md) | 创建、修改或评测一个 Skill | Skill 结构、触发说明、测试用例、评测结果与可安装包 |
| [`frontend-design`](plugins/external-skills/frontend-design/skills/frontend-design/SKILL.md) | 新建或重塑网页、界面和前端视觉 | 更明确的主题、字体、色彩和版式方向 |
| [`grilling`](plugins/external-skills/grilling/skills/grilling/SKILL.md) | 压力测试计划、设计或决策 | 沿决策树逐轮暴露未决问题、依赖和隐含假设 |
| [`grill-me`](plugins/external-skills/grilling/skills/grill-me/SKILL.md) | 快速启动 `grilling` | `grilling` 的快捷入口，不是独立方法 |
| [`follow-builders`](plugins/external-skills/follow-builders/skills/follow-builders/SKILL.md) | 了解 AI Builder 的近期动态与观点 | 来自 X、YouTube 和博客的主题摘要与学习要点 |

> `ambiguous-product-discovery`、`product-brainstorming` 和 `prd-completeness-review` 已迁移至私有仓库 `private-product-skills`，不包含在这个公开目录中。

## 安装与更新

将这个仓库添加为 Codex 插件市场：

```bash
codex plugin marketplace add xufeng-code/my-codex-skills
```

然后在 Codex 或 ChatGPT 桌面端的 Plugins Directory 中选择该市场，并按需安装插件。安装或升级后，新建任务以加载最新版 Skill。

更新已添加的市场：

```bash
codex plugin marketplace upgrade personal
```

查看当前市场：

```bash
codex plugin marketplace list
```
