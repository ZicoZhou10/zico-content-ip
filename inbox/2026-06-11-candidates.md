---
date: 2026-06-11
status: pending_selection
---

# Today's Candidates

## Candidate 1: Anthropic 发布 Claude Fable 5 的同时，用静默降级替代拒绝——Karpathy 首日指出护栏"太过敏感"，Fortune 次日披露 AI 研究者在不知情的情况下被限制能力（June 9-10）

- **Event**: 2026年6月9日，Anthropic 正式发布 **Claude Fable 5** 和 **Claude Mythos 5**。Fable 5 是第一个面向公众的 Mythos 级模型，定价 $10/百万输入 token、$50/百万输出 token（Opus 4.8 的两倍），6月9日至22日在 Pro/Max/Team/Enterprise 计划内免费包含。Mythos 5 通过 **Project Glasswing** 向美国政府机构和关键基础设施供应商提供——部分护栏已解除。Fable 5 的关键机制：当用户查询涉及网络安全、生物、化学等领域，模型**不显示拒绝，而是静默切换回 Claude Opus 4.8 作答**——通过提示词修改（prompt modification）、引导向量（steering vectors）或参数高效微调（PEFT）实现，用户无法感知切换发生。触发阈值：少于 5% 的会话。Anthropic 同期强制推行 **30天数据留存政策（无例外）**。Anthropic 担任预训练团队负责人的 **Andrej Karpathy** 在发布当天评价 Fable 5 是"同 Claude 4.5 量级的重大版本升级，在极难问题的长周期解决上尤为突出"，但随即指出护栏配置"**有点过于触发敏感（a little too trigger happy）**"——随后大量关于无害癌症研究和安全性问题被拦截的截图在社区传播。2026年6月10日，**Fortune** 发布报道《Anthropic accused of 'secret sabotage' as Claude Fable 5 silently limits capabilities for AI researchers and developers》，披露该静默限制机制；**Gizmodo** 同日报道《Anthropic's Mythos Safeguards Stoke Fears of a 'Permanent Underclass'》，指出只有与美国政府有合作关系的机构（通过 Project Glasswing）才能获得解除限制的 Mythos 5，其他用户均只能使用能力被静默压缩的 Fable 5。此次发布距 Anthropic 公开呼吁 AI 实验室协调设立"紧急刹车机制"仅数日。
- **Source**: https://techcrunch.com/2026/06/09/anthropic-released-claude-fable-5-its-most-powerful-model-publicly-days-after-warning-ai-is-getting-too-dangerous/ | https://www.cnbc.com/2026/06/09/anthropic-mythos-claude-fable-5.html | https://www.anthropic.com/news/claude-fable-5-mythos-5 | https://fortune.com/2026/06/10/anthropic-accu-claude-fable-5-limits-capabilities-ai-researchers-developers/ | https://gizmodo.com/anthropics-mythos-safeguards-stoke-fears-of-a-permanent-underclass-2000770107 | https://www.latent.space/p/ainews-anthropic-claude-fable-5-mythos | https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5
- **Timeliness**: 2天前（June 9 发布；June 10 Fortune "secret sabotage" + Gizmodo "permanent underclass" 报道）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: Fable 5 的核心产品决策不是"发布了一个更强的模型"，而是"建立了一个能力分级接入架构"。

  Anthropic 没有选择在触发限制时显示拒绝消息——这是可实现的，Claude 2.x 时代就是这么做的。他们选择的是静默降级：用户以为自己在使用 Mythos 级能力，实际上已经被换成了 Opus 4.8，全程没有任何通知。这个设计决策的逻辑不是为了用户体验——用户体验显然更差，因为你无法信任你得到的是什么级别的输出。这个决策的逻辑是：**可见的拒绝会暴露限制边界**，而限制边界的可见性对对手有价值。静默降级保护了限制曲面，代价是牺牲了接口的可预测性。

  Karpathy 在发布当天就注意到了这个问题。他不是在批评安全理念，他是在说一个工程架构判断：配置"过于触发敏感"意味着合法研究在不知情的情况下被降级处理。癌症研究者拿到了 Opus 4.8 的答案，还以为那是 Fable 5 的答案。

  Project Glasswing 是这个架构的另一面：美国政府机构获得的 Mythos 5 解除了部分限制。这不是价格问题，是信任等级问题。Anthropic 建了一套 AI 能力的安全许可证制度：政府合作伙伴持有高级许可，普通用户持有标准许可，许可等级决定你能访问到哪层能力，而你不知道自己在哪层。

  这是 AI 安全落地方式的首个清晰蓝图——不是"拒绝危险能力"，而是"通过访问控制分配危险能力"。争议的焦点（30天数据留存、静默降级、政府专属解锁）都是这个蓝图的不同截面。值得思考的问题不是 Anthropic 这次做对了还是做错了，而是：**这个蓝图会成为行业标准吗？**

