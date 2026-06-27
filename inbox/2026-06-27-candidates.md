---
date: 2026-06-27
status: pending_selection
---

# Today's Candidates

## Candidate 1: OpenAI 发布《Agentic AI 证据报告》：法务和招聘团队用 Codex 做主力 AI 工具，99 分位用户每天生成 60+ 小时 Agent 任务（June 25-26）

- **Event**: 2026年6月25日，OpenAI 同步在官网和 arXiv（论文编号 2606.26959v1）发布研究报告《The Shift to Agentic AI: Evidence from Codex》，以及关联博客《How agents are transforming work》（6月26日）。核心数据：① 研究类 Agent 使用量相比 2025年11月上涨 **56倍**，客服类上涨 32倍，工程类上涨 27倍；② **非开发者个人用户自 2025年8月起增长 137倍**，非开发者企业用户增长 189倍；③ **99 分位用户每天生成超过 60 小时的 Codex Agent 执行轮次**，分布在多个并行 Agent 上；④ Codex 已成为 **OpenAI 内部所有团队的主力 AI 工具**，包括法务（Legal）和招聘（Recruiting）等非技术团队——即非技术团队也放弃了对话式 AI，全面转向 Agent；⑤ OpenAI 内部员工的 Codex 使用量占所有 AI 输出 token 的 **85% 以上**；⑥ 近 25% 的 Codex 请求对应的任务需要人类 **超过 1 小时才能完成**。报告明确表述：**"Chat 时代已经结束（The chat era is over）"**。数据基于 OpenAI 真实内部使用数据，不是问卷也不是用户访谈。
- **Source**: https://openai.com/index/how-agents-are-transforming-work/ | https://arxiv.org/html/2606.26959v1 | https://www.techtimes.com/articles/319114/20260626/agentic-ai-reaches-lawyers-recruiters-openai-data-shows-137-fold-non-dev-growth.htm | https://fourweekmba.com/openai-agents-60-hours-day-codex-85-percent/ | https://thenextweb.com/news/openai-codex-agents-shift-employees-non-developers
- **Timeliness**: 1-2 天前（OpenAI 官方 arXiv 2026年6月25日；博客 2026年6月26日）
- **Topic pillar**: Agent经济
- **Zico's angle**: 这份报告的核心信号不是"Agent 增长了多少倍"，而是**谁在用、用来做什么**。

  法务和招聘团队把 Codex 当成了主力 AI 工具。他们不是在用 Agent 写代码，是在用 Agent 处理原本需要数小时的知识工作——合同审查、候选人匹配、政策梳理。Agent 越过了"辅助编程"这个早期叙事，开始成为通用知识工作的基础设施。

  60 小时/天这个数字更值得仔细想。99 分位用户每天管理的 Agent 执行时间，相当于一个 7.5 人团队同时全天工作。这些人不再是在"提问"，而是在**管理一个 Agent 项目组合**——批量下发任务，异步等结果，审核并合并输出。他们和 AI 的关系已经从"用户↔助手"变成了"PM↔多人并行执行"。

  这个模式转变，让几乎所有现有 AI 产品的设计假设失效：单轮延迟（秒级响应足够吗？）、单任务执行（队列管理需要 UI 吗？）、单一批准点（谁来 review 60 小时的 Agent 输出？）。

  对 Zico 的 Agent 经济框架：这份数据是第一次用真实内部数据验证了"人类角色从执行者变成调度者"的预测。不是论文里的设想，是 OpenAI 内部 2025年8月至 2026年6月真实发生的事。Agent 经济的基础设施问题——**怎么让一个不懂代码的招聘总监每天有效管理 60 小时的 Agent 工作量**——才刚刚被提出来。

- **Resonance hook**: 6月26日，OpenAI 公布了一份内部数据报告。法务和招聘团队现在把 Codex 当成主力 AI 工具，不是工程团队——是法务和招聘。非开发者用户在10个月里增长了137倍。99分位用户每天生成超过 60 小时的 Agent 任务，靠并行 Agent 同时跑。OpenAI 在报告里说：Chat 时代已经结束。这不是预测，是他们自己员工使用数据的结论。
- **Recommended priority**: high

---

## Candidate 2: 白宫要求 OpenAI "逐客户审批" GPT-5.6 访问权限——政府首次介入前沿 AI 的发布流程，对比 Anthropic Fable 5 的强制下线（June 25-26）

