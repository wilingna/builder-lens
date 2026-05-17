<div align="center">

# 🔮 Builder Lens

### AI 时代的"三镜头"翻译官 / The Three-Lens Translator for the AI Era

**Stop asking AI. Start building systems.**

[中文](#中文版) · [English](#english) · [GitHub](https://github.com/wilingna)

![status](https://img.shields.io/badge/status-v0.1.0-green) ![license](https://img.shields.io/badge/license-MIT-blue) ![built_by](https://img.shields.io/badge/built_by-wilingna-purple)

</div>

---

<a name="中文版"></a>
## 中文版

### 这是什么

Builder Lens 是一款**每日 AI 资讯解读产品**——但它不是又一个"AI 早报"。

市面上的 AI 资讯产品都在做同一件事:**把英文翻译成中文**。
Builder Lens 做的是**把"技术内容"翻译成"对你的影响"**。

每天,Builder Lens 用三个镜头审视当天最重要的 AI 进展:

- 🔬 **个体创造者镜头**——这件事对一人公司、独立开发者、AI 创业者意味着什么?
- 🏢 **企业组织镜头**——这件事对企业、HR、组织演化意味着什么?
- 👤 **个人镜头**——这件事对普通职场人的技能、职业、副业意味着什么?

每一份解读都附上**未来 1 周 / 1 月 / 1 季度的具体应对建议**。

### 为什么是我做这件事

我是会灵,50 岁,北京大学， 500 强 HR 负责人,半年前开始全力转型 AI builder。

2025 年 11 月开始自学 AI,半年内发布了 9 个 GitHub 开源项目:

| 项目 | 简介 |
|---|---|
| ai-ppt-toolkit | NotebookLM + Gemini + Gamma 三件套 |
| hermes-core | Multi-agent context routing 引擎 |
| ai-content-pipeline | 7-agent 内容生产流水线 |
| ai-decision-5steps | 5 层决策框架 |
| ai-ppt-web | Web 升级版 |
| PPTFlux | End-to-end AI presentation system |
| ai-side-hustle | AI 副业规划 |
| kpi-self-review | HR 绩效自评工具 |
| wilingna | 主宣言 repo |

**全网很难找到第二个人,同时具备这 6 项能力**:

- ✓ 看懂英文技术内容
- ✓ 理解一人公司视角(我自己就是)
- ✓ 理解企业组织视角(20+ 年 HR 一线)
- ✓ 理解中年职场人焦虑(我就是其中之一)
- ✓ 用 AI 系统自动化生产(已经发了 9 个项目)
- ✓ 长期主义沉淀者(从未停止过 ship)

Builder Lens 是这 6 项能力的产物,也是它们的最佳证明。

### 一份样本输出

> **2026.05.05 · 一条新闻 · 三个镜头**
>
> 📰 **新闻摘要**:Anthropic 发布 Managed Agents API,让多个 Claude agent 可以并行运行,各有独立 context。
>
> 🔬 **个体创造者镜头**:你的 ai-content-pipeline 之前是 7-agent 串行运行,平均出稿 8 分钟。改为 Managed Agents 并行,可以压到 90 秒以内。**这意味着你一个人一天能产出的内容量从 8 篇飙升到 50+ 篇**——单人媒体公司的可能性瞬间打开。
>
> 🏢 **企业组织镜头**:**3 类岗位会被加速重构**——(1) 初级文案/客服,1 人 + Managed Agents 顶过去 5 人; (2) 中层协调岗,因 agent 间通信不再需要人; (3) 运营岗,人变成"agent 编排师"而非执行者。HR 部门要立刻盘点的是:哪些岗位不再 headcount-bound,而是 token-budget-bound。
>
> 👤 **个人镜头**:**最危险的不是被裁,是被"没必要存在"**——你的工作如果可以被一个 prompt + 3 个 agent 替代,就该尽快重新定义自己。
>
> ⚡ **应对建议**:
> - 本周内:把 ai-content-pipeline 升级到 Managed Agents 版本
> - 本月内:给企业 HR 朋友圈做"岗位 token-budget 重审"小调研
> - 本季度内:把这条思考写成深度文章,改写英文版发 X 引爆国际共振

### 路线图

- [x] **v0.0.1** · 项目启动,核心 prompts 落地
- [ ] **v0.1.0** · MVP 跑通(端到端生成第一份完整报告)
- [ ] **v0.2.0** · Web 站点 builder-lens.wilingna.github.io 上线
- [ ] **v0.3.0** · 飞书 / 邮件 / X 自动分发管道
- [ ] **v0.4.0** · 社区共建启动(读者反馈驱动产品演化)
- [ ] **v1.0.0** · Builder Atlas 周刊上线(每周共振主题图谱)
- [ ] **v2.0.0** · 国际化英文版 / Substack 同步发布

### 项目结构

```
builder-lens/
├── README.md                  # 本文档(产品宣言)
├── prompts/                   # 三镜头核心 prompt(项目灵魂)
│   ├── topic-clustering.md    # 主题聚类
│   ├── impact-scoring.md      # 影响力评分
│   ├── lens-creator.md        # 镜头 1:个体创造者
│   ├── lens-organization.md   # 镜头 2:企业组织
│   ├── lens-personal.md       # 镜头 3:个人
│   └── action-advice.md       # 应对建议生成
├── examples/                  # 真实输出样本
└── ROADMAP.md                 # 详细开发计划
```

📌 **第一份真实 sample brief**:[examples/2026-05-17-v0.1.0-sample-brief.md](examples/2026-05-17-v0.1.0-sample-brief.md)(基于真实 feed,2026-05-17 ship)

### 致谢

本项目数据采集层 fork 自 [@zarazhangrui/follow-builders](https://github.com/zarazhangrui/follow-builders)。

zara 提供了 32 位 builder + 5 个播客的中央 feed,Builder Lens 在此之上加入了:

- ➕ 中文 AI 圈信息源(知乎 / 即刻 / 公众号)
- ➕ 主题聚类 + 影响力评分
- ➕ 三镜头并行解读(本项目灵魂)
- ➕ 应对建议生成
- ➕ Web 化分发

*Builder Lens 的 X 数据上游基于 zarazhang/follow-builders skill 构建。*

### License

MIT, 但请引用作者。

---

<a name="english"></a>
## English

### What is this

**Builder Lens** is a daily AI digest product — but not another "AI news roundup."

Most AI digest products do the same thing: **translate English into Chinese.**
Builder Lens translates **technical content into "what this means for you."**

Every day, Builder Lens examines the most important AI developments through three lenses:

- 🔬 **The Solo Creator Lens** — What does this mean for indie hackers, solo founders, AI builders?
- 🏢 **The Organizational Lens** — What does this mean for companies, HR teams, org evolution?
- 👤 **The Personal Lens** — What does this mean for ordinary professionals' skills, careers, side hustles?

Every interpretation includes **actionable advice for the next week, month, and quarter.**

### Why I'm building this

I'm Wiling (会灵), 50, Peking University, Fortune 500 HR director, and a full-time AI builder since late 2025.

I started teaching myself AI in November 2025. In six months, I shipped 9 open-source projects on GitHub.

**You won't easily find someone else with all six of these:**

- ✓ Reads English technical content fluently
- ✓ Lives the solo founder reality (I am one)
- ✓ Understands organizational dynamics (20+ years of HR practice)
- ✓ Knows the mid-career anxiety (I'm in it)
- ✓ Ships AI systems autonomously (9 projects in 6 months)
- ✓ Plays the long game (never stopped shipping)

Builder Lens is the product of those six capabilities — and the proof of them.

### Roadmap

(Same as Chinese version above.)

📌 **First sample brief**: [examples/2026-05-17-v0.1.0-sample-brief.md](examples/2026-05-17-v0.1.0-sample-brief.md) (based on real feed, shipped 2026-05-17)

### Acknowledgements

The data layer of this project is forked from [@zarazhangrui/follow-builders](https://github.com/zarazhangrui/follow-builders). zara provides the central feed of 32 builders + 5 podcasts. Builder Lens adds on top of it:

- ➕ Chinese AI ecosystem sources
- ➕ Topic clustering + impact scoring
- ➕ Three-lens parallel interpretation (the soul of this project)
- ➕ Actionable advice generation
- ➕ Web-based distribution

*Builder Lens is powered by zarazhang/follow-builders skill for upstream X data.*

### Built by

[@wilingna](https://github.com/wilingna) · 50, mid-life builder · "Stop asking AI. Start building systems."

---

<div align="center">

**乾坤未定,你我皆是黑马。**

The dust hasn't settled. We're all dark horses still.

</div>