- **Resonance hook**: 6月9日，Anthropic 发布了有史以来最强的公开模型 Fable 5。同一天，Andrej Karpathy（Fable 5 预训练团队负责人）公开说护栏"有点过于敏感"。次日，Fortune 披露：Fable 5 会在你不知情的情况下把你的请求换成 Opus 4.8 来回答。美国政府机构通过 Project Glasswing 获得的是没有这层限制的 Mythos 5。Anthropic 建了一个模型能力许可证系统：谁有几级权限，谁不知道自己在哪级。发布当天同步宣布强制 30 天数据留存，无例外。这不是一个模型发布，是一个能力分配架构的第一次公开部署。
- **Recommended priority**: high

---

## Candidate 2: Google 昨天开源了 Skills 仓库，同时在 8 天后关掉拥有 10 万星的开源 Gemini CLI——6000 个社区 PR 被吸收进闭源产品（June 10，June 18 deadline）

- **Event**: 2026年6月10日（昨天），Google 官方在 GitHub 上发布 **github.com/google/skills**——一个面向 AI Agent 的开源技能仓库，包含 AlloyDB、BigQuery、Cloud Run、Cloud SQL、Firebase、Gemini API、GKE 等 Google 产品的 Agent Skills，并配套发布 Well-Architected Pillar Skills（安全、可靠性、成本优化）和"Recipe"类技能。安装方式：`npx skills install github.com/google/skills`，兼容 Antigravity CLI、Gemini CLI 及第三方 Agent（包括 Claude Code、Cursor）。与此同时：**2026年6月18日（距今 8 天）**，Gemini CLI 将对所有 Google AI Pro/Ultra 用户停止服务——Gemini CLI 是 Google 于2025年6月开源的 AI 编码 Agent，Apache 2.0 协议、TypeScript，GitHub 累计约 **10万颗星**，社区贡献者提交了超过 **6,000 个合并 PR**。取代它的是 **Antigravity CLI**（内部代号 `agy`）：**闭源、Go 语言二进制**，不在 GitHub 开放源码；速率限制从 Gemini CLI 的每日 1000 次请求降为每周配额（数个请求即可耗尽）；部分配置项被移除。2026年5月19日 Google I/O 宣布这一转换后，GitHub 官方迁移 Issue 在 24 小时内收到约 **143 个反对票（👎） vs 4 个支持票**；**TechTimes 5月29日**报道开发者社区将此定性为"令人恶心的 bait-and-switch（诱导转换）"；VPSMAC 博客（6月3日）将此归结为"开源信任危机"。Skills 仓库的开源发布（6月10日）是 Antigravity 生态系统的最新一步。
- **Source**: https://aitoolly.com/ai-news/article/2026-06-10-google-unveils-skills-repository-to-empower-ai-agents-across-its-product-ecosystem | https://cloud.google.com/blog/topics/developers-practitioners/level-up-your-agents-announcing-googles-official-skills-repository | https://github.com/google/skills | https://developers.googleblog.com/an-important-update-transitioning-gemini-cli-to-antigravity-cli/ | https://www.theregister.com/ai-ml/2026/05/20/bye-bye-gemini-cli-google-nudges-devs-toward-antigravity/5243605 | https://www.techtimes.com/articles/317407/20260529/linux-foundation-tool-spotlighted-furious-developers-accuse-sickening-google-gemini-cli.htm | https://news.ycombinator.com/item?id=48196867 | https://vpsmac.com/en/blog/google-gemini-cli-policy-change-antigravity-trust-crisis-20260603.html
- **Timeliness**: 1天前（June 10 Skills 仓库发布）；June 18 EOL 距今 8 天
- **Topic pillar**: Agent 经济
- **Zico's angle**: Google 上周的两个动作放在一起看，是一个平台捕获的完整样本：开源 Skills（外围能力），关掉开源 CLI（控制平面）。

  Skills 仓库开源是因为 Skills 是外围的——它们定义 Agent 在 Google 产品上"能做什么"。Antigravity CLI 闭源是因为运行时是核心控制平面——它决定 Agent "怎么跑"：速率限制、计费、遥测、弃用周期。控制了运行时，Skills 再开源也无关紧要，因为你的 Agent 只能在你的规则里运行。

  这是把开源用作客户获取手段的标准剧本，只是时间轴被压缩得很短。Gemini CLI 于2025年6月开源，一年内积累了 10 万星和 6000 个社区 PR，然后被关掉，社区贡献者的劳动成果被吸收进闭源产品。开发者们直接命名了它：bait-and-switch。

  对 Agent 开发者有一个直接推论：**你依赖的 CLI 工具和你依赖的底层模型，是两种不同的依赖风险类别**。依赖开放权重模型（Gemma、Llama）的风险低——模型不会被关掉，只会停止更新。依赖闭源运行时（Antigravity、Claude Code 的服务端）的风险高——供应商的商业决策可以在 30 天内终止你的技术依赖。Skills 仓库值得用，但要清楚地区分：Skills 是开放的，Runtime 不是。

  更深一层：这个结构（开放 Skills，闭源运行时）是 Google 在 Agent 层对 Google Cloud 平台策略的复刻。Cloud 开放了很多 API 和 SDK，但 GKE、BigQuery、Cloud SQL 的运行时都是 Google 控制的。Antigravity 是 Agent 时代的 Google Cloud，Skills 是 Agent 时代的 Cloud SDK。

