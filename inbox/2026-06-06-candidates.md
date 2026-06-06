---
date: 2026-06-06
status: written
selected: candidate 1 → drafts/039-pause-game-theory-xhs.md
---

# Today's Candidates

## Candidate 1: Anthropic 发布"当 AI 开始构建自身"报告，Claude 已写 80% 以上代码——Jack Clark 和 Marina Favaro 发出全球协调暂停倡议，但条件是"别人先动"（June 4）

- **Event**: 2026年6月4日，Anthropic Institute 发布报告《When AI Builds Itself》，作者为 Anthropic 联合创始人 **Jack Clark** 和研究院院长 **Marina Favaro**。核心数据披露：截至2026年5月，超过 **80% 的 Anthropic 生产代码** 由 Claude 模型编写（Claude Code 于2025年2月上线时这一比例不足10%）；Anthropic 工程师如今每季度合并代码量是2021-2025年历史均值的 **8倍**；在最复杂、最开放的工程问题上，Claude 的成功率在2026年5月达到 **76%**（六个月前上升50个百分点）。同月，Anthropic 还演示了九个并行 Claude agent 自主运行 AI 安全研究项目：累计工作 **800小时**，计算成本约 **$18,000**，恢复了目标任务 **97%** 的性能差距。政策主张：报告呼吁在"递归自我改进"阈值到达之前建立**可验证的国际协调机制**，必要时可临时暂停前沿 AI 开发——但 Anthropic 明确声明**不会单方面暂停**，只有在"所有前沿实验室在可验证条件下同步行动"时才会跟进。背景：Anthropic 同期已于6月1日向 SEC 提交机密 S-1，估值 $965B，年化营收 $47B。
- **Source**: https://www.anthropic.com/institute/recursive-self-improvement | https://fortune.com/2026/06/05/anthropic-ai-pause-development-recursive-self-improvement/ | https://siliconangle.com/2026/06/04/anthropic-calls-global-pause-ai-development-humans-lose-control/ | https://qz.com/anthropic-ai-pause-brake-pedal-coordination-labs-060526 | https://www.pymnts.com/artificial-intelligence-2/2026/anthropic-wants-a-global-ai-pause-if-everyone-else-does/
- **Timeliness**: 2天前（2026年6月4日，Anthropic Institute 官方发布）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: "我们会暂停，如果所有人都暂停。"这个条件结构是这份报告里最值得分析的东西，不是80%的代码数字。

  博弈论里有一个概念叫 Nash equilibrium（纳什均衡）：每个参与者的选择，都是在其他人选择不变的前提下自己的最优策略。Anthropic 的"条件暂停"就是一个 Nash equilibrium 解：单方面暂停 = 放弃领先地位，由一个更不安全的实验室接管；所有人同时暂停 = 保持相对竞争位置的同时建立全球协商机制。

  所以这份报告的真实内容是：**Anthropic 没有在呼吁停下来，它在呼吁建立一套让所有人同时停下来的机制，同时宣告自己是定义这套机制的人**。谁来决定"递归自我改进"的门槛在哪里？谁来负责验证"可验证条件"的可验证性？报告没有回答，但它让 Anthropic 占据了提问的位置。

  80% 代码这个数据点同样值得拆分看：这不只是"AI变强了"的信号，是 Anthropic 自己在提供**证据支持自己的主张**。如果你是一家普通 AI 应用公司，你的 Claude 用量是成本。如果你是 Anthropic，你用 Claude 写代码，然后用 Claude 研究 AI 安全，然后用这两件事共同证明"递归自我改进就在转角处"。这是一条内部一致的叙事链，也是绝大多数报道错过的闭环。

  最后一个张力：Anthropic 在同一个月提交了 $965B 估值的 IPO 申请。IPO 叙事的前提是持续高速增长；暂停倡议的前提是增长需要减速。两个叙事同时成立的唯一条件是：Anthropic 认为它能在暂停规则落地之前完成上市，而且它的竞争优势在任何暂停方案里都能保持。这不是矛盾，是战略。

- **Resonance hook**: 2026年6月4日，Anthropic 发布报告：Claude 已经写了他们80%以上的生产代码，从2025年初的不足10%。Jack Clark 和 Marina Favaro 在报告里呼吁全球协调暂停——但 Anthropic 不会单方面暂停，只有"所有人在可验证条件下同步行动"才会跟进。这是一份关于 AI 安全的呼吁，也是一个纳什均衡解：单方面停下的代价是让一个更不安全的实验室接管。暂停倡议的真正主张不是"停下"，是"我来定义停下的规则"。
- **Recommended priority**: high

---

## Candidate 2: Microsoft 发布 MAI-Thinking-1——首个完全不含 OpenAI 数据的自研推理模型，零蒸馏、独立训练，AIME 2026 达 94.5%（June 2）

