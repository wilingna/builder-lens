# Builder Lens · ROADMAP

## 当前版本: v0.1.0

> 2026-05-17 · v0.1.0 ship 完成 · 第一份基于真实 feed 的 sample brief 落地 · 编辑红线 + 工程纪律落地

---

## v0.1.0 · MVP 跑通(已完成 ✅ 2026-05-17)

**定义**: 端到端跑通一次,生成第一份完整的 Builder Lens 报告

### 任务清单

- [x] 主题聚类 + 影响力评分(Plan B 路线:由 Claude Code runtime 在会话中即时完成,无独立 prompt 文件)
- [x] 集成 zarazhang 的 follow-builders skill(通过 Claude Code skills 加载 feed-x.json)
- [x] 第一份完整 sample brief → 归档到 `examples/`
- [ ] 录一条 5 分钟"Builder Lens 是什么"短视频(B 站 / 视频号)—— **可选 · 不卡 ship**

### 关键产出

- `examples/2026-05-17-v0.1.0-sample-brief.md` —— 第一份基于真实 feed 的 sample brief
- `prompts/editorial-rules.md` —— 编辑红线 + 写作规范 + 工程纪律
- `CLAUDE.md` —— 项目根目录工作规则,新会话入口
- **三镜头读者画像 + 应对建议可二元自检** 范式确立

### 决策记录

原计划写 `scripts/generate-brief.js` 自动化主流程。Plan B 决定:**Claude Code 做 runtime**,prompts/ 是知识资产、brief 通过 Claude Code 会话生成,不需要独立脚本。

---

## v0.2.0 · 数据源升级与新鲜度

**定义**: 让 Builder Lens 从"X 推文聚合 + 静态快照"升级为"多源 + 定期刷新 + 可信"

### 任务清单

- [ ] 接入至少 1 个深度内容源(候选:Every RSS / Lenny's Podcast transcript / Substack 聚合)
- [ ] follow-builders skill 加定时刷新机制(至少每周一次)
- [ ] `examples/` 里所有 brief 必须标明数据时间戳(由 `editorial-rules.md` 第五节强制)
- [ ] NO-FABRICATION 自检报告标准化(可校验 / 可回归测试)

### 关键产出

第一份真正的"实时多源 brief",**数据时间戳 ≤ 7 天**

---

## v0.3.0 · Web 化

**定义**: 从命令行升级到网页可读

### 任务清单

- [ ] Next.js 静态站点搭建
- [ ] 部署到 GitHub Pages: builder-lens.wilingna.github.io
- [ ] 每日 markdown 自动转 HTML 页面
- [ ] RSS feed 生成
- [ ] 邮件订阅(免费层)

### 关键产出

builder-lens.wilingna.github.io —— 首个公开访问的 Builder Lens 站点

---

## v0.4.0 · 自动分发

**定义**: 多渠道自动推送

### 任务清单

- [ ] 飞书 webhook 集成
- [ ] X / Twitter 自动发推(英文版)
- [ ] 视频号 / B 站短视频自动生成脚本
- [ ] 小红书图文自动生成

### 关键决策

- 飞书走 OpenClaw 还是自写 webhook?
- X 自动发还是半手动审核后发?

---

## v0.5.0 · 社区共建启动

**定义**: 让真实读者反馈驱动产品演化

### 任务清单

- [ ] 14 天免费日报投放,收集真实读者反馈
- [ ] 私信调研 5 个高互动读者:他们最想看什么镜头?最想看哪类主题?
- [ ] 在私域社群 100+ 人投放,看哪几条转发 / 收藏最高
- [ ] 沉淀第一批 case study(读者真实使用场景)
- [ ] 录 B 站长视频:《Builder Lens 第一个月,读者教我的 5 件事》

### 关键产出

第一批 50 位真实读者 + 至少 10 条具体反馈

---

## v1.0.0 · Builder Atlas 上线

**定义**: 每周共振主题图谱

### 任务清单

- [ ] 主题共振算法(谁引用谁、谁回应谁)
- [ ] D3.js 交互式 SVG 渲染
- [ ] 周刊形式发布
- [ ] 季度演化报告

---

## v2.0.0 · 国际化

**定义**: 英文版同步发布,打开北美市场

### 任务清单

- [ ] Substack / X 英文版同步发布
- [ ] 英文版 prompt 微调
- [ ] Product Hunt 上架(寻求第一波国际声量)
- [ ] 申请 TEDx 演讲(基于 Builder Lens 的故事)

---

## 长期愿景(2027+)

- 成为"AI 时代中文世界最权威的影响力翻译产品"
- 沉淀为《AI 时代的组织重构》课程产品
- 建立深度共建的真实读者社区
- 完成 TED 主舞台演讲

> **乾坤未定,你我皆是黑马。**

---

## 度量指标

| 阶段 | 关键指标 | 目标 |
|---|---|---|
| v0.1 | sample brief 完整性 | ✅ 三镜头 + 应对建议齐全 + 红线落地 |
| v0.2 | 数据新鲜度 | 数据时间戳 ≤ 7 天 |
| v0.3 | Web 站点流量 | 首月 1000 PV |
| v0.4 | 多渠道触达 | 5 个渠道并行 |
| v0.5 | 真实读者反馈 | 50 位读者 / 10 条具体反馈 |
| v1.0 | 用户留存 | 每周回访率 ≥ 40% |
| v2.0 | 国际声量 | X 英文账号 1000 粉丝 |

---

*Last updated: 2026-05-17*