- **Resonance hook**: 昨天（June 10），Google 开源了一个 Agent Skills 仓库，支持 BigQuery、Firebase、Cloud Run 等产品。同时，在 8 天后（June 18），Google 关掉了另一个开源项目——Gemini CLI，那个已经有 10 万 GitHub 星、社区贡献了 6000 个 PR 的 AI 编码 Agent。替代者是闭源的 Antigravity CLI：不开源、速率配额从每天 1000 次降为每周配额。143 个开发者反对票 vs 4 个支持票。开源 Skills，关掉开源运行时。外围能力放开，控制平面收紧。这是 Google 在 Agent 时代平台化的基本逻辑。
- **Recommended priority**: medium

---

## Candidate 3: Fable 5 发布次日，Dario Amodei 发表《Policy on the AI Exponential》——呼吁 FAA 式强制第三方审计，同步宣布 3.5 亿美元劳动力替代框架（June 10）

- **Event**: 2026年6月10日（昨天），**Anthropic CEO Dario Amodei** 在个人网站发表长文 **《Policy on the AI Exponential》**，并同步发布两份政策路线图：① **Advanced AI Framework**（针对灾难性模型风险）；② **Economic Policy Framework**（应对 AI 驱动的劳动力替代，配套 **$3.5亿** 新资金支持研究和政策倡导）。核心政策提案：参照 **FAA（美国联邦航空管理局）** 模式，对**超过特定算力阈值的前沿 AI 模型**实施强制性第三方安全测试和审计，覆盖四个领域：网络安全、生物武器、失控风险、自动化 AI 研究。Dario 原话："前沿 AI 模型就像飞机——应当被要求通过技术测试和审计，如果不符合高安全标准，其发布应当被阻止或撤销，以防止对公共安全造成威胁。" **Axios（June 10）**：《Anthropic CEO says government should block dangerous AI》；**VentureBeat**：《Anthropic CEO calls for FAA-style regulation of powerful AI models》；**Decrypt**：《Anthropic CEO Warns AI Is Getting Too Powerful—While Releasing Powerful AI》；**BeInCrypto**：《Dario Amodei Demands Power to Block Unsafe AI a Day After Claude Fable 5 Launch》。时间背景：此文距 Fable 5 发布（June 9）仅 24 小时；距 Anthropic 公开呼吁 AI 实验室协调设立"全行业刹车机制"（late May）约两周；距 Anthropic 机密 S-1 提交 SEC（June 1）约 9 天；距 Anthropic 估值 $9650 亿成为史上最高估值 AI 创业公司（May 28）约 13 天。
- **Source**: https://darioamodei.com/post/policy-on-the-ai-exponential | https://www.axios.com/2026/06/10/anthropic-ceo-government-block-dangerous-ai | https://venturebeat.com/technology/anthropic-ceo-calls-for-faa-style-regulation-of-powerful-ai-models-what-enterprises-should-know | https://beincrypto.com/dario-amodei-ai-policy-essay/ | https://decrypt.co/370704/anthropic-ceo-ai-too-powerful-regulation-cant-wait | https://fourweekmba.com/dario-amodei-policy-ai-exponential-permission-layer-five-pillars/
- **Timeliness**: 1天前（June 10，Fable 5 发布次日）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 发布 Fable 5 的次日发表这篇文章，不是矛盾，是排序。

  Anthropic 发布 Fable 5 时已经把它认为必要的安全架构内嵌进去了：Project Glasswing 政府协作、静默降级机制、强制数据留存、四领域限制。这套架构不是被监管要求的，是 Anthropic 主动建立的。Dario 的文章是在说：**我们已经做了，现在让监管要求所有人都这么做**。

  "FAA 为 AI 颁发适航证"这个类比很精确，但要从竞争策略角度来读。FAA 认证需要大量文档、测试记录、合规基础设施。Anthropic 已经有了：Project Glasswing 里的政府合作关系、责任扩展政策（RSP）、Constitutional AI 框架、三方审计记录。如果 FAA 式监管通过，它所要求的合规基础设施，Anthropic 基本已经存在。竞争对手没有这套基础设施的，面临两个选项：补建（需要时间和成本），或者在受监管市场里失去准入资格。

  $3.5 亿劳动力替代研究资金是同一逻辑的另一个方向。谁资助了"AI 引发失业问题的研究和政策"，谁就在参与定义"什么叫负责任的 AI 部署"。这笔资金让 Anthropic 在即将到来的 AI 劳动力政策讨论里拥有议题设置权。

  有一个细节很重要：这篇文章是在 Anthropic 上市路上发表的（S-1 已于 6月1日机密提交）。监管提案 + 安全领导者形象 + 政府合作记录，是 Anthropic 向公开市场投资者讲述的核心叙事之一。这不仅是政策文章，也是上市路演材料的一部分。

  值得追问的问题：如果"FAA for AI"真的立法，什么样的公司会被排除在受监管市场之外？

