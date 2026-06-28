---
date: 2026-06-28
status: written
selected: candidate 2 → drafts/059-third-paradigm-xhs.md
---

# Today's Candidates

## Candidate 1: Anthropic Mythos 5 获批重新上线，Fable 5 仍封锁——美国政府首次在两款来自同一公司的 AI 模型之间划出能力分级线（June 26）

- **Event**: 2026年6月26日（周五），美国商务部长 **Howard Lutnick** 签署信函正式通知 Anthropic：允许 Anthropic 向约 **100 家美国受信机构和联邦机构**发布 **Claude Mythos 5** 模型，有效期按"受信伙伴（trusted partners）"名单管理。Lutnick 在信中写道："我已确认已有适当保障措施允许特定受信伙伴访问 Claude Mythos 5 模型"。但信函明确：**Fable 5 不在本次批准范围内**，仍维持完全封锁状态。背景：2026年6月12日，Anthropic 在政府行政指令下将 Fable 5 和 Mythos 5 同时下线，指令以"国家安全"为由，要求 Anthropic 中止"任何外国国籍人员（包括 Anthropic 外籍员工）"的访问权限——两周内约 100% 的访问能力被切断。本次部分批准历时两周谈判，Anthropic 与政府"共同处理了两款模型的相关风险"方才达成。来源：**CNBC**（2026年6月26日首发）、**CNN Business**（6月26日确认）、**NBC News**（6月26日）、**9to5Mac**（6月26日，详细信函内容）、**The Hill**（6月26日，立法背景）、**MLQ News**（6月26日，"Trusted Partner" 机制分析）、**NewsBytesApp**（6月26日，Anthropic 回应）。
- **Source**: https://www.cnbc.com/2026/06/26/us-government-anthropic-claude-mythos5-ai.html | https://www.cnn.com/2026/06/26/tech/anthropic-mythos-release | https://www.nbcnews.com/tech/tech-news/us-government-gives-anthropic-green-light-limited-re-release-mythos-5-rcna352018 | https://9to5mac.com/2026/06/26/anthropic-cleared-to-release-claude-mythos-5-to-over-100-us-institutions/ | https://thehill.com/policy/technology/5943549-anthropic-mythos-5-access/ | https://mlq.ai/news/trump-administration-lifts-mythos-5-blackout-clears-anthropic-model-for-100-us-partners/ | https://beincrypto.com/anthropic-mythos-5-export-block-lifted/
- **Timeliness**: 2 天前（2026年6月26日，CNBC 首发）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 这个"分开批准"的动作，比"批准"本身更值得分析。

  同一家公司的两个模型，政府同时下令封锁，然后只解封其中一个——这不是一个模糊的政策决定，这是政府第一次在公开记录中用"行为"而非"文字"定义了什么叫做"可管控的 AI"和"不可管控的 AI"。Mythos 5 和 Fable 5 的差别是什么？能力级别、越狱难度、网络安全用途范围、可解释性——具体哪一点让政府画了这条线，没有人公开说。但这条线已经存在了。

  这有一个直接的产品战略含义：**AI 公司现在必须设计"可分级的模型"**。不是按市场定价分层（Haiku/Sonnet/Opus），而是按政府认可的安全能力边界分层——什么能力可以出现在"受信伙伴"名单可用的版本里，什么能力只能在"完全封锁"版本里。这是新的产品架构约束，来自监管，不是来自市场。

  Anthropic 面对的处境：Mythos 5 回来了，但"受信伙伴"名单本质上是政府审批的客户白名单。Anthropic 卖的每一个 Mythos 5 访问权限，背后都有政府的隐性审批。这和 OpenAI 的 GPT-5.6"逐客户审批"机制几乎同构——两家公司同时被纳入了不同路径的政府客户管控框架。Fable 5 还没回来，意味着 Anthropic 最强的前沿模型仍然无法面向市场。两家公司的处境放在一起看：政府正在从"事后监管"转向"准入前嵌入"，两周之内，以两种完全不同的方式。

  对 AI 产品 PM 的直接信号：**当监管成为最强约束，前沿模型的"能力分级"将同时受两套逻辑驱动——一套是市场逻辑（定价/性能），一套是政府准入逻辑（哪些能力可以合规发布）。** 两套逻辑之间会出现张力：最强的模型能力，往往是监管最敏感的能力。