- **Event**: 2026年6月25日，CNN Business 独家报道：**特朗普政府（Trump administration）正式向 OpenAI 提出请求**，要求 OpenAI 将 GPT-5.6 的发布限制在一批经政府审批的合作伙伴范围内，理由是该模型的"先进能力和国家安全影响"。6月26日，OpenAI 同步在官网发布 GPT-5.6 预览版（OpenAI 官方页面：《Previewing GPT-5.6 Sol》），以三款分层模型形式推出：① **GPT-5.6 Sol**（最强，针对复杂编程和安全研究，定价 $5/$30 per 1M token）；② **GPT-5.6 Terra**（均衡，针对高频企业任务，$2.50/$15）；③ **GPT-5.6 Luna**（快速低成本，日常摘要/起草，$1/$6）。初始访问仅开放约 **20 个组织**，均经过政府逐一审批。Sam Altman 对员工表示："政府将在预览期逐客户审批访问权限（the government would approve access customer by customer during this preview period）"。CNBC（6月26日）和 VentureBeat（6月26日）多方确认。背景对比：**2026年6月12日，特朗普政府以不同方式对 Anthropic 出手**——强制 Anthropic 在 90 分钟内将 Fable 5 和 Mythos 5 完全下线（#053 已分析）。同是政府管控，Anthropic 是被动关停，OpenAI 是主动协商分级发布。
- **Source**: https://www.cnn.com/2026/06/25/tech/openai-limit-release-white-house | https://openai.com/index/previewing-gpt-5-6-sol/ | https://www.cnbc.com/2026/06/26/openai-limits-new-ai-models-to-trusted-partners-request-us-government.html | https://venturebeat.com/technology/openai-unveils-gpt-5-6-sol-terra-and-luna-models-but-only-accessible-to-limited-preview-partners-for-now-per-us-gov | https://www.axios.com/2026/06/26/openai-gpt-sol-terra-luna-trump
- **Timeliness**: 1-2 天前（CNN Business 2026年6月25日首发；OpenAI 官方 + CNBC + VentureBeat 2026年6月26日确认）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 把 6月12日和 6月25-26日放在一起看：美国政府连续两次介入前沿 AI 模型的发布——Anthropic 被关停，OpenAI 被要求分级发布。但处理方式完全不同，结果也完全不同。

  Anthropic 被动：Fable 5 越狱事件发生后，政府下令 90 分钟关停，Fable 5 和 Mythos 至今仍不可用。OpenAI 主动：GPT-5.6 在发布前已与白宫协商，政府得到了"逐客户审批"的控制节点，OpenAI 得到了"可以发布，只是发布给谁由我说了算"的结果。

  这不只是公关差异，是**与监管者建立关系结构的先后顺序问题**。OpenAI 先把政府纳入了发布流程，变成了"共同管控者"；Anthropic 面对的是"事后监管者"的强制命令。两种角色，权力结构完全不同。

  从产品战略层，这创造了一个新的产品决策维度：**你的前沿模型，要在什么时候、以什么方式，让政府进入发布决策链条？** 不进，你面对的是被动关停；进得早，你保留发布权，政府只拿审批权。Altman 的"逐客户审批"机制把政府变成了 OpenAI 的 KYC 合规外包——政府批准，OpenAI 收钱，审批风险转移。

  Sol/Terra/Luna 的三层定价（$5/$30 → $2.50/$15 → $1/$6）本身也值得一看：这是 Anthropic Haiku/Sonnet/Opus 三层结构的 OpenAI 版本。前沿模型市场的分层结构已经成为行业标准——不只是技术分层，是市场细分和定价权的主动设计。

- **Resonance hook**: 6月25日，CNN Business：白宫要求 OpenAI 把 GPT-5.6 的访问权限限制在政府审批的合作伙伴里，且逐客户审批。6月26日，OpenAI 发布了三款分层模型（Sol/Terra/Luna），初始约 20 个机构能用。两周前，同一个政府强制 Anthropic 在 90 分钟内关停 Fable 5 和 Mythos——至今未恢复。都是政府管控，但处理方式不同：Anthropic 是事后强制关停，OpenAI 是事前协商分级发布。结果也不同：一个模型还在线，一个至今下线。
- **Recommended priority**: high

---

## Candidate 3: 科技九巨头六月蒸发 $2.7 万亿市值——$7250 亿年度 AI 资本开支遇上 3% 家庭付费率（June 2026 ongoing, peak June 27）

