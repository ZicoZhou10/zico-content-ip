---
date: 2026-06-10
status: pending_selection
---

# Today's Candidates

## Candidate 1: WWDC 正式宣布 Siri AI 由 Google Gemini 驱动、每年$10亿——DOJ 正在上诉法院挑战 Apple-Google $200亿/年搜索协议"垄断性"，Apple 的回应是再叠一层 AI 依赖（June 8）

- **Event**: 2026年6月8日，Apple WWDC 2026 主题演讲（Tim Cook 以 CEO 身份的最后一次 WWDC 亮相），正式发布 **Siri AI**。核心架构：Siri 的云端推理层由 **Google Gemini** 驱动——基于 Apple 与 Google 于2026年1月12日签署的战略协议，合同年值约 **$10亿**，使用一个基于 Gemini 架构的定制化 **~1.2万亿参数模型**（内部代号 Apple Foundation Models v10），通过苹果 **Private Cloud Compute** 在 **Nvidia B200 GPU / Google Cloud 基础设施**上运行（Google 合同条款：不得用 Siri 对话数据训练 Gemini）。具体功能：① 自然来回对话（不再是单轮问答）；② 跨应用实时屏幕理解（无需切换 App 直接访问 Messages / Mail / Photos）；③ 独立 Siri App（含会话历史）；④ 兼容 iPad 和 Mac。同日 MacObserver 确认：Gemini 协议同时部分替代了 Apple 与 OpenAI 此前的 ChatGPT 集成，Gemini 成为 Siri 云端推理主干。**关键反讽背景**：美国司法部（DOJ）于2026年2月提出上诉，正在联邦上诉法院挑战2025年9月维持 Apple-Google **$200亿/年搜索默认协议**的判决，主张该协议构成搜索市场垄断结构；Apple 在此期间签署的 Gemini 协议，向 Google 再增加 $10亿/年 AI 依赖。
- **Source**: https://tech-insider.org/wwdc-2026-siri-ai-gemini-deal/ | https://www.macobserver.com/news/apple-calls-its-new-assistant-siri-ai-at-wwdc-2026-gemini-partnership-now-official/ | https://www.cnbc.com/2026/06/08/apple-wwdc-2026-live-updates.html | https://news.bloomberglaw.com/legal-exchange-insights-and-commentary/google-apple-gemini-deal-underscores-techs-antitrust-catch-22 | https://moginlawllp.com/apple-iphone-google-gemini-deal-search-monopoly-antitrust-judge-mehta/
- **Timeliness**: 2天前（June 8 WWDC 官方发布；January 12 为合同签署日，June 8 为产品实体面世日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: Apple 选择 Gemini，不是因为它没有自研的尝试。

  AFM（Apple Foundation Models）是 Apple 三年内真实投入数十亿美元建立的基础模型能力——端侧的摘要、改写、轻量对话，AFM 够用。端侧之外的场景，AFM 不够。Apple 也不是没试过外包：和 OpenAI 的 ChatGPT 集成是"第三方 AI 的客人"——用户清楚知道自己在用 ChatGPT，品牌归属是 OpenAI。Gemini 协议做到了 ChatGPT 合作做不到的事：Google 的模型运行在苹果的身份认同里，用户看到的是 Siri，不是 Gemini。

  这个结果的结构含义：Apple 在 AI 前沿能力上做了一个"无法假装是战略选项"的判断——它无法在合理时间和成本范围内自建与 Gemini 同等级的云端推理能力。这是迄今为止关于 AI 能力护城河最清晰的单一数据点：拥有 $2000 亿现金储备、全球最强硬件设计团队的公司，选择花 $10亿/年买这个能力，而不是自建。

  DOJ 的上诉指向的正是这个结构——Google 和 Apple 之间的搜索协议，因为它让竞争者无法在最重要的分发渠道上挑战 Google。问题是，Apple 不需要反竞争协议来维持 Google 依赖，它需要 Google 是因为 Google 有它没有的能力。反垄断执法能拆散一笔商业合同，拆不散一个能力差距。

  这对做 AI 产品的团队的含义：**护城河不在应用层，不在集成层，在前沿训练本身**。Apple 证明了这件事——当你无法在这个层次上竞争时，你唯一的选项是付钱给能竞争的人。这个能力层的集中度，是2026年 AI 行业结构里被低估的一道墙。

