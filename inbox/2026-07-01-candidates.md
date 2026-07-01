---
date: 2026-07-01
status: pending_selection
---

# Today's Candidates

## Candidate 1: Anthropic 昨天发布 Claude Science Workbench——Nobel 得主 John Jumper 首次公开亮相，VirBench 数据说明工具集成质量决定 AI 科学家准确率（而非模型质量）（June 30）

- **Event**: 2026年6月30日（昨天），Anthropic 在旧金山举行 **"The Briefing: AI for Science"** 发布活动，正式推出 **Claude Science Workbench**——专为科研人员设计的 AI 工作台。核心产品数据：① Claude Science Workbench 接入 **60+ 个科学数据库**，内置基因组学、蛋白质结构、化学等领域的预置工具包，集成 **Modal** 等计算资源，产出可审计的研究 artifacts；② Anthropic 为 **50 个** AI for Science 项目提供最高 **$30,000** 的 Claude API Credits + Modal $2,000 计算补贴；③ 大会发布 **VirBench**——一个包含 **120 条病毒序列检索查询、涵盖 40 种病原体**的生物 AI 基准测试，核心发现：Claude Sonnet 4 在 **无工具辅助**下准确率仅 **16.9%**，接入确定性工具（数据库 API）后准确率跳升至 **91.3%**；同天发布 **GPT-5.5** 同类测试对照；④ 诺贝尔奖得主 **John Jumper**（AlphaFold 联合创始人，2024年诺贝尔化学奖得主）在离开 Google DeepMind 11 天后首次公开亮相，发表演讲；⑤ 背景：Anthropic 2026年2月宣布与 **Allen Institute（艾伦研究所）** 和 **Howard Hughes Medical Institute（HHMI）** 建立旗舰科研合作，并开设了真实的 **湿实验室（wet labs）**；Andrej Karpathy 于5月加入 Anthropic 主导预训练研究，Jumper 于6月20日宣布加入主导 AI for Science 方向。来源：**TechCrunch**（2026年6月30日，《Anthropic's Claude Science bets on workflow, not a new model, to win over scientists》）、**HPCWire/AIwire**（2026年6月30日，《Anthropic Launches Claude Science AI Workbench for Scientific Research》）、**Technobezz**（2026年6月30日，《Anthropic Launches Claude Science Workbench for Researchers and Drug Discovery》）、**Anthropic 官方活动页面**（The Briefing: AI for Science，2026年6月30日）、**CNBC**（2026年6月19日，John Jumper 宣布离职 DeepMind）、**TechTimes**（2026年6月20日，《AlphaFold Nobel Laureate John Jumper Joins Anthropic After Nine Years at DeepMind》）。
- **Source**: https://techcrunch.com/2026/06/30/anthropics-claude-science-bets-on-workflow-not-a-new-model-to-win-over-scientists/ | https://www.hpcwire.com/aiwire/2026/06/30/anthropic-launches-claude-science-ai-workbench-for-scientific-research/ | https://www.anthropic.com/events/the-briefing-ai-for-science-virtual-event | https://www.cnbc.com/2026/06/19/john-jumper-to-leave-google-deepmind-for-anthropic.html | https://www.techtimes.com/articles/318754/20260620/alphafold-nobel-laureate-john-jumper-joins-anthropic-after-nine-years-deepmind.htm | https://www.technobezz.com/news/anthropic-launches-claude-science-workbench-for-researchers-and-drug-discovery | https://aitoolsrecap.com/Blog/ai-news-june-30-2026
- **Timeliness**: 1 天前（2026年6月30日，Anthropic 官方发布活动）
- **Topic pillar**: AI产品战略
- **Zico's angle**: TechCrunch 的标题点名了核心：Claude Science "bets on workflow, not a new model"。这是 Anthropic 明确用产品策略做了一个判断：**科学 AI 的瓶颈不是模型质量，是工具集成质量**。

  VirBench 的数据是证据：Claude Sonnet 4 没有工具时准确率 16.9%，有工具时 91.3%——同一个模型，5.4 倍的精度差距，完全来自工具访问权限，不来自模型本身的升级。这个数字在中文媒体几乎没有被分析过，但它是当前 AI for Science 领域最重要的基准之一：如果你想让 AI 做科学研究，与其等下一代更强的基础模型，不如先把工具接入权限做对。

  这和 DeepMind 的路径形成了直接对比。DeepMind 做 AlphaFold 的方式是：**建一个专用的突破性模型**（AlphaFold 本身就是一个专为蛋白质折叠设计的架构）。Anthropic 做 Claude Science 的方式是：**用现有前沿模型 + 结构化工具接入 + 工作流工程**，绕过"模型够不够好"的问题直接去解决"科学家用 AI 的工作流是否对"的问题。

  从产品 PM 的视角，这是两种不同的"制高点"策略：DeepMind 抢的是模型层（AlphaFold 是 DeepMind 的护城河）；Anthropic 抢的是工作流层（60+ 数据库接入 + 可审计 artifacts = 科研 SOP 的 AI 化）。现在 Anthropic 还把 AlphaFold 的发明者本人（Jumper）从 DeepMind 挖走了——这是在**同时威胁 DeepMind 的模型层护城河和工作流层布局**。

  中文媒体会报"Anthropic 做了一个科学 AI 产品"，不会分析：**当 VirBench 证明工具集成质量比模型质量更决定性时，整个 AI for Science 领域的竞争逻辑从"谁训出最好的科学模型"变成了"谁先锁定科学工作流入口"**——这和 AI 编程领域（Cursor vs Claude Code 之争）的竞争逻辑完全同构。