- **Event**: 2026年6月，Apple、Microsoft、Google/Alphabet、Amazon、Nvidia、Meta、Broadcom、Oracle、Tesla 九家公司合计市值蒸发约 **$2.7 万亿**（2.7 trillion USD），为 AI 热潮以来最大单月跌幅。核心数字：① 2026年四大超大规模云服务商（Microsoft、Alphabet、Amazon、Meta）预计 AI 相关资本开支达 **$7250 亿**，同比 2025年的 $4100 亿上涨 **77%**；② Goldman Sachs 预测至 2030财年，四大 hyperscaler 累计 AI 资本开支将达 **$5.3 万亿**；③ 与此形成对比的是：**目前仅约 3% 的美国家庭为任何 AI 服务付费**（来源：Yahoo Finance 引用分析师数据，June 27）；④ 典型触发事件：Alphabet 单日市值蒸发约 **$2250 亿**，股价当日跌 5%，创 2026年2月以来最大单日跌幅；⑤ Yahoo Finance 于 6月27日以《Big Tech's $2.7 Trillion AI Bill Comes Due》为题作为"Chart of the Day"专项分析，成为今日科技媒体最广传播的数据故事。来源：Yahoo Finance（6月27日）、Startup Fortune（6月27日，《Big Tech has lost $2.7 trillion in market value this month as investors question whether AI can pay for itself》）、Knowledge Hub Media、AOL Finance。
- **Source**: https://finance.yahoo.com/markets/article/big-techs-27-trillion-ai-bill-comes-due-chart-of-the-day-100000100.html | https://startupfortune.com/big-tech-has-lost-27-trillion-in-market-value-this-month-as-investors-question-whether-ai-can-pay-for-itself/ | https://knowledgehubmedia.com/big-techs-2-7-trillion-ai-reckoning-what-investors-need-to-know/
- **Timeliness**: 今日（2026年6月27日，Yahoo Finance Chart of the Day）；6月全月积累市场事件
- **Topic pillar**: 深层AI思考
- **Zico's angle**: $7250 亿年度资本开支，和 3% 付费家庭渗透率，这两个数字不能同时成立太久。

  $7250 亿是 2026年四大超大规模云服务商的 AI 资本开支预测，这个数字比瑞士全年 GDP 还高。但今天为 AI 付费的美国家庭只有 3%。数学很简单：如果按美国 1.3 亿个家庭，3% 大约是 390 万个付费用户，每人 $20/月 × 12 = $240/年 → 全年约 $9.4 亿消费端收入，和 $7250 亿 capex 之间有约 800 倍的差距。

  这里有一个重要的结构分析：**市场对"AI 板块"的整体定价，混淆了价值链上两种完全不同的商业模式**。Nvidia 卖芯片、超大规模云服务商卖算力，他们的 capex 是为了获取长期算力市场地位，预期收益在 3-5 年；OpenAI/Anthropic 卖 token，他们的收益在订阅合同周期（月度/年度）。市场在 6月把这两类都作为"AI 交易"卖出——但他们的底层商业模式和时间跨度根本不同。蒸发的 $2.7 万亿，很大程度上是市场把短期软件估值逻辑（快速变现）错误地应用在了基础设施投资逻辑（长周期）上。

  LeCun 六月上旬说"投资人在补贴用户"——$2.7 万亿的市值蒸发是市场开始同意这个判断。但和 LeCun 的结论不同：这不一定是泡沫爆炸，更可能是**基础设施周期的正常估值调整**——电力网络、铁路、互联网基础设施在早期都经历了超前资本投入和短期市场修正，长期最终被证明是对的。AI capex 是不是同一个故事，2026年不知道。但市场卖出的逻辑是错的：它在问"这笔钱今年能赚回来吗"，但这个问题对基础设施投资根本不是正确的评估框架。

- **Resonance hook**: 今天，Yahoo Finance 把 6月科技股市值蒸发做成了 Chart of the Day：九家公司单月合计蒸发 $2.7 万亿。同月，四大超大规模云服务商的 AI 年度资本开支预计达 $7250 亿，同比上涨 77%。而目前为任何 AI 服务付费的美国家庭只有 3%。投资者的问题是：这笔钱能赚回来吗？这个问题问错了。AI capex 是基础设施投资，不是软件投资。问题应该是：这个基础设施，在谁的手里变成了护城河？
- **Recommended priority**: high

---

## Scan summary