- **Resonance hook**: 2 天前，美国政府允许 Anthropic 重新发布 Mythos 5——给约 100 家受信机构。但 Fable 5 不在列，至今仍完全封锁。两款模型两周前被同时关停，现在只有一款回来了。政府第一次用行动（而非文字）在两款来自同一公司的 AI 模型之间划出了一条能力分级线。这条线叫什么，没有人说。但所有 AI 产品团队现在都需要理解它在哪里。
- **Recommended priority**: high

---

## Candidate 2: Karpathy 命名 LLM 的"第三次界面范式"：Claude Tag 把 AI 从个人助手变成了组织共享成员（June 23-24）

- **Event**: 2026年6月23日（周二），Anthropic 正式发布 **Claude Tag**——一款让 Claude 作为可@标记的 AI 队友嵌入 Slack 工作区的产品，面向 Claude Enterprise 和 Team 客户开放 beta。核心机制：每个 Slack 工作区有一个 **共享的 Claude 成员**（不是每人一个独立会话），任何频道成员可以 @Claude 分配任务，Claude 在线程中分阶段完成并更新进度，同时构建跨频道的组织级记忆。2026年6月24日（周三），**Andrej Karpathy**（已于5月加入 Anthropic pre-training 团队）在 X 上发帖回应 Claude Tag，提出了一个框架：这是 **"LLM 界面的第三次重大重设计（the 3rd major redesign of LLM UIUX）"**。Karpathy 的三阶段叙述：① **第一范式**：基于网页的聊天机器人（ChatGPT 网页版），个人、同步；② **第二范式**：独立应用（Claude Code、Cursor、Copilot），个人、同步；③ **第三范式**：组织内部的持久性、异步性自治实体（Claude Tag），**成员而非工具**。Karpathy 的原文："This is a new paradigm for interacting with Claude that is significantly more 'inline' with all the other human activity org-wide. Once you do all of the under the hood engineering work to make this 'just work'... Claude basically joins the team in a seamless way." X 帖子链接：x.com/karpathy/status/2069547676849557725。媒体跟进：Benzinga（6月24日）、Yahoo Tech（6月24日）、VentureBeat（6月23日，Claude Tag 发布）、TechCrunch（6月23日，Claude Tag 发布）、Bloomberg（6月23日《Anthropic Wants Claude to Be Your New Slack Coworker》）、Latent.Space AINews（《Claude Tag: Multiplayer, Proactive, Persistent Agents in Slack》）。
- **Source**: https://x.com/karpathy/status/2069547676849557725 | https://www.benzinga.com/markets/tech/26/06/60091727/andrej-karpathy-says-ai-is-no-longer-a-chatbot-its-becoming-your-teammate | https://tech.yahoo.com/ai/claude/articles/andrej-karpathy-says-ai-no-203107531.html | https://venturebeat.com/technology/anthropic-launches-claude-tag-replacing-its-slack-app-with-a-persistent-ai-teammate-that-learns-monitors-and-works-autonomously | https://techcrunch.com/2026/06/23/anthropics-claude-tag-is-learning-your-company-one-slack-message-at-a-time/ | https://www.buildfastwithai.com/blogs/anthropic-claude-tag-slack-review | https://www.latent.space/p/ainews-claude-tag-multiplayer-proactive
- **Timeliness**: 4-5 天前（Claude Tag 2026年6月23日，Karpathy X 发帖 2026年6月24日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: Karpathy 提的这个框架，值得仔细拆一下，因为它在命名一件比"Slack 集成"大得多的事情。

  第一、二范式里，AI 是你的（personal）。你有自己的 Claude 会话，自己的上下文，自己的记忆。AI 在你个人的使用范围内运作，你关掉窗口它就消失了。

  第三范式里，AI 是**我们的**（organizational）。整个团队共用一个 Claude，Claude 有自己的组织级记忆，它知道你们上周讨论了什么、两个月前的 OKR 是什么、上次客户反馈的重点是什么。它不会因为你下线而中止工作——它在 Slack 里继续存在，处理别人分配的任务，推进项目。

  这个转变有几个具体的产品和组织后果，Karpathy 没有细说但值得展开：

  **产品后果**：AI 界面从"单人对话"变成"多人协同"。谁能看到 Claude 的记忆？谁能撤销 Claude 的操作？谁在 review Claude 做出的决定？这些问题在个人 AI 工具里不存在，在组织 AI 成员里必须有答案。

  **组织后果**：当 AI 有组织级记忆时，"信息透明度"的默认设置发生了变化。你和 Claude 讨论的策略方向，可能在组织内部是可见的。AI 从"个人思考工具"变成了"组织知识基础设施的一部分"。

  **权力后果**：谁控制 Claude Tag 的权限设置，谁就在一定程度上控制了哪些信息进入了 AI 的组织级记忆。这是一个以前不存在的权力节点。

  中文职场讨论会关注"Claude 加入 Slack 了"，不会分析 Karpathy 提的这个范式转变意味着什么——AI 在组织里的存在方式，从"工具"到"成员"，需要完全重新设计协作流程、权限管理、信息治理。