- **Resonance hook**: 昨天，Anthropic 发布了一个数字：Claude Sonnet 4 在生物病毒数据库查询上，没有工具时准确率 16.9%，有工具时 91.3%。同一个模型，5 倍以上精度差距，全部来自工具接入，不来自模型本身。Anthropic 招了 AlphaFold 发明者 John Jumper，建了湿实验室，做了 AI for Science 发布会——但 TechCrunch 说他们赌的是"workflow，not a new model"。科学 AI 的下一个护城河，不一定在模型里。
- **Recommended priority**: high

---

## Candidate 2: GitHub Copilot 第一个完整计费周期昨天结束——开发者账单从 $29/月跳到 $750，10-50 倍成本冲击（June 1 起，June 30 首周期结束）

- **Event**: 2026年6月1日，GitHub Copilot 正式从固定订阅制切换至**基于 token 消耗的用量计费（usage-based billing）**——每个 Copilot 计划包含月度 AI Credits 额度，超额按 API 定价收费。2026年6月30日（昨天）为**第一个完整计费周期结束日**，大量开发者收到或计算出了首个完整月度账单，Reddit / X / GitHub Discussions 上的反应立刻爆发。核心数据：① **Copilot Pro（原 $29/月）→ 重度 agentic 工作流用户实际消耗：$750/月**（增幅 25 倍）；② **Copilot Pro+（原 $50/月）→ 最重度用户估算：$3,000/月**（增幅 60 倍）；③ TechCrunch 报道：**"一名开发者单次 change request 花了超过 $6"**；④ **一名开发者单天消耗约 360 AI Credits**，主动降低部分工作流使用以控制成本；⑤ **The Register** 标题直接：《Angry devs vow to flee GitHub Copilot as metered billing takes hold》；⑥ 开发者列出迁移替代方案：直接调用 Anthropic / OpenAI API，或通过 **OpenRouter / RooCode / LM Studio** 等第三方路由。GitHub 方面（Microsoft 旗下）在 GitHub Discussions（#192948）中确认机制不变。来源：**TechCrunch**（2026年5月30日，《'What a joke': GitHub Copilot's new token-based billing spurs consternation among devs》）、**The Register**（2026年6月2日，《Angry devs vow to flee GitHub Copilot as metered billing takes hold》）、**gHacks Tech News**（2026年6月2日，《GitHub Copilot Usage-Based Billing Takes Effect, Drawing Developer Backlash Over Rapid Credit Depletion》）、**GitHub Blog**（官方公告，usage-based billing 机制说明）、**GitHub Community Discussions #192948**（开发者反馈汇总，实时更新）、**techjournal.org**（《GitHub Copilot Token Billing Starts Today: Devs Report 10x-50x Cost Increases》）、**Visual Studio Magazine**（2026年6月4日，《Copilot Billing Shock Hits Developers》）。
- **Source**: https://techcrunch.com/2026/05/30/what-a-joke-github-copilots-new-token-based-billing-spurs-consternation-among-devs/ | https://www.theregister.com/ai-and-ml/2026/06/02/github-copilot-users-threaten-exit-as-metered-billing-kicks-in/5249826/ | https://www.ghacks.net/2026/06/02/github-copilot-usage-based-billing-takes-effect-drawing-developer-backlash-over-rapid-credit-depletion/ | https://github.blog/news-insights/company-news/github-copilot-is-moving-to-usage-based-billing/ | https://github.com/orgs/community/discussions/192948 | https://techjournal.org/github-copilot-token-billing-backlash | https://visualstudiomagazine.com/articles/2026/06/04/copilot-billing-shock-hits-developers.aspx
- **Timeliness**: 第一个完整计费周期昨天（6月30日）结束；账单冲击爆发于 1-29 天内持续发酵
- **Topic pillar**: Agent经济
- **Zico's angle**: 这不是 GitHub Copilot 涨价的问题，这是 AI coding agent 的计费模型从**「订阅服务」转向「计量基础设施」**，而这个转变的第一批受害者是那些最重度使用 agentic 工作流的开发者。

  逻辑是这样的：订阅制的隐含假设是"你用多少 AI，成本是固定的"——这和用云存储的逻辑是一样的（最早的云存储也是固定套餐）。计量制的隐含假设是"你用多少计算，你就付多少"——这和 AWS EC2 按秒计费的逻辑是一样的。从订阅到计量，不是一个定价调整，是**AI 工具从"产品"变成"基础设施"的信号**。

  但计量制有一个关键副作用：**它让成本变得可见，从而强制开发者开始思考"这件事值得让 AI 做吗"**。在 $29/月固定订阅的时代，一个开发者不会去问"用 Claude Code 做 code review，每次花多少钱，值不值"——因为成本是固定的，边际使用成本为零。在 $6/次 change request 的计量时代，这个问题必须被回答。

  这对 Agent 经济有一个直接含义：**metered billing 是第一个让 AI agent 的经济成本真实化的机制**。当 AI coding agent 的每次执行都有显式成本，开发者就开始像管理工程团队那样管理 AI：哪些任务值得 delegate，哪些任务自己做更高效，哪些任务的 AI 输出质量足以抵消成本。这是 Agent 经济从"用尽可能多的 AI"到"用最合适的 AI 做合适的事"的必要转变——GitHub Copilot 的计费改变让这个转变提前发生了。

  Uber 在 2026年前四个月烧完了全年 AI 预算，找不到 token 消耗和消费者功能价值之间的关联（见6月26日 CNBC 报道）。GitHub Copilot 的计量冲击是同一个问题在个人开发者层面的精确重演：**在没有真实成本信号之前，AI 的使用量和 AI 的价值创造之间的关联从未被迫建立过**。现在成本信号来了。