**Sources scanned**:
- OpenAI 官方博客（《How agents are transforming work》，2026年6月26日）
- OpenAI 官方 arXiv（《The Shift to Agentic AI: Evidence from Codex》，2606.26959v1，2026年6月25日）
- OpenAI 官方预览页面（《Previewing GPT-5.6 Sol》，2026年6月26日）
- TechTimes（《Agentic AI Reaches Lawyers and Recruiters: OpenAI Data Shows 137-Fold Non-Dev Growth》，2026年6月26日）
- FourWeekMBA（《OpenAI Data: Top Users Generate 60 Hours of Agent Work Per Day》，2026年6月26日）
- The Next Web（《OpenAI says 98% of its employees now use Codex agents》，2026年6月26日）
- CNN Business（《White House asks OpenAI to limit its next model release》，2026年6月25日）
- CNBC（《OpenAI limits new AI models to trusted partners, request US government》，2026年6月26日）
- VentureBeat（《OpenAI unveils GPT-5.6 Sol, Terra and Luna models》，2026年6月26日）
- Axios（《OpenAI releases powerful new GPT-5.6 model under restrictions》，2026年6月26日）
- MacRumors（《OpenAI Launches GPT-5.6 Sol, Terra, and Luna in Limited Preview》，2026年6月26日）
- MarkTechPost（GPT-5.6 tiered models + pricing details，2026年6月26日）
- Yahoo Finance（《Big Tech's $2.7 trillion AI bill comes due: Chart of the Day》，2026年6月27日）
- Startup Fortune（《Big Tech has lost $2.7 trillion in market value this month》，2026年6月27日）
- Knowledge Hub Media（《Big Tech's $2.7 Trillion AI Reckoning》）
- TechCrunch（《AI researchers continue to leave Google for its rivals》，2026年6月24日）
- Bloomberg（《Google Poised to Lose Two More High-Profile AI Staffers to Anthropic》，2026年6月24日）
- CryptoBriefing（《Anthropic recruits two more key Gemini researchers from Google》，2026年6月24日）
- The Next Web（《Two more Gemini researchers are leaving Google for Anthropic》，2026年6月24日）
- AITNT（《2026.06.27 Global AI News Daily》，2026年6月27日）
- LLM-stats.com（June 2026 模型更新全局扫描）
- OSSInsight（GitHub Trending AI repos — 无独立时效事件锚点，排除）
- arXiv embodied AI / world models June 2026（背景扫描，无独立高传播单篇事件锚点，排除）
- Anthropic《The Briefing: AI for Science》虚拟活动（6月30日，未发生，排除）
- Jonas Adler + Alexander Pritzel / Google→Anthropic（6月24日，Bloomberg + TechCrunch 确认；内容和 6月24日候选文件 Shazeer+Jumper 叙事柱相同，Adler/Pritzel 新增"IPO 吸引力"角度但信号强度弱于今日三个候选，排除）

**Total signals found**: 约 22 个信号评估

**Why these 3**:

- **Candidate 1（OpenAI Codex Agent 数据报告，6月25-26日）**：**Agent经济柱**：过去4天 SELECTED 覆盖了 AI协作实践（6月25日）、AI产品战略（6月24日）、组织形式变革（6月26日）——Agent经济柱连续4天未被使用，今日强制优先；时效最强（1-2天前，OpenAI 官方 + arXiv 同步发布）；「法律和招聘团队把 Codex 当主力 AI 工具」+ 「99分位用户每天60小时 Agent 执行量」这两个具体数字在中文媒体几乎无深度分析（中文媒体会翻译数据，不会分析"60小时/天意味着用户角色变成了 Agent PM"这个结构性转变）；arXiv 论文 2606.26959v1 提供学术锚点；与 Zico 的 Agent 经济框架直接对应；**HIGH 优先级**。

- **Candidate 2（GPT-5.6 白宫逐客户审批，6月25-26日）**：**AI产品战略柱**（虽然该柱6月24日被使用，今日角度独立——「主动协商分级发布 vs. 被动关停」的治理结构对比）；CNN Business + CNBC + VentureBeat + Axios + OpenAI 官方五方来源确认；这是继 Fable 5 出口管制（#053）之后政府第二次介入前沿 AI 模型，但机制完全不同：前者是主权行政命令强制关停，后者是协商分级访问控制——两种不同的"政府-AI公司"关系结构正在同时出现；Sol/Terra/Luna 三层定价结构 + "政府变成 KYC 外包"这一机制分析在中文媒体完全缺席；与 Fable 5 故事（#053）形成对话但角度完全独立；**HIGH 优先级**。

- **Candidate 3（科技九巨头 $2.7 万亿蒸发，6月27日）**：**深层AI思考柱**：过去4天未被 SELECTED 使用此柱；Yahoo Finance Chart of the Day 今日首发，时效最强（今天）；$7250 亿 capex + 3% 付费家庭 = 两个可独立验证的精确数字，构成"发现式"钩子（读者可以自己验证计算）；与 LeCun 6月18日的"大泡沫爆炸"预言形成叙事链但角度不同——LeCun 是预测，这是市场已经发生的行动；「AI capex 是基础设施投资，不是软件投资，评估框架不同」这一判断在中文 AI 财经媒体几乎无系统分析；规模（$2.7 万亿）提供自然传播势能；**HIGH 优先级**。