- **Event**: 2026年6月2日，Microsoft Build 2026 上，微软正式发布 **MAI-Thinking-1**，这是微软有史以来第一个自研推理模型，亦是新 MAI（Microsoft AI）模型家族（共7个模型）的旗舰。关键参数：**350亿活跃参数**，稀疏混合专家架构（MoE），总参数约 **1万亿**；上下文窗口 **256K token**（足以单次处理600页文档）。训练来源：**完全从零训练，不含任何第三方模型蒸馏，包括 OpenAI 的任何模型**，数据为企业级许可数据集。基准测试：**AIME 2026 得分 94.5%**（AIME 2025 得分 97.0%）；SWE-Bench Pro 编程评测与 Claude Opus 4.6 持平；Surge 盲测人工评估中优于 Claude Sonnet 4.6。当前状态：Microsoft Foundry 私有预览。背景时间轴：2026年4月28日，微软与 OpenAI 的 Azure 独家合作协议终止；同月，微软宣布收购 Inflection AI 的模型团队；6月2日 MAI-Thinking-1 发布是微软自有模型栈的首次公开展示。
- **Source**: http://www.techtimes.com/articles/317631/20260602/microsoft-build-2026-mai-thinking-1-first-house-reasoning-model-trained-without-openai-data.htm | https://microsoft.ai/news/microsoft-build-2026-mai-keynote-transcript/ | https://www.thurrott.com/a-i/336960/build-2026-microsoft-launches-first-flagship-reasoning-ai-model-and-more | https://www.notebookcheck.net/MAI-Thinking-1-Microsoft-enters-the-advanced-reasoning-AI-race-with-its-own-from-scratch-model.1314757.0.html
- **Timeliness**: 4天前（2026年6月2日，Microsoft Build 2026 发布日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 微软过去五年最大的 AI 战略是：用 $130 亿投资获得 OpenAI 49% 的利润分配权，然后通过 Azure 把 GPT 分发给全球企业。这个模型是"AI 分销商"战略——微软不创造前沿 AI，它分发前沿 AI，并在分发环节收取利润。

  MAI-Thinking-1 是这个战略的终止信号。"零 OpenAI 蒸馏"不是技术细节，是法律和战略声明：微软建造了一个和 OpenAI 完全没有 IP 关联的模型。这意味着什么？微软可以把 MAI-Thinking-1 部署在任何 OpenAI 无法进入的场景：政府合同（OpenAI 的公司治理结构让某些政府采购复杂化）、竞争敏感的企业环境（企业不想让 OpenAI 获得其数据训练下一代模型）、以及任何 OpenAI 的 ToS 和定价不合适的场景。

  时间轴上的两件事需要放在一起看：4月28日，Azure 和 OpenAI 的独家协议终止。6月2日，MAI-Thinking-1 发布。两者相差35天。这不是巧合，是微软在 Azure 合同到期后第一时间展示"我有自己的后备"。

  对 AI 产品战略的判断：平台公司在 AI 时代不能只依赖一个外部模型供应商。微软的 MAI 战略说的是：Azure 的差异化，不应该完全来自 OpenAI 的模型，而应该来自微软自己控制的模型栈 + OpenAI 的模型 + 其他第三方模型（Anthropic、Meta Llama）。这是一个主动降低单点依赖、提升议价能力的结构性动作。对于那些在 Azure 上构建 AI 产品的团队：你现在有了一个不需要经过 OpenAI 的推理选项。这改变了你的供应商风险地图。

- **Resonance hook**: 2026年6月2日，微软在 Build 2026 发布 MAI-Thinking-1。这是微软第一个完全自研的推理模型，35B 活跃参数，AIME 2026 得分 94.5%，SWE-Bench Pro 与 Claude Opus 4.6 持平。关键细节：零 OpenAI 蒸馏——模型训练里不含任何来自 OpenAI 的数据或知识。就在35天前，微软和 OpenAI 的 Azure 独家协议刚刚终止。微软正在从"AI 分销商"变成"AI 自主生产者"。这两件事之间的距离，就是微软在 AI 时代独立战略的起点。
- **Recommended priority**: high

---

## Candidate 3: OpenAI 把"Dreaming V3"记忆系统扩展至免费用户——ChatGPT 开始在后台自动合成你的历史对话，召回率从 41.5% 涨到 82.8%（June 4）