- **Resonance hook**: 6月24日，Karpathy 在 X 上说：Claude Tag 是 LLM 的"第三次界面范式"。第一代是网页聊天机器人，第二代是独立 AI 应用（比如 Cursor、Claude Code），第三代——AI 成为组织里的共享成员，有组织级记忆，异步自主工作。前两代，AI 是你一个人的；第三代，AI 是整个团队的。当 AI 有了组织级记忆，一切协作流程、权限管理、信息治理，都需要重新设计。
- **Recommended priority**: high

---

## Candidate 3: Anthropic Economic Index《Cadences》报告：49% 的职业有 25%+ 任务由 AI 完成，AI 使用已发展出与人类工作节律同步的时间模式（June 26）

- **Event**: 2026年6月26日（周五），Anthropic 在官方研究页面发布 **Economic Index 第三期报告**，标题为《Cadences》（节律），正式 URL：anthropic.com/research/economic-index-june-2026-report。这是 Anthropic Economic Index 系列的 2026年6月更新，引入了更高分辨率的数据采样和来自 **约 9,700 名 Claude 用户调查问卷**的新数据（2026年4月-6月调查，链接到 5月中旬至6月初的真实使用数据）。核心数据与发现：① **49% 的职业类型中，至少有 25% 的任务由 Claude 完成**——不是少数职业，是近一半（MindStudio 2026年6月报道，标题直引 Anthropic 数据）；② **AI 使用已发展出与人类工作节律高度同步的时间模式**："工作相关查询在周末减少，但在高薪职业中减幅更小"；"早晨是新闻类查询的峰值时间"；"睡眠建议的峰值在凌晨 5 点"；"税务相关请求在申报截止日附近激增"；③ **重度 AI 用户对工作前景更乐观**：依赖 Claude 做自动化的用户报告更高工作满意度、认为 AI 会提升薪资和工作安全感；④ **早期职业阶段的担忧最集中**：在 Claude 承担最多工作量的职业里，低年资工作者对工作被替代的担忧更高。来源：Anthropic 官方研究页面（6月26日）、Blockchain News（6月26日）、MindStudio（标题《Anthropic's Economic Index Shows 49% of Jobs Already Have 25%+ of Tasks Done by Claude》）、Built In（《Anthropic's Economic Index Shows the AI Skills Gap Is Growing》，June 2026）。
- **Source**: https://www.anthropic.com/research/economic-index-june-2026-report | https://blockchain.news/news/anthropic-june-2026-economic-index | https://www.mindstudio.ai/blog/anthropic-economic-index-49-percent-jobs-25-percent-tasks-claude | https://builtin.com/articles/anthropic-economic-index-2026-ai-jobs-report
- **Timeliness**: 2 天前（2026年6月26日，Anthropic 官方发布）
- **Topic pillar**: Agent经济
- **Zico's angle**: "Cadences"（节律）这个标题不是营销词汇，是这份报告最值得分析的信号。

  AI 使用有了和人类生物节律同步的时间模式——工作日高峰、周末下降、早晨新闻、凌晨5点睡眠建议。这说明什么？它说明 AI 已经不是你"用时拿起、用完放下"的工具了。工具没有节律——自来水有节律，因为自来水是基础设施，它的使用模式跟随人类的生活模式。

  当 AI 使用出现了和人类工作作息同步的节律，它变成了基础设施，不是工具。这是一个身份转变，不是功能升级。

  49% 的职业有 25%+ 的任务由 AI 完成——这个数字是量，节律是质。量告诉你 AI 渗透了多少；质告诉你 AI 渗透到了什么深度。如果 AI 使用只是偶发的效率助推，你看不到节律；只有当 AI 嵌入了日常工作流程的每个时间节点，节律才会出现。凌晨 5 点的睡眠建议峰值更耐人寻味：这不是工作场景，这是人在最脆弱的时刻（失眠焦虑、早起担忧）转向 AI 寻求帮助。这不是 Agent 经济，这是 AI 成为人类情绪和决策基础设施的证据。

  对 Agent 经济框架：如果 49% 的职业正在让 AI 承担 25%+ 的任务，这些任务的交付链条是什么样的？人类是 delegator（委派者），AI 是 executor（执行者）。但 delegator 的技能要求完全不同——不是"会用 prompt"，是"知道把什么任务给 AI、怎么验证 AI 的结果是否正确"。这对应 Anthropic 上周那篇域知识论文的结论：域知识深度决定了 AI 委派的效率。两份数据相互印证：49% 渗透率说明 Agent 经济的基础设施已经建成；域知识论文说明谁能高效使用这个基础设施。

  中文职场讨论会停在"49% 的工作有 25% 的任务被 AI 取代了"这个层面引发焦虑，不会分析"节律出现意味着 AI 成了基础设施"这一质的转变。