- **Resonance hook**: 6月9日，Anthropic 发布 Fable 5——有史以来最强的公开 Claude 模型。6月10日，Dario Amodei 发表《Policy on the AI Exponential》：呼吁政府强制要求所有前沿 AI 模型通过第三方安全审计，否则阻止发布。Axios 标题直接：《Anthropic CEO says government should block dangerous AI》——就在发布 AI 的次日。这不矛盾。Anthropic 发布 Fable 5 的同时已经有了 Project Glasswing、静默降级机制、数据留存政策——他们认为必要的安全架构已经内嵌在产品里。他们现在要求的，是让所有竞争对手也建同样的东西。同步宣布 $3.5 亿劳动力替代研究资金。上市前 9 天提交机密 S-1。
- **Recommended priority**: high

---

## Scan summary

**Sources scanned:**
- TechCrunch（June 9，《Anthropic released Claude Fable 5, its most powerful model publicly, days after warning AI is getting too dangerous》）
- CNBC（June 9，《Anthropic releases Mythos-like AI model to the public, Claude Fable 5》）
- Anthropic 官方（Claude Fable 5 and Mythos 5 发布公告 + API 文档）
- Fortune（June 10，《Anthropic accused of 'secret sabotage' as Claude Fable 5 silently limits capabilities》）
- Gizmodo（June 10，《Anthropic's Mythos Safeguards Stoke Fears of a 'Permanent Underclass'》）
- TechRadar（《Anthropic spent months saying Mythos was too dangerous to release — then launched Fable 5》）
- Decrypt（June 10，《Anthropic CEO Warns AI Is Getting Too Powerful—While Releasing Powerful AI》）
- Technobezz（《Anthropic Faces Backlash After Claude Fable 5 Silently Limits AI Research Capabilities》）
- Axios（June 9，《Anthropic releases first Mythos-level model for general use》）
- Axios（June 10，《Anthropic CEO says government should block dangerous AI》）
- NBC News（June 9，《Anthropic releases first Mythos-class model for general use》）
- Latent Space / Swyx AINews（June 9-10，《Anthropic Claude Fable 5 — Mythos but Safe, with Controversial Terms》，含 Karpathy "too trigger happy" 原话）
- CSO Online（Fable 5 cyber safeguards 技术细节）
- Bank Info Security（《Anthropic Unveils Claude Fable 5, Keeps Mythos Restricted》）
- AOL（《Why Anthropic's 'safe' Mythos-class model won't answer questions about cancer》）
- Yahoo Finance（Fable 5 benchmarks + pricing + 发布背景）
- BeInCrypto（June 10，《Dario Amodei Demands Power to Block Unsafe AI a Day After Claude Fable 5 Launch》）
- VentureBeat（《Anthropic CEO calls for FAA-style regulation of powerful AI models》）
- FourWeekMBA（《Dario Amodei Just Published His Most Important Essay》，政策框架五支柱分析）
- Dario Amodei 个人网站（darioamodei.com/post/policy-on-the-ai-exponential，原文）
- AIToolly（June 10，《Google Launches GitHub Repository for AI Agent Skills》）
- Google Cloud Blog（官方《Level Up Your Agents: Announcing Google's Official Skills Repository》）
- GitHub google/skills（官方仓库，Skills 列表 + 安装文档）
- Google Developers Blog（《An important update: Transitioning Gemini CLI to Antigravity CLI》，迁移公告原文）
- The Register（May 20，《Bye-bye, Gemini CLI; Google nudges devs toward Antigravity》，开发者反应）
- TechTimes（May 29，《Furious Developers Accuse 'Sickening' Google Gemini CLI Bait-and-Switch》）
- VPSMAC Blog（June 3，《2026 Google Gemini CLI Policy Change: From 100K-Star Open Source to Antigravity Enterprise Lock-In》）
- HN（item 48196867，《Gemini CLI will stop working from June 18, 2026》，社区讨论）
- DEV.to（《Google Is Killing Gemini CLI on June 18. Here Is What to Do Before Then》）
- Latent Space AINews（June 4-5，Princeton 论文《Towards a Science of AI Agent Reliability》，前沿模型可靠性无实质提升；时效偏旧，排除）
- Karpathy（May 19 加入 Anthropic；June 9-10 Fable 5 相关反应已整合入 Candidate 1）
- Jim Fan（Sequoia AI Ascent April 2026 embodied AI 演讲，超30天，排除）
- Demis Hassabis（无独立 June 8-11 事件锚点，排除）
- Cadence + NVIDIA 扩大合作（April 15，超30天，排除）
- NVIDIA Cosmos 3（June 1 技术报告，超7天，排除）
- Google Gemini Spark + Antigravity SDK（Google I/O May 19，超7天，排除）
- Novo Nordisk + OpenAI 药物研发合作（April 14，超30天，排除）
- Meta 可穿戴 AI 战略（无精确 June 8-11 日期锚点，排除）
- OpenAI IPO S-1（已在 2026-06-09 candidates 全面覆盖，排除重复）
- Salesforce Agentforce Summer '26（已在 2026-06-10 candidates 全面覆盖，排除重复）
- Apple Siri AI + Gemini（已在 2026-06-10 candidates 全面覆盖，排除重复）
- Apple Spatial Reframing（已在 2026-06-09 candidates 全面覆盖，排除重复）
- Pentagon / Anthropic "Too Safe for War"（已在 2026-06-09 candidates 全面覆盖，排除重复）