- **Event**: 2026年6月4日，OpenAI 将 **ChatGPT Dreaming V3** 记忆架构扩展至**免费（Free）层用户**（此前仅限 Plus 和 Pro 订阅者）。技术机制：Dreaming V3 是一个后台记忆合成系统，在用户不做任何操作的前提下，持续读取其历史对话记录，自动更新记忆档案——例如，"你7月要去新加坡"会在旅行结束后自动更新为"你2026年7月去了新加坡"。精度数据：内部评估显示，**事实召回率从2024年的41.5%上升至2026年的82.8%**（约翻倍）；偏好和时效敏感类得分在70%区间。新增功能：可读的记忆摘要页面（用户可查看 ChatGPT 合成了哪些关于自己的信息）、手动添加或修正记忆的控制项、话题订阅设置。这次扩展得益于 Dreaming 计算成本降低约 **5倍**。美国 Free/Go 用户先行，国际用户和其他层级随后。
- **Source**: https://openai.com/index/chatgpt-memory-dreaming/ | https://www.techtimes.com/articles/317840/20260605/chatgpt-memory-dreaming-update-openai-rewrites-personalization-engine-limits-audit-trail.htm | https://dataconomy.com/2026/06/05/chatgpt-memory-dreaming-architecture-upgrade/ | https://en.cryptonomist.ch/2026/06/05/openai-chatgpt-dreaming-v3-memory/
- **Timeliness**: 2天前（2026年6月4日，OpenAI 官方扩展至 Free 层）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: Dreaming V3 创造的不是更好的记忆，是一种新的锁定结构。

  以前的 ChatGPT 记忆是用户主动添加的：你告诉它"我喜欢简短的回答"，它记住了。这是你在主动投资这段关系。Dreaming V3 是另一件事：ChatGPT 在**不需要你做任何事**的情况下，持续观察你的所有对话，然后自动构建一个关于你的模型。你每次开新对话，它已经知道你是谁。

  这创造了一个以前不存在的转移成本：你的 **AI 记忆**。每一次你和 ChatGPT 的对话，都在让它更了解你。你用得越久，它就越懂你。你越换不掉它——不是因为功能没有替代，而是因为从头让一个新 AI 理解你的成本太高。这不是传统意义上的数据迁移问题（你可以导出聊天记录），而是**理解的不可迁移性**：Dreaming V3 在 OpenAI 服务器上合成的那个"关于你的模型"是不能被导出的。

  从产品战略的角度：这是 OpenAI 在消费者市场建立护城河最聪明的方式，没有之一。它不靠功能壁垒（功能都可以被复制），靠的是个性化深度——而个性化深度是随时间积累的，时间本身无法被竞争对手复制。Google Calendar 锁住了你，不是因为没有其他日历软件，是因为你的所有事件都在里面。Dreaming V3 的赌注是：六个月后，ChatGPT 对你的了解程度，会变成一个真实的转移摩擦力。

  做 AI 产品的人在评估竞争格局时，不应该只看当下的模型能力比较。要问的问题是：**我的产品有没有在用户每次使用时积累一个不能被复制走的资产？** Dreaming V3 给了一个具体的答案形态。

- **Resonance hook**: 2026年6月4日，OpenAI 把 ChatGPT 的 Dreaming V3 记忆系统扩展至免费用户。这个系统不需要你做任何事——它后台读取你所有的历史对话，自动更新对你的理解。事实召回率：41.5%（2024）→ 82.8%（2026）。ChatGPT 正在悄悄构建一个关于你的模型，你可以看到摘要，但你不能把这个模型带走。你用它越久，它就越懂你。转移成本不是数据，是理解。这是 OpenAI 在消费者市场能建立的最深的护城河，因为时间本身无法被复制。
- **Recommended priority**: medium

---

## Scan summary