- **Resonance hook**: 2026年6月8日，Apple WWDC 正式宣布 Siri AI 由 Google Gemini 驱动，每年向 Google 支付约 $10亿。同时，DOJ 在上诉法院挑战 Apple 与 Google 之间现有的 $200亿/年搜索协议，主张这是垄断结构。Apple 在 DOJ 挑战其 Google 依赖的同时，又加了一层 $10亿/年的 AI 依赖。自研三年，和 OpenAI 合作一轮，最后还是选了 Google。Apple 用它最大的产品决策说了一件事：前沿 AI 能力的护城河，不是钱能解决的。
- **Recommended priority**: high

---

## Candidate 2: Salesforce Agentforce 多 Agent 编排6月15日 GA 推送15万企业客户——Atlas 3.0 动态推理路由 + Gemini Flash + A2A + MCP，企业 Agent 从 demo 变成季度更新（June 9）

- **Event**: 2026年6月9日，**Salesforce** 宣布 **Summer '26 Release**，6月15日起分波次向全球客户推送（部分客户6月13日提前收到）。三项核心更新：① **Agentforce Multi-Agent Orchestration 从 beta 升为正式可用（GA）**——全球超 **150,000家** Salesforce 企业客户无需额外采购，在下一次系统自动更新中即可使用多 Agent 编排能力；② **Atlas Reasoning Engine 3.0** 同步发布——工作方式：当请求到来时，Atlas 读取已注册的每个 Specialist Agent 的描述和可用 Actions，**实时动态推理决定路由，不使用固定决策树**，每次都从描述重新推断；③ **Gemini 3.5 Flash 原生集成进 Atlas Reasoning Engine 3.0**，通过此前（4月22日）宣布的 Salesforce-Google Cloud 深度整合实现；④ Agent 间通信协议层：**Model Context Protocol (MCP)** 和 **Agent2Agent (A2A)** 标准双协议支持，兼容 Slack 和 Google Workspace 跨平台 Agent 协作。Salesforce 官方数据：使用 Agentforce 的企业客户平均每周自动处理案例量较去年同期增长 **340%**；Salesforce CEO **Marc Benioff** 在公告中称 Summer '26 为"the quarter autonomous agents became enterprise infrastructure"。
- **Source**: https://www.techtimes.com/articles/318085/20260609/salesforce-puts-google-gemini-35-flash-inside-agentforce-june-15-release.htm | https://chatforest.com/builders-log/salesforce-summer-26-agentforce-multi-agent-orchestration-atlas-a2a-mcp-builder-guide/ | https://www.salesforce.com/agentforce/multi-agent-orchestration/ | https://www.siroccogroup.com/agentforce-multi-agent-the-seam-problem/
- **Timeliness**: 1天前（2026年6月9日 Salesforce 官方宣布；6月15日推送至全球客户）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 6月15日是一个分界线，但分界线不在功能，在分发路径。

  OpenAI、Anthropic、Google 做多 Agent 产品，需要开发者主动选用、企业主动采购、IT 部门走采购流程。Salesforce 用的是它的季度自动推送机制——15万家企业不需要做任何决策，**在下一个 IT 维护窗口，Multi-Agent Orchestration 就出现在了他们的 Agentforce 控制台里**。这是企业 Agent 能力历史上最大的一次被动部署事件，数量级比任何单次产品发布的主动采购量都高。

  Atlas 3.0 的架构设计暴露了一个工程真相——**接缝问题（Seam Problem）**：当 Orchestrator Agent 把任务路由给 Specialist Agent 的那一刻，信息压缩不可避免地发生。Orchestrator 的完整上下文、用户的原始意图语境、当前已执行步骤的状态——这些在"交棒"的瞬间有多少能被完整传递？Atlas 3.0 的动态推理（每次从 Agent 描述重新推断路由）是在解决"选哪个 Agent"，不是在解决"传多少上下文"。接缝问题是多 Agent 系统在生产规模下第一个会暴露的结构性故障模式——不是能力问题，是信息架构问题。6月15日是这个问题第一次在企业真实生产规模上被检验的时间节点。

  Salesforce 选 Gemini 3.5 Flash 而不是 Claude Sonnet 或 GPT-4o，是一个 Agent 经济的基础设施判断：**Agent 路由决策的速度和单次调用成本，比推理深度更关键**。多 Agent 系统里，大量的调用是中间层的路由推理（"把这个子任务交给哪个专用 Agent？"），这类调用需要快速、廉价、足够准确——这是 Flash 的定位，不是 Pro 的定位。Salesforce 的模型选择，是给"Agent 经济里什么性能指标最重要"的一个来自企业侧的实际答案。