- **Resonance hook**: 6月26日，Anthropic 发布了 Economic Index 最新报告，标题叫《Cadences》——节律。49% 的职业里，已有 25%+ 的任务在由 Claude 完成。更值得注意的是：AI 使用开始有了和人类工作作息同步的时间节律。周末使用量下降，早晨是新闻查询峰值，凌晨 5 点是睡眠建议峰值。工具没有节律，基础设施有节律。这份报告说的不是 AI 渗透了多少，是 AI 已经变成了什么。
- **Recommended priority**: high

---

## Scan summary

**Sources scanned**:
- Karpathy X（x.com/karpathy/status/2069547676849557725，2026年6月24日，"3rd major redesign of LLM UIUX"原文）
- Benzinga（《Andrej Karpathy Says AI Is No Longer A Chatbot—It's Becoming Your Teammate》，2026年6月24日）
- Yahoo Tech（《Andrej Karpathy Says AI Is No Longer A Chatbot—It's Becoming Your Teammate》，2026年6月24日）
- VentureBeat（《Anthropic launches Claude Tag, replacing its Slack app with a persistent AI teammate》，2026年6月23日）
- TechCrunch（《Anthropic's Claude Tag is learning your company, one Slack message at a time》，2026年6月23日）
- Bloomberg（《Anthropic Wants Claude to Be Your New Slack Coworker》，2026年6月23日）
- Latent.Space AINews（《Claude Tag: Multiplayer, Proactive, Persistent Agents in Slack》，2026年6月23日）
- BuildFastWithAI（Claude Tag review，2026年6月23日）
- DataCamp（《Claude Tag: Anthropic's AI Teammate for Slack》，2026年6月23日）
- Reworked.co（《Anthropic Brings Claude Into Slack as a Taggable AI Teammate》，2026年6月23日）
- CNBC（《Trump admin allows Anthropic to release Mythos AI model to some companies, government agencies》，2026年6月26日首发）
- CNN Business（《US government allows Anthropic limited release of AI model that sparked cybersecurity concerns》，2026年6月26日）
- NBC News（《US government gives Anthropic green light for limited re-release of Mythos 5》，2026年6月26日）
- 9to5Mac（《Anthropic cleared to release Claude Mythos 5 to over 100 US institutions》，2026年6月26日，信函内容详情）
- The Hill（《Federal government permits release of Anthropic's Mythos model to select companies》，2026年6月26日）
- MLQ News（《Trump Administration Lifts Mythos 5 Blackout》，2026年6月26日）
- BeinCrypto（《Claude Mythos 5 Cleared for 100 US Institutions: Will Fable 5 Follow?》，2026年6月26日）
- Anthropic 官方研究页面（《Economic Index report: Cadences》，2026年6月26日）
- Blockchain News（《Anthropic's Economic Index Reveals New AI Usage Trends》，2026年6月26日）
- MindStudio（《Anthropic's Economic Index Shows 49% of Jobs Already Have 25%+ of Tasks Done by Claude》，2026年6月）
- Built In（《Anthropic's Economic Index Shows the AI Skills Gap Is Growing》，2026年6月）
- OpenAI 新闻页（无独立6月27-28新事件锚点，排除）
- Jim Fan / NVIDIA GR00T（Physical Turing Test 框架为早期文章，无6月25-28新锚点，排除）
- arXiv《Agentic Software》2606.05608（6月11日，超7天窗口，排除）
- World Labs / Fei-Fei Li（世界模型分类法 6月3日，超7天，排除）
- Rhoda AI FutureVision（3月2026，超30天，排除）
- GitHub Trending（palmier-pro / OpenMontage / headroom，无清晰叙事锚点，排除）
- Karpathy LLM Wiki / idea files（病毒式传播 X 帖子，无精确 6月24-28 独立日期确认，排除）
- GPT-4.5 从 ChatGPT 下线（6月26日，功能变更类，无独立战略叙事强度，排除）
- HN top AI June 27-28（主导话题为 GPT-5.6 Sol/Terra/Luna 和 AI 安全漏洞，前者已在 6月27日候选文件完整覆盖，后者技术细节类无战略叙事锚点，排除）