- **Resonance hook**: 昨天，GitHub Copilot 完成了切换计量计费后的第一个完整月度账单周期。有开发者发现自己的成本从 $29/月跳到了 $750，有人单次 change request 花了 $6。The Register 标题：Angry devs vow to flee。这不是 Copilot 涨价了，这是 AI coding tool 第一次对开发者诚实地说：你委托给 AI 的每一件事，都有真实成本。这个成本信号，以前从来没有出现过。
- **Recommended priority**: high

---

## Candidate 3: Gemini 2.5 Pro Deep Think 以 82.4% GPQA Diamond 拿下科学推理第一——同期 ChatGPT 首次跌破 50% 市场份额，AI 能力正在按领域专业化分化（June 16-22）

- **Event**: 2026年6月22日，Google DeepMind 发布 **Gemini 2.5 Pro with Deep Think**，该版本在多个科学与推理基准上取得历史最高分：① **GPQA Diamond**（研究生级别科学，含物理、化学、生物）：**82.4%**（Anthropic Fable 5 封锁前最高：79.1%；OpenAI GPT-5.5：76.3%）；② **MMLU-Pro**（多学科综合理解）：**89.8%**，为所有公开模型最高；③ **Humanity's Last Exam**（跨学科专业知识极限基准）：当前最优。Deep Think 技术本质：**在推理时启动扩展并行推理（extended parallel inference）**，不是单纯扩大模型规模，而是在答题瞬间投入更多计算量做多路并行思考。与此同时，Gemini 2.5 Pro 仍在软件工程基准（SWE-bench Verified）上落后于 Fable 5；GPT-5.5 在创意写作和对话自然度上仍有领先。同期数据：2026年6月16日，市场分析公司 **Sensor Tower** 发布 State of AI 2026 报告：**ChatGPT 全球 AI 助手市场份额降至 46.4%**，为有记录以来**首次跌破 50%**（实际跌破发生在3月2026，6月16日为首次公开披露）；Gemini：27.7%；Claude：10.3%；xAI Grok：剩余份额分担。来源：**FAQ.com.tw**（2026年6月27日，《Google's Gemini 2.5 Deep Think Claims the Top of Science, Math, and Reasoning Benchmarks》）、**Ortemtech**（《Gemini 2.5 Pro 2026: 2M Context, Deep Think — When It Beats GPT-5.5 & Claude Opus》）、**TechCrunch**（2026年6月16日，《ChatGPT's market share slips below 50% for first time》）、**Business Standard**（2026年6月17日，《ChatGPT market share slips below 50% as Gemini, Claude gain ground》）、**Google DeepMind 官方 blog**（Gemini 2.5 Deep Think 发布，2026年6月22日）、**Artificial Analysis**（Gemini 2.5 Pro benchmark 完整对比数据）。
- **Source**: https://faq.com.tw/en/ai-ml/2026-06-27-google-gemini-25-deep-think-reasoning-en/ | https://techcrunch.com/2026/06/16/chatgpts-market-share-slips-below-50-for-first-time/ | https://www.business-standard.com/technology/artificial-intelligence/chatgpt-market-share-slips-below-50-google-gemini-anthropic-claude-gain-ground-126061700765_1.html | https://blog.google/products/gemini/gemini-2-5-deep-think/ | https://artificialanalysis.ai/models/gemini-2-5-pro | https://ortemtech.com/blog/gemini-2-5-pro-complete-guide-2026/
- **Timeliness**: 9 天前（Gemini 2.5 Pro Deep Think，2026年6月22日）；ChatGPT 跌破 50% 报告，15 天前（6月16日）；信息增量在中文圈仍为低覆盖
- **Topic pillar**: 深层AI思考
- **Zico's angle**: 两件事放在一起读，才能看见真正的信号。

  Gemini 2.5 Pro Deep Think 在 GPQA Diamond 上以 82.4% 拿了第一，Fable 5 此前最高 79.1%，GPT-5.5 76.3%——科学推理，Google 赢了。但 Fable 5 在软件工程基准（SWE-bench Verified）上仍然领先；GPT-5.5 在创意写作上仍然更自然。ChatGPT 的市场份额跌破了 50%，Gemini 拿到了 27.7%，Claude 10.3%。

  这个格局说明了一件事：**AI 模型市场没有在收敛成"一个赢家"，它在按领域能力分化**。科学推理领域，Google Gemini 领先；代码生成和 agentic 任务，Anthropic Fable 5 领先；对话自然度，GPT-5.5 领先；成本效益，GLM-5.2 等开源模型正在逼近。

  LLM 领域最早流行的叙事是"谁参数多谁赢"，然后是"谁 benchmark 最高谁赢"，现在这个叙事正在失效。**Gemini 2.5 Pro 的 Deep Think 不是在所有维度超越了所有人，它是在"推理时投入更多计算量做多路并行思考"这一机制上找到了科学推理的专项优势**。这和 Fable 5 在长时程 agentic coding 上的优势来自不同的机制假设，和 GPT-5.5 对话流畅度的优势来自又一个不同的机制假设。

  对 AI 产品 PM 的直接含义：**"用最好的 AI 模型"这个决策规则正在失效**。如果你在做科学研究工具，Gemini 2.5 Pro Deep Think 在推理密集任务上比 Claude 或 GPT-5.5 便宜且更准确；如果你在做代码生成工具，Fable 5 的 SWE-bench 优势可能更重要；如果你在做对话产品，GPT-5.5 的自然度可能比基准分数更关键。未来 12 个月，"模型选型"会变成一个需要按任务类型做专项评估的工程决策，而不是品牌忠诚决策。

  中文媒体停在"Google追上了" / "ChatGPT掉份额了"的叙事层——没有人在分析**能力专业化分化**这个更深层的结构变化，以及它对 AI 产品构建的实际影响。