- **Resonance hook**: 6月9日，Salesforce 宣布 Summer '26 更新6月15日推送给全球15万家企业客户。亮点：Agentforce 多 Agent 编排从 beta 变成正式功能——这些企业在系统自动更新里就会多出一个多 Agent 系统，不需要任何主动采购决策。Atlas 3.0 + Gemini Flash + MCP + A2A 协议。Marc Benioff 说这是"autonomous agents 成为企业基础设施的季度"。多 Agent 的第一个真实工程问题不是"Agent 能不能干活"，是"Agent 交接任务时信息丢了多少"。6月15日，这个问题第一次在企业生产规模上被检验。
- **Recommended priority**: high

---

## Candidate 3: Uber 4个月烧完全年AI预算——内部排行榜把 token 消耗量变成考核指标，工程师采用率32%→84%，70%代码AI生成，但没人能答 COO 的问题："值得吗？"（Bloomberg June 2）

- **Event**: 2026年6月2日，**Bloomberg** 发布报道，**Uber** 已正式对员工使用 AI 编码工具设置 **$1,500/月/人** 硬性上限，并建立内部仪表板供员工追踪 token 支出；可申请豁免但需说明理由。关键数字链：① Uber **CTO Praveen Neppalli Naga** 披露：工程团队在 **4个月内消耗了2026全年的 AI 工具预算**（预算耗尽时间节点：2026年4月）；② 触发机制：Uber 内部曾设立**工程师 AI 使用量排行榜**，团队按 token 消耗量排名，直接驱动采用率从2月的 **32%** 飙升至3月的 **84%**，4月底约 **95%** 工程师已每月使用 AI 工具；③ 现状：**70%+ 的 commit 代码为 AI 生成**，但公司管理层**无法把这个数字和可度量的消费者端功能产出连接起来**；④ Naga 本人在一次内部 demo 中 2 小时内消耗了 **$1,200 的 token 费用**；⑤ **COO Andrew Macdonald** 在播客访谈中（May 2026）公开表示："很难画出一条线，从 token 消耗到我们为用户交付了什么"（"it's very hard to draw a line"）；**CEO Dara Khosrowshahi** 被问及 token 支出是否已超过雇用一名初级工程师的成本时，回答："我还没有算过，但数字很大。" 主要工具：**Claude Code**（Anthropic）和 **Cursor**。Simon Willison 于 June 3 发布独立分析《Uber Caps Usage of AI Tools Like Claude Code》。
- **Source**: https://www.bloomberg.com/news/articles/2026-06-02/uber-caps-usage-of-ai-tools-like-claude-code-to-cut-costs | https://techcrunch.com/2026/06/02/uber-caps-employee-ai-spending-after-blowing-through-budget-in-four-months/ | https://fortune.com/2026/05/26/uber-coo-ai-spending-tokens-claude-code/ | https://simonwillison.net/2026/Jun/3/uber-caps-usage/ | https://aiweekly.co/alerts/uber-exhausts-ai-budget-as-claude-code-hits-84
- **Timeliness**: 8天前（Bloomberg June 2 首发；7天窗口边缘，但 Fortune May 26 首漏、Simon Willison June 3 独立确认，事件持续有新分析）
- **Topic pillar**: AI 协作实践
- **Zico's angle**: $1,500 的上限是一个管理工具，但它暴露的是一个度量问题，而不是预算问题。

  Uber 的内部排行榜是一个教科书级的 Goodhart 定律案例：**当 token 消耗量成为考核指标，token 消耗量就不再是好的指标**。排行榜让工程师有激励最大化 token 使用，而不是最大化 token 的价值输出。采用率从 32% 到 84% 在一个月内完成，这个速度不是 AI 工具价值被验证的速度，是游戏排行榜规则的速度。

  COO Andrew Macdonald 的问题不是一个管理问题，是一个产品度量架构问题。软件工程的价值创造主要在质量维度：写的代码对不对、设计得好不好、bug 少不少、系统稳定度有没有提升。这些质量维度的改善，在"代码行数"或"commit 数量"这类传统工程效率框架里是看不见的。70% 的 commit 是 AI 生成——这个数字描述的是 AI 的参与度，不是 AI 的贡献质量。"没有办法画线"，是因为 Uber 在用错误的数轴。

  Uber 不会是最后一家问这个问题的公司。$1,500 的月上限会被广泛模仿——不是因为它是正确答案，而是因为它是管理成本的唯一可执行抓手，在你没有价值度量框架的时候。在组织里推 AI 落地的产品团队，现在做的事应该包含两件：让团队用工具，以及同时建立"这个工具生产了什么价值"的度量框架。如果你没有后者，Uber COO 的问题早晚会落在你头上。