**Sources scanned**:
- OpenAI 官方 newsroom（openai.com/index/chatgpt-memory-dreaming/，June 4，Dreaming V3 扩展至 Free 层；releasebot.io OpenAI June 2026，chatgpt-release-notes，ChatGPT Lockdown Mode 确认为2026年2月发布超30天窗口排除；GPT-5.5-Cyber EU Action Plan，helpnetsecurity May 8，超7天窗口排除）
- TechTimes（June 5，Dreaming V3 memory audit trail 技术细节确认）
- Dataconomy + CryptoNomist（June 5，Dreaming V3 架构更新细节多方确认）
- Anthropic Institute 官方（anthropic.com/institute/recursive-self-improvement，June 4，"When AI Builds Itself" Jack Clark + Marina Favaro 报告原文）
- Fortune（June 5，Anthropic pause call 多方确认）
- SiliconAngle（June 4，Anthropic 全球暂停呼吁报道）
- QZ + PYMNTS（June 4-5，条件暂停结构分析确认）
- Microsoft AI 官方博客（microsoft.ai/news/microsoft-build-2026-mai-keynote-transcript/，June 2，MAI-Thinking-1 发布原文）
- TechTimes（June 2，MAI-Thinking-1 零 OpenAI 蒸馏条款确认）
- Thurrott + NotebookCheck + SHM Studio（June 2-3，MAI-Thinking-1 参数/基准多方确认）
- Claude Opus 4.8（anthropic.com/news/claude-opus-4-8，May 28 发布，9天前，超7天窗口排除；GitHub Changelog May 28 确认同日 GA for GitHub Copilot）
- Claude 20+ legal MCP connectors（releasebot.io Anthropic June 2026，具体日期无独立 June 3-6 精确锚点，排除）
- WWDC 2026（apple.com/newsroom，keynote 为 June 8，今天尚未开幕，排除；将在 June 8 之后扫描）
- Meta Superintelligence Labs + Alexandr Wang + Nat Friedman（CNBC，June 30 2025，超30天窗口排除）
- arXiv 2606.00133 World Models Comprehensive Survey（submitted May 28，9天前，超7天窗口；综述论文无独立产品/事件锚点，排除）
- arXiv 2606.00135 Agentic Tool-calling RL（ICML 2026 accepted；提交日期未精确确认为 June 3-6 2026，排除）
- Q2 2026 Agentic AI Funding Report（DigitalApplied，published May 1 2026，36天，超30天窗口排除）
- Karpathy（anthropic.com 加入于5月19日，已在过去候选排除记录中；无独立 June 3-6 新帖子）
- Jim Fan（Sequoia AI Ascent April 2026，超30天窗口排除；无独立 June 3-6 锚点）
- Swyx AINews（June 2026 覆盖 GPT-5.5、ChatGPT 变化，无独立 June 3-6 事件锚点，排除）
- GitHub Trending（Claude-mem 项目无独立 June 3-6 爆发事件，排除；Gemini CLI 104K stars 为持续增长无单点锚点，排除）
- HN top AI posts（June 5-6：Anthropic pause paper 为主导话题，已收录 Candidate 1；ChatGPT Dreaming 讨论已收录 Candidate 3）

**Total signals found**: 约31个评估

**Why these 3**:

- **Candidate 1（Anthropic "When AI Builds Itself"，June 4）**：时效2天，Anthropic Institute 官方 + Fortune + SiliconAngle + QZ + PYMNTS 五方来源确认；深层AI思考柱：过去3天 SELECTED 覆盖了 Apple SFI-Bench 空间功能推理（June 3，CVPR 基准论文）和 Tesla 神经世界模拟器（June 3，物理 AI 护城河）——今天角度完全不重叠："AI 是否已在实质意义上开始自我构建"是阶段性定义时刻而非工具进步；80% 代码 + 8x 工程师产出 + 97% agent 自主研究恢复率是首次披露的量化内部数据；"条件暂停 = 纳什均衡解"的博弈论框架中文媒体报道不会分析；IPO + 暂停倡议同月的结构性矛盾是 Zico 可以独家解读的张力；HIGH 优先级。

- **Candidate 2（Microsoft MAI-Thinking-1，June 2）**：时效4天（7天窗口内），TechTimes June 2 + Microsoft AI 官方博客 + Thurrott + NotebookCheck 四方来源确认；AI 产品战略柱：过去3天 SELECTED 覆盖了 Anthropic Partner Network（June 4，分发层锁定）和 ChatGPT 转化广告（June 5，消费端双激励结构）——今天角度完全不重叠："平台公司从 AI 分销商转型为 AI 自主生产者"是供应链控制层的新叙事；"零 OpenAI 蒸馏"是首次独立可验证的技术法律声明；Azure 独家协议终止（4月28日）→ MAI-Thinking-1 发布（6月2日）的35天时间轴是具体的因果证据链；中文媒体报道 Microsoft Build 但不会分析"微软降低单点依赖的战略结构"；HIGH 优先级。

- **Candidate 3（ChatGPT Dreaming V3，June 4）**：时效2天，OpenAI 官方 + TechTimes June 5 + Dataconomy + CryptoNomist 四方来源确认；组织形式变革柱：过去3天 SELECTED 覆盖了 Trump AI EO（June 4，治理形态变革）和 Windows Agent Platform（June 2，OS 用户关系重构）——今天角度完全不重叠："AI 通过后台记忆合成建立个性化锁定"是用户关系结构的演变，不是监管层或硬件层；82.8% 事实召回率 + 5x 计算成本降低是首次披露的性能和经济指标；"理解的不可迁移性"作为新型转移成本框架在中文媒体无人分析；Free 层扩展代表从付费用户到全用户的飞轮加速，时效节点清晰；MEDIUM 优先级（OpenAI 产品更新类，叙事依赖执行质量；过去5天已有两个 OpenAI 候选入选，需评估选题方向多样性）。