- **Resonance hook**: 6月22日，Gemini 2.5 Pro Deep Think 以 82.4% GPQA Diamond 拿下科学推理第一，比 Fable 5 和 GPT-5.5 都高。但 Fable 5 在代码生成上还是最强，GPT-5.5 在对话自然度上还是更好。ChatGPT 首次跌破 50% 市场份额，但没有一家公司全面领先。"用最好的 AI"这个建议正在变得没有意义——在科学、代码、对话三个场景，答案已经不一样了。
- **Recommended priority**: medium-high

---

## Scan summary

**Sources scanned**:
- AIToolsRecap（2026年6月30日，《AI News June 30 2026: Anthropic's AI for Science Event — What Was Announced and What It Means》）
- TechCrunch（2026年6月30日，《Anthropic's Claude Science bets on workflow, not a new model, to win over scientists》）
- HPCWire/AIwire（2026年6月30日，《Anthropic Launches Claude Science AI Workbench for Scientific Research》）
- Anthropic 官方活动页面（The Briefing: AI for Science，2026年6月30日）
- Technobezz（2026年6月30日，《Anthropic Launches Claude Science Workbench for Researchers and Drug Discovery》）
- byteiota（《Anthropic's AI for Biology: The Accuracy Crisis Explained》，VirBench 数据分析）
- CNBC（2026年6月19日，《John Jumper to leave Google DeepMind for Anthropic》）
- TechTimes（2026年6月20日，《AlphaFold Nobel Laureate John Jumper Joins Anthropic After Nine Years at DeepMind》）
- TechCrunch（2026年5月30日，《'What a joke': GitHub Copilot's new token-based billing spurs consternation among devs》）
- The Register（2026年6月2日，《Angry devs vow to flee GitHub Copilot as metered billing takes hold》）
- gHacks Tech News（2026年6月2日，《GitHub Copilot Usage-Based Billing Takes Effect, Drawing Developer Backlash》）
- GitHub Blog（官方公告，usage-based billing 机制说明）
- GitHub Community Discussions #192948（开发者反馈汇总）
- techjournal.org（《GitHub Copilot Token Billing Starts Today: Devs Report 10x-50x Cost Increases》）
- Visual Studio Magazine（2026年6月4日，《Copilot Billing Shock Hits Developers》）
- FAQ.com.tw（2026年6月27日，《Google's Gemini 2.5 Deep Think Claims the Top of Science, Math, and Reasoning Benchmarks》）
- TechCrunch（2026年6月16日，《ChatGPT's market share slips below 50% for first time》）
- Business Standard（2026年6月17日，《ChatGPT market share slips below 50% as Gemini, Claude gain ground》）
- Google DeepMind 官方 blog（Gemini 2.5 Deep Think 发布，2026年6月22日）
- Artificial Analysis（Gemini 2.5 Pro benchmark 完整数据对比）
- CNBC（2026年6月22日，SpaceX Reflection AI $6.3B compute deal — 主题与6月30日 SpaceX/Cursor 候选重叠，排除）
- Forbes（2026年6月24日，《SpaceX's Colossus Lands $6.3 Billion Compute Deal With Reflection AI》——同上，排除）
- CNBC（2026年6月22日，《OpenAI launches GPT-5.5-Cyber》——无深层产品战略叙事锚点，排除）
- Medium（《AI NEWS: Week of June 22 to June 28, 2026》——汇总，无独立新锚点）
- dentro.de（《AI News - June 2026: Key Events & Releases》——汇总，无独立新锚点）
- Sequoia Capital AI Ascent 2026（4月活动，超30天窗口，排除）
- Boston Dynamics + Gemini Robotics-ER 1.6（April 14, 2026，超30天，排除）
- Amazon Trainium $20B ARR（6月18-30，Bloomberg 首发 6月18日，超7天窗口，技术指标类无强叙事，排除）
- ChatGPT GPT-4.5 从 ChatGPT 下线（6月26日，排除于 6月29日候选文件）