- **Resonance hook**: Uber 在4个月内烧完了2026全年的 AI 工具预算。内部曾有一个按 token 消耗量给工程团队排名的排行榜，Claude Code 和 Cursor 的工程师采用率从32%涨到84%用了一个月。70%的提交代码现在是 AI 生成的。然后 Uber COO 公开问了一句：这值得吗？Bloomberg June 2 披露，Uber 随即给每人设了 $1,500/月的上限。CEO Dara Khosrowshahi 被问到 token 钱够不够雇一个工程师，他说："我还没算过。" 用排行榜驱动 AI 采用，最后得到的是一个 token 消耗问题，而不是一个生产力答案。
- **Recommended priority**: medium

---

## Scan summary

**Sources scanned:**
- CNBC（June 8，WWDC 2026 live；Siri AI + Gemini 合作官方确认）
- tech-insider.org（"WWDC 2026: Siri AI Runs on Google's $1B Gemini Deal"；合同金额 + 技术架构）
- MacObserver（June 8，"Apple Calls New Assistant 'Siri AI' at WWDC 2026, Gemini Partnership Now Official"）
- Business Standard（June 9，WWDC Siri AI Gemini 报道，独立确认）
- Bloomberg Law（"Google–Apple Gemini Deal Underscores Tech's Antitrust Catch-22"；DOJ 上诉背景）
- Mogin Law LLP（"Isn't the Apple–Google Deal Exactly What Judge Mehta's Antitrust Opinion Was About?"；法律结构分析）
- The Antitrust Attorney Blog（May 14，"Apple's Gemini-Siri Deal Is the Next Microsoft Antitrust Case"；独立法律视角）
- ChatForest（"Apple Picks Google Gemini to Power Siri — The Deal Reshaping the AI Industry"；AFM 能力局限分析）
- TechTimes（June 9，"Salesforce Puts Google Gemini 3.5 Flash Inside Agentforce in June 15 Release"；原始报道）
- ChatForest（Salesforce Summer '26 multi-agent orchestration：Atlas 3.0, A2A, MCP 详细技术分析）
- Sirocco Group（"Agentforce Multi-Agent: The Seam Problem"；接缝问题工程分析）
- Salesforce.com 官方（Agentforce Multi-Agent Orchestration 产品页）
- Salesforce Engineering Blog（"Inside the Brain of Agentforce: Revealing the Atlas Reasoning Engine"）
- Bloomberg（June 2，"Uber Caps Usage of AI Tools Like Claude Code to Cut Costs"；原始报道）
- TechCrunch（June 2，"Uber caps employee AI spending after blowing through budget in 4 months"）
- Fortune（May 26，"Uber COO says it's getting harder to justify the company's AI spend"；COO 原话 + 内部 leaderboard 细节）
- Simon Willison（June 3，"Uber Caps Usage of AI Tools Like Claude Code"；独立社区分析）
- AI Weekly（"Uber Exhausts AI Budget as Claude Code Hits 84%"；采用率数字确认）
- TechStartups.com（June 9 top news；全局信号扫描）
- llm-stats.com（June 2026 LLM updates；模型发布动态）
- TechTimes（June 5，"Gemini-Powered Apple Siri Will Run on Nvidia B200 Chips via Google Cloud"；基础设施细节）
- TechTimes（June 6，"Google Gemini 3.5 Pro Nears June Launch With 2 Million Token Context And Deep Think Reasoning"；背景扫描）
- Claude Opus 4.8（May 28 发布，超7天窗口，排除）
- Gemini 3.5 Pro GA（6月内，尚无精确 June 7-10 发布日期锚点，排除）
- White House AI Executive Order（June 2，8天前；边界，但 Candidate 3 Uber 有更具体的企业级叙事锚点，EO 优先级降低，排除）
- NVIDIA Vera CPU / Agent Toolkit（June 1-2，已在 June 3 inbox 全面覆盖为 Candidate 1，排除重复）
- Anthropic S-1 IPO 机密申请（June 1，已在 June 3 inbox 全面覆盖为 Candidate 2，排除重复）
- Karpathy June 2026 posts（无独立 June 7-10 新帖可追溯锚点，排除）
- Jim Fan / Demis Hassabis June posts（无独立 June 7-10 事件锚点，排除）
- OpenAI Economic Research Exchange（June 9，信号偏弱、缺乏独立深度叙事空间，排除）
- arXiv June 7-10（无具备 June 7-10 精确提交日期且具备独立叙事强度的单篇突破论文，排除）
- Bulletin of Atomic Scientists "AGI's ETA Delayed"（June 2026，无精确发布日期锚点，排除）
- ARC-AGI-3（March 25 发布，超30天窗口，排除）

