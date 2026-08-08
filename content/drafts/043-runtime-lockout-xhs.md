# 小红书 Draft #043

**主题**：Google 同时开源 Agent Skills 仓库和关停 10 万星 Gemini CLI——你依赖的东西从来不开源
**平台**：小红书
**状态**：v1
**日期**：2026-06-11
**时效锚点**：2026年6月10日 Google 在 GitHub 发布 Agent Skills 仓库（开源）；6月18日 Gemini CLI 永久关停，闭源 Antigravity CLI 取代；TechTimes 5月29日、VPSMAC 6月3日报道开发者定性为 bait-and-switch
**钩子类型**：C 反共识自白式——"我以前以为 X，现在不这么想了"，认知翻转

---

## 标题候选
A. Google 同一天开源了 Skills，关掉了 10 万星的 Gemini CLI
B. 10 万颗星、6000 个 PR——然后被关掉，代码进了闭源产品
C. 开源的不是你依赖的东西，你依赖的东西从来不开源

---

## 正文

我以前以为，一个开源项目有 10 万 GitHub 星和 6000 个社区 PR，就是安全的技术依赖。Google 上周证明这个判断错了。

6 月 10 日，Google 在 GitHub 上发布了一个 Agent Skills 仓库——BigQuery、Firebase、Cloud Run、GKE 的 Agent 技能，Apache 协议，Claude Code 和 Cursor 都能用。同一天，倒计时开始：8 天后的 6 月 18 日，Google 关掉 Gemini CLI。

Gemini CLI 是 Google 2025 年 6 月开源的 AI 编码 Agent。Apache 2.0，TypeScript，一年内社区贡献了超过 6000 个合并 PR。然后 Google 把它关掉了。替代者是 Antigravity CLI——闭源，Go 语言二进制，不公开源码。速率限制从每天 1000 次请求降为每周配额。GitHub 迁移 Issue 24 小时内收到 143 个反对票，4 个支持票。开发者直接命名了这件事：bait-and-switch。

两件事放在一起看才有意义。Skills 仓库开源，是因为 Skills 是外围——它定义 Agent 在 Google 产品上"能做什么"。Antigravity CLI 闭源，是因为运行时是控制平面——它决定 Agent"怎么跑"：速率、计费、遥测、弃用周期。控制了运行时，Skills 再开源也不影响大局——你的 Agent 只能在它的规则里运行。

这是一个标准的平台捕获剧本，只是时间轴压缩到一年以内。先开源，积累社区贡献和生态依赖。路径锁定形成后，关掉开源版本，把 6000 个 PR 的社区劳动成果整合进闭源产品。原贡献者对此没有任何控制。

我在一家做 AI 产品的公司工作过，直接经历过类似的依赖决策。团队对 CLI 工具的路径依赖往往比对底层模型更深——模型可以换，改几个参数的事，但 CLI 工具嵌入的是工作流、配置文件、CI/CD 管线。一旦 Gemini CLI 的插件和自动化脚本渗透进开发流程，切换成本远比换一个模型高。

这件事对所有依赖 AI 开发工具的团队有一个直接推论：**你的技术依赖至少要分两类——模型依赖和运行时依赖。** 开放权重模型（Gemma、Llama）的风险低，模型不会被关掉，权重在你手里。闭源运行时的风险高——供应商一个商业决策就能在 30 天内终止你的整条工具链。

Google 在 Agent 层做的事，是它在 Cloud 层做过的事情的精确复刻。Cloud 开放了很多 API 和 SDK，但 GKE、BigQuery、Cloud SQL 的运行时全是 Google 控制的。Antigravity 是 Agent 时代的 Google Cloud。Skills 是 Agent 时代的 Cloud SDK。结构一模一样。

**开源的永远是外围能力，闭源的永远是控制平面。** 判断一个 AI 工具的依赖风险，不要看它有没有开源组件——看它的运行时在谁手里。你现在用的 AI 开发工具，运行时归谁控制？

---

## 封面方案

**风格**：延续极简高级感
- 主视觉：左右对比结构——左侧一个 GitHub 仓库卡片（标注 "google/skills · Apache 2.0 · OPEN"，绿色边框），右侧一个被划掉的仓库卡片（标注 "google/gemini-cli · 100K stars · 6000 PRs · CLOSED"，红色叉号）。中间用一条虚线连接，虚线上标注 "same day"
- 主标题（大字）：外围开源，控制面闭合
- 副标题：Google Agent 生态的平台捕获剧本
- 角标小字：GitHub · 2026/06/10

## 内页配图建议（图文笔记 3-4 页）

1. **Page 1（封面）**：标题 + 左右对比视觉
2. **Page 2**：核心事实卡片——「6/10 Google 开源 Agent Skills 仓库（BigQuery · Firebase · Cloud Run · GKE） / 6/18 关停 Gemini CLI（2025年6月开源 · Apache 2.0 · 10万星 · 6000+ 社区 PR） / 替代者 Antigravity CLI：闭源 · Go 二进制 · 速率从每天1000次→每周配额 / GitHub 迁移 Issue：143 反对 vs 4 支持」
3. **Page 3**：结构拆解卡片——上方「Skills 仓库（外围）」标注"定义 Agent 能做什么 → 开源"，下方「Antigravity CLI（控制平面）」标注"决定 Agent 怎么跑 → 闭源"，中间标注：「控制了运行时，Skills 再开源也不影响大局」
4. **Page 4**：结尾金句——「你的技术依赖至少要分两类 / 模型依赖（权重在你手里）→ 低风险 / 运行时依赖（供应商控制）→ 高风险 / 开源的永远是外围能力 / 闭源的永远是控制平面」

## 标签

#AI #Google #GeminiCLI #开源 #Agent经济 #科技洞察 #产品思维 #深度思考 #人工智能 #ClaudeCode #AI开发工具 #BaitAndSwitch

## 发布策略

- 发布时间：今天（6月11日）晚 8-9 点，Skills 仓库发布次日 + 距 Gemini CLI 关停仅 7 天，双重时效窗口
- 搜索流量机会：小红书「Gemini CLI」「Google AI」「开源」「AI 开发工具」关键词因 June 18 关停日期临近将有搜索增量；「Agent Skills」为新热词
- 自评论建议：「补充一个更大的模式：Google 在 Cloud 层已经做过完全一样的事。Kubernetes 开源了（外围编排），但 GKE 运行时闭源（控制平面）。TensorFlow 开源了，但 TPU 和 Vertex AI 闭源。Android 开源了，但 GMS 闭源。每次都是同一个剧本：开源外围能力积累生态，闭源控制平面锁定依赖。Gemini CLI → Antigravity 只是最新一个案例。判断你对 Google 的依赖风险，看你用的到底是外围还是控制面。」
