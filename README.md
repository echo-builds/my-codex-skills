# 我的 Codex Skills

这个仓库保存我使用的 Codex 插件与 Skills，并用于跨设备安装。内容按来源分成两类：来自开源社区的 Skills，以及从日常产品工作中沉淀的方法。

## 目录

```text
plugins/
├── external-skills/       # 从 GitHub 和开源社区收集的 Skills
└── work-derived-skills/   # 从日常工作与真实项目复盘中沉淀的 Skills
```

## 从 GitHub 和开源社区收集

这些 Skills 主要用于补充通用能力。我保留原始方法，并在插件层补充了适合个人工作流的说明与安装配置。

| Skill | 什么时候使用 | 它会帮助你得到什么 |
| --- | --- | --- |
| `find-skills` | 想知道是否已有可安装的 Skill 能解决当前任务时 | 搜索、核验来源与质量，并协助安装合适的 Skill |
| `skill-creator` | 创建、修改或评测一个 Skill 时 | Skill 结构、触发说明、测试用例、评测结果与可安装包 |
| `frontend-design` | 新建或重塑网页、界面和前端视觉时 | 更明确的主题、字体、色彩和版式方向，减少模板化设计 |
| `grilling` | 需要压力测试计划、设计或决策时 | 沿决策树逐轮暴露未决问题、依赖关系和隐含假设 |
| `grill-me` | 想快速启动 `grilling` 时 | `grilling` 的快捷入口，不是独立方法 |
| `follow-builders` | 想了解 AI Builder 的近期动态与观点时 | 来自 X、YouTube 和博客的主题摘要与学习要点 |

## 从日常工作中沉淀

这些 Skills 来自真实产品工作、PRD 评审、竞品分析、汇报和人机协作中的反复实践。名称描述的是可迁移的方法；具体经历与人物只作为方法来源，不作为使用前提。

| Skill | 什么时候使用 | 它会帮助你得到什么 |
| --- | --- | --- |
| `ai-frontier-digest` | 想系统了解今天、昨日或指定日期真正重要的 AI 模型、产品和 Builder 一手动态时 | 经过白名单扫描、反向查漏和原文核验的高信噪比中文图文简报 |
| `pyramid-communication` | 汇报、方案、复盘或演示材料逻辑松散时 | 结论先行、上下对应、归类清楚的沟通结构 |
| `product-decision-review` | 在需求变成 PRD 或开发计划前，判断是否值得做、为谁做以及做到什么程度时 | 产品终态、用户分层、证据、取舍、推荐方向与上线前验证方案 |
| `executive-product-judgment` | 做需求、评审方案、分析上线结果或思考模糊方向，需要补充老板/业务负责人视角时 | 主要矛盾、价值传导断点、因果审计、机会成本及继续、调整、验证或停止建议 |
| `prd-strategic-framing` | PRD 的背景、目标、结果、判断链或整体方案框架不清楚时 | 一条解释“为什么做、为什么这样做、这期做什么”的宏观叙事 |
| `engineering-prd-review` | PRD 已基本写完、正式研发细评前，需要提前发现实现歧义和工程风险时 | 细评就绪度、研发阻塞项、产品与研发责任边界、范围化简及可直接补回 PRD 的规则 |
| `decision-driven-competitive-analysis` | 竞品研究容易滑向产品清单、功能罗列或截图堆积时 | 围绕待决策问题组织证据、比较机制并明确可迁移边界 |
| `signal-to-judgment` | 面对杂乱材料、反馈、研究或数据，难以形成核心观点时 | 关键信号、竞争性解释、证伪条件、有证据边界的判断与核心叙事 |
| `human-ai-collaboration-design` | 与 AI 完成复杂研究、分析、方案或写作，且容易陷入先出成品再返工时 | 人机分工、推进阶段、检查点、决策责任与成品门槛 |

### 产品工作的使用顺序

```text
产品决策
  → product-decision-review
  → decision-driven-competitive-analysis
  → prd-strategic-framing
  → engineering-prd-review
```

这不是强制流程：根据任务所处阶段，直接调用最接近当前问题的 Skill 即可。

`executive-product-judgment` 是贯穿式判断视角，可在需求、方案、上线复盘和方向思考的任一阶段调用。


> `ambiguous-product-discovery`、`product-brainstorming` 和 `prd-completeness-review` 已迁移至私有仓库 [`private-product-skills`](https://github.com/xufeng-code/private-product-skills)。

## 跨设备使用

在 Codex 中添加这个仓库对应的插件市场，再安装需要的插件。安装或升级后，请新建任务以加载最新版 Skill。