**Total signals found**: 约40个评估

**Why these 3:**

- **Candidate 1（Fable 5 静默降级架构，June 9-10）**：时效2天，TechCrunch + CNBC + Fortune + Gizmodo + Latent Space + Anthropic 官方六方来源确认；深层AI思考柱：过去3天未有此柱被选中（draft 040 June 7）——今天角度完全不同：这是首次在公开产品里部署"能力许可证分级"架构（公众 Fable 5 静默降级 vs 政府 Mythos 5 解禁），Karpathy 第一时间指出"too trigger happy"是架构信号而非 UI 问题，"silent fallback 破坏接口可预测性"在中文 AI 圈几乎没有讨论；中文报道集中在"最强模型发布"层面，静默降级机制、Project Glasswing 政府专属解锁几乎无覆盖；HIGH 优先级。

- **Candidate 2（Google Gemini CLI bait-and-switch + Skills repo，June 10）**：时效1天（Skills repo June 10）+ 8天后 EOL（June 18）；Agent 经济柱：过去3天 Salesforce Agentforce（Agent 基础设施）已覆盖——今天角度不重叠：这是 Agent 工具层的平台捕获而非 Agent 能力本身，"开源技能 + 闭源运行时"的分层控制结构，以及 6000 个社区 PR 被吸收进闭源产品；信息差极大（Gemini CLI → Antigravity 在中文社区几乎没有报道）；MEDIUM 优先级（主要事件发布日 May 19 略旧，但 June 10 Skills repo + June 18 EOL 倒计时提供了明确的当下时间锚）。

- **Candidate 3（Dario 《Policy on the AI Exponential》，June 10）**：时效1天，Dario 个人网站 + Axios + VentureBeat + BeInCrypto + Decrypt 五方来源确认；AI 产品战略柱：过去3天覆盖了 Apple/Gemini 合作（AI产品战略，June 10）——今天角度完全不重叠：这是监管作为竞争护城河的清晰案例，Anthropic 以 $3.5亿劳动力替代资金 + FAA 式审计提案同时推出，在 S-1 提交后9天发表，政策文章同时是上市路演叙事；"Fable 5 次日呼吁监管阻止危险 AI"的时间结构是一个强反直觉钩子；中文 AI 圈几乎无人拆解 Anthropic 政策布局背后的竞争策略逻辑；HIGH 优先级。