**Total signals found**: 约 26 个信号评估

**Why these 3**:

- **Candidate 1（Anthropic Mythos 5 部分解封，6月26日）**：**AI产品战略柱**：过去3天 SELECTED 覆盖 深层AI思考（6月27日）、组织形式变革（6月26日）、AI协作实践（6月25日）——AI产品战略近3天最大空白（上次选中：6月24日 Jalapeño 芯片）；时效最强（2天前，CNBC+CNN+NBC News+9to5Mac+The Hill 五方以上确认）；"Mythos 5 回来了但 Fable 5 没有"这一分级解封动作在中文媒体完全停在"AI 模型批准了"的层面，无人分析政府第一次在能力级别上对两个同公司模型画线意味着什么——这是 AI 产品设计的新监管约束维度；与 Fable 5 出口管制（#053）是延续事件但角度完全独立（那篇是"封锁发生"，今天是"部分解封 + 解封逻辑意味着什么"）；**HIGH 优先级**。

- **Candidate 2（Karpathy "第三范式" / Claude Tag，6月23-24日）**：**组织形式变革柱**：过去3天 SELECTED 中此柱用于 6月26日（Alibaba 蒸馏攻击）——今日提供完全不同角度（人机协作界面的范式跃迁 vs. 法律/IP 边界）；Karpathy 是 Tier 1 来源（Anthropic pre-training 核心，深度学习一线实践者），X 帖子直接可追踪；Claude Tag 是 Anthropic 近年来最重要的界面产品转变之一，Karpathy 的框架是中文媒体完全缺失的分析层次（会报道"Claude 进了 Slack"，不会分析"AI 成为组织成员"这一身份转变的产品和治理后果）；与 Zico 的 AI 协作/组织演变框架直接对应；时效 4-5 天，在 7 天窗口内；**HIGH 优先级**。

- **Candidate 3（Anthropic Economic Index《Cadences》，6月26日）**：**Agent经济柱**：过去3天 SELECTED 中此柱用于 6月27日（OpenAI Codex 数据报告）——今日角度完全独立（"AI 使用发展出节律 = AI 变成基础设施"而非"Agent 数量增长"）；时效最强（2天前，Anthropic 官方研究发布）；"节律"发现（凌晨5点睡眠建议峰值、早晨新闻峰值、周末下降）在中文媒体完全缺席——停在"49% 的职业有 25% 任务被 AI 完成了这么可怕"的表层焦虑叙事；与 Anthropic 上周域知识论文（6月16日，#056 已发布）形成数据互证链条但视角完全不同；49% 这个数字本身有强传播势能；**HIGH 优先级**。