**Total signals found**: 约35个评估

**Why these 3:**

- **Candidate 1（Apple Siri AI = Gemini 正式发布，June 8）**：时效2天，tech-insider + MacObserver + CNBC + Business Standard + Bloomberg Law 五方来源确认；AI 产品战略柱：June 7 inbox 已覆盖 Apple iOS 27 Extensions（AI OS 平台战略 + ChatGPT 独家地位终结）——今天角度完全不重叠：DOJ 上诉挑战 Google-Apple 搜索协议的同时 Apple 再叠 AI 依赖，以及 Apple 自研能力局限的战略告白；"前沿 AI 能力护城河让反垄断执法追不上" 的论点在中文媒体几乎缺失；HIGH 优先级。

- **Candidate 2（Salesforce Agentforce Summer '26 GA，June 9）**：时效1天，TechTimes June 9 + Salesforce 官方 + ChatForest 技术分析 + Sirocco Group 三方独立确认；Agent 经济柱：过去3天 SELECTED 未覆盖此柱（June 8 Codex 为最近一次，已过7天）——今天是多 Agent 编排从 beta 到 GA 的企业被动部署事件；15万家客户自动更新是任何主动采购不可及的分发规模；接缝问题是工程视角的新锚点；中文媒体几乎不报道 Salesforce Agentforce 技术细节，信息差极大；HIGH 优先级。

- **Candidate 3（Uber AI 预算耗尽 + $1,500 上限，Bloomberg June 2）**：时效8天（窗口边界），Bloomberg + TechCrunch + Fortune + Simon Willison 四方来源确认；AI 协作实践柱：过去3天 SELECTED 未覆盖此柱；Uber 内部排行榜游戏化 token 消耗是 Goodhart 定律的典型案例、COO "Is it worth it" 是企业 AI ROI 质疑首个有名有姓的公开叙事；过去3天 June 3 inbox 仅将 Uber 5000 工程师作为 Anthropic 营收增长的数据点，本次作为独立主候选；"排行榜制造采用率而非价值" 角度在中文媒体几乎缺失；MEDIUM 优先级（时效略旧，但内部排行榜机制 + COO 原话数字足够强）。