**Total signals found**: 约 22 个信号评估

**Why these 3**:

- **Candidate 1（Anthropic Claude Science Workbench，昨天 6月30日）**：**AI产品战略柱**——查阅近期选中记录（059 third-paradigm / 060 tokenmaxxing-end / 061 trust-inheritance-trap），AI产品战略是近 7 天内选中频次最低的柱（最近一次选中约在 6月23日 054-pipeline-monopoly）；时效最强（昨天）；VirBench 16.9% vs 91.3% 这组数字是具体可引用的产品层面证据（发现式钩子）；"workflow not model"这个 TechCrunch 标题直接命名了策略判断——中文媒体完全缺失这层分析；John Jumper + Karpathy 在同一家公司是传播亮点（AlphaFold 发明者 + 深度学习教父级人物，共同赌注 Anthropic）；Allen Institute + HHMI + 湿实验室是产品战略外化证据；**HIGH 优先级**。

- **Candidate 2（GitHub Copilot 计量计费冲击，6月30日第一周期结束）**：**Agent经済柱**——6月30日候选（061 Agentjacking）已选中 Agent経済柱，但角度完全不同：Agentjacking 是 Agent 的安全信任问题，Copilot 计量计费是 Agent 的经济模型问题；时效最强（昨天是第一个完整周期结束日，开发者账单冲击今天最集中）；$29→$750 / $50→$3000 等具体数字符合发现式钩子（读者能自己算自己的成本）；与 6月29日 tokenmaxxing 故事（企业层面，Uber COO 视角）形成个人开发者层面的精确对称——同一个"AI 成本不透明"问题在不同粒度的表现；"metered billing = 第一个强制建立 AI 价值验证的机制"这一论点在中文圈完全没有人分析；**HIGH 优先级**。

- **Candidate 3（Gemini 2.5 Pro Deep Think，6月22日；ChatGPT 跌破 50%，6月16日）**：**深层AI思考柱**——查阅6月28/29/30候选排除列表，未见 Gemini 2.5 Pro Deep Think 被明确排除（排除列表集中在 GPT-5.6、GLM-5.2、Cosmos 3、Karpathy 3rd paradigm 等已覆盖话题）；时效为 9 天（略超7天最优窗口，但信息增量在中文圈仍属低覆盖）；"AI 能力按领域专业化分化"这一叙事（科学 → Gemini，coding → Fable 5，对话 → GPT-5.5）在中文媒体完全缺失（停在"Google 追上了/ChatGPT 掉份额了"的竞争态叙事）；与 Candidate 1（Claude Science 工具工程）形成补充：同一周，Google 在科学推理方向拿了第一，Anthropic 在科学工作流方向发了产品——两个不同赌注；**MEDIUM-HIGH 优先级**。
