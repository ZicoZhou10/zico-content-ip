---
date: 2026-05-23
status: written
selected: candidate 1 → drafts/025-outcome-pricing-xhs.md
---

# Today's Candidates

## Candidate 1: Zendesk 在 Relate 2026 宣布按"结果"而非"席位"向 AI Agent 收费（May 19）：企业 SaaS 的定价原子，从访问权变成了输出量

- **Event**: 2026年5月19日（4天前），Zendesk 在其年度 Relate 2026 大会（丹佛）宣布"Autonomous Service Workforce"愿景，推出全面重构的定价模型——**Outcome-Based Pricing（结果导向定价）**：每一个由 AI Agent 成功处理的客服 ticket，收费 **$1.50 起**（大客户享折扣，Pay-as-you-go 为 **$2.00**），未能解决需转人工的对话**不计费**。关键细节：① Zendesk 对"成功解决"的定义采用**双重验证**——AI Agent 自评完成交互 + 一个独立的 AI 评估模型再次确认，两个条件都满足才计费；② 同步宣布 AI Agent 覆盖全渠道（messaging、email、voice），并推出 No-Code Agent Builder 和 MCP（Model Context Protocol）集成支持；③ Zendesk Resolution Platform 基于 **200 亿条历史 ticket** 训练，是业界规模最大的客服 AI 训练数据集之一；④ Zendesk 产品工程 AI 总裁 **Shashi Upadhyay** 在发布会上的原话："Stop thinking of agents as software... start thinking of them as a unit of labor."。竞争背景：Intercom 已以 **$0.99/resolved conversation** 跑到 $100M+ ARR；HubSpot Customer Agent 在 2026 年4月从 $1.00 降至 **$0.50**；Salesforce Agentforce 同期采用 **$2/conversation** 结构。来源：Zendesk 新闻稿（May 19）、TechRadar（May 19）、CMSWire（May 19）、diginomica（May 19）、Computer Weekly（May 19）。
- **Source**: https://www.zendesk.com/newsroom/articles/relate-2026/ | https://www.techradar.com/pro/zendesk-links-ai-pricing-to-verified-resolution-outcomes | https://www.cmswire.com/customer-experience/zendesk-unveils-autonomous-ai-workforce-at-relate-2026/ | https://diginomica.com/zendesk-relate-2026-outcome-based-future-verified-resolutions | https://www.computerweekly.com/news/366611612/Zendesk-debuts-outcome-based-pricing-for-AI-agents
- **Timeliness**: 4 days ago（2026年5月19日）
- **Topic pillar**: Agent 经济
- **Zico's angle**: Shashi Upadhyay 那句"停止把 Agent 看作软件，开始把它当作劳动力的单位"听起来像一句营销口号，但它实际上在描述一件真实发生的事：**定价单位的改变正在重新定义 AI Agent 的本质**。传统 SaaS 定价里，你买的是"访问权"——订了席位，不管用不用，按月付。Outcome-based pricing 把买的东西换成了"输出量"：AI Agent 不上班时不收费，搞砸了不收费，只有真的解决问题才收费。这不只是定价策略的调整，是一次关于"AI 是什么"的底层重新定义。Intercom 早就在用这个模型，但 Zendesk 是 CX 行业规模最大的玩家之一，当 Zendesk 把这个模型标准化，**"按结果付费"就从先锋选择变成了行业基线**。对 Zico 受众来说，这里有一个更深的工程问题：什么叫"verified resolution"？Zendesk 的答案是用一个独立的 AI 评估模型来确认另一个 AI 的工作——**你需要 AI 来验证 AI**。这是一种新的基础设施层，在 Agent 经济里还没有多少人意识到它的必要性。中文 AI 圈对这个事件的报道停留在"Zendesk 又更新了什么"，没有分析这个"验证层"对 Agent 产品设计意味着什么。
- **Resonance hook**: 2026年5月19日，Zendesk 宣布：AI Agent 解决了 ticket 才收钱，没解决不收钱，每个成功解决的对话 $1.50 起。确认方式是双重验证——一个 AI 说解决了，另一个 AI 来复核。Intercom 同样的模式已经到了 $100M+ ARR。Shashi Upadhyay 的原话："Stop thinking of agents as software... start thinking of them as a unit of labor." 席位这个定价单位，正在被 outcome 取代。
- **Recommended priority**: high

---

## Candidate 2: Meta 裁 8000 人 + Intuit 裁 3000 人，同日（May 20）：创纪录营收 + 大规模裁员，是矛盾还是新组织逻辑？

- **Event**: 2026年5月20日（3天前），**Meta** 宣布裁员约 **8,000 人**（占员工总数 78,865 人的约 **10%**），同时取消 **6,000 个在招职位**，合计有效减员 **14,000 人**。同一天，**Intuit** CEO Sasan Goodarzi 在内部备忘录中宣布裁减约 **3,000 人**（占员工 **17%**）。关键数据对比：Meta Q1 2026 单季营收 **$563 亿**（创历史纪录），同期宣布 2026 全年 AI 基础设施投入 **$1350 亿-$1450 亿**；Intuit Q3 FY2026 营收 **$46.5 亿**（同比增长 **17%**），净利润 **$6.93 亿**（同比增长 **48%**）。内部细节：① Meta 此次裁员的结构不同于以往：不是裁绩效末位，而是全公司架构重组——大量员工职位被重命名为 **"AI builder"、"AI pod lead"、"AI org lead"**，约 **7,000 人**被分配到新成立的 AI 专属团队（Applied AI Engineering、Agent Transformation Accelerator XFN、Central Analytics）；② Zuckerberg 将 Meta Superintelligence Labs（由前 Scale AI CEO **Alexandr Wang** 主导）设为公司核心增长引擎；③ Intuit CEO Goodarzi 在 CNBC 采访中明确表示此次裁员"与 AI **无关**"（had "nothing to do with AI"），但 TechCrunch 标题是"Intuit to lay off over 3,000 employees **to refocus on AI**"，两者说法直接矛盾。来源：NPR（May 20）、The Next Web（May 20，多篇）、TechCrunch（May 20，Intuit 裁员）、CNBC（May 20，Intuit Q3 earnings + CEO 声明）、Yahoo Finance（May 20，Meta 裁员）。
- **Source**: https://www.npr.org/2026/05/20/nx-s1-5826917/meta-layoffs-ai-jobs | https://thenextweb.com/news/meta-layoffs-8000-zuckerberg-ai-reality-may-2026 | https://techcrunch.com/2026/05/20/intuit-to-lay-off-over-3000-employees-to-refocus-on-ai/ | https://www.cnbc.com/2026/05/20/intuit-ceo-says-companys-17percent-workforce-cut-had-nothing-to-do-with-ai.html | https://letsdatascience.com/blog/meta-8000-layoffs-may-20-135-billion-ai-wang
- **Timeliness**: 3 days ago（2026年5月20日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: "创纪录营收 + 大规模裁员"这个组合出现在同一个季报里，不是悖论，是一个新的组织逻辑在运行。Meta 在裁员的同时花 $1450 亿买 AI 基础设施——这意味着它认为自己可以用更少的人 + 更多的算力产出同样甚至更多的收入。这不是成本压缩，是**生产函数的替换**：人力 → 算力。但 Meta 这次裁员有一个细节比裁员数字更值得关注：他们在**重新命名所有职位**。"AI builder"、"AI pod lead"、"AI org lead"——这不是语义游戏，是在用新的职位名称固化一种新的工作范式：人不再是直接的生产者，而是 AI 生产单元的设计者和协调者。Zuckerberg 把公司的核心组织单元从"部门"变成了"AI pod"——一个以 AI 为中心的小型工作单元，人类在里面扮演的是设计者和仲裁者，不是执行者。这是 Zico 长期在写的"组织形式三阶段"里，从第二阶段（AI 辅助人工）向第三阶段（人类监督 AI 生产单元）的真实转型。Intuit CEO 说裁员"与 AI 无关"这件事本身也值得单独分析：**"AI 驱动裁员"这个叙事已经变成了政治雷区**——公司知道媒体会拿这个框架放大，所以即使是 AI 重组，CEO 也开始用"simplification"、"focus"这样的中性词替代。但这种措辞回避本身证明了：AI 驱动的结构性裁员在2026年已经是不言而喻的背景。中文 AI 圈的报道会停在"Meta 又裁员了"，不会分析 Meta 同时在做什么：把 7,000 人重新分配到 AI pod 里。裁员和 AI 重组是同一件事的两面。
- **Resonance hook**: 2026年5月20日，Meta 宣布裁 8,000 人（同时取消 6,000 个在招职位），当季营收创历史最高 $563 亿，同年 AI 基础设施投入 $1450 亿。同一天，Intuit 裁 3,000 人（17%），营收同比增长 17%，利润同比增长 48%。Meta 没有只是裁员——它把剩下的人重命名为"AI builder"和"AI pod lead"，把 7,000 人转入 AI 专属团队。创纪录营收 + 组织重构 + 裁员，同时发生。这是生产函数在换人。
- **Recommended priority**: high

---

## Candidate 3: Anthropic 联合创始人 Jack Clark 在牛津预测：12个月内 AI 协作诺贝尔级突破，2028年前 AI 自主训练下一代自己（May 21）

- **Event**: 2026年5月21日（2天前），Anthropic 联合创始人、Import AI 创始人 **Jack Clark** 在牛津大学 **Institute for Ethics in AI** 发表公开演讲，做出一系列带具体时间窗口的预测：① **12个月内**：AI 将与人类协作完成一项诺贝尔奖级别的科学发现（"AI will work with humans to make a Nobel prize-winning discovery within 12 months"）；② **18个月内**：完全由 AI 运营的公司将产生数百万美元营收（"AI-run companies generating millions in revenue within 18 months"）；③ **2年内**：双足机器人开始协助工匠（bipedal robots assisting tradespeople in two years）；④ **2028年前**：AI 系统将能设计自己的继任者，Clark 给出的概率是 **60%以上**（"a 60%+ chance of an AI model fully training its successor by the end of 2028"）。同时 Clark 维持了对 AI 存在性风险的警告：AI 仍然存在"非零概率伤害所有人"的场景，这个风险没有消失。Time Magazine 次日（5月22日）将此事定性为："Anthropic Sells Claude's Promise While Warning About AI's Dangers"。背景：Clark 是 OpenAI 研究政策前主任，Anthropic 联合创始人之一，同时创办 Import AI 周刊（AI 领域技术深度最高的英文 newsletter 之一），在 AI 前沿研究者中影响力极高。来源：Resultsense（May 21）、TechCentral.ie（May 21）、Time Magazine（May 22）、Axios（背景，May 7）。
- **Source**: https://www.resultsense.com/news/2026-05-21-jack-clark-anthropic-ai-nobel-prize-prediction/ | https://www.techcentral.ie/anthropic-co-founder-predicts-that-ai-will-within-a-year/ | https://time.com/article/2026/05/22/anthropic-claude-code-jack-clark-ai-safety/ | https://www.axios.com/2026/05/07/anthropic-jack-clark-ai-intelligence-explosion
- **Timeliness**: 2 days ago（2026年5月21日）
- **Topic pillar**: 深层思考
- **Zico's angle**: Jack Clark 在牛津说了什么不是重点，重点是**他为什么敢说**，以及**这四个预测的内在逻辑**。Clark 不是普通的 AI 乐观主义者——他是 Anthropic 的联合创始人，Import AI 的创始人，对 AI 安全问题比大多数技术人更了解。他同时预测了"AI 12个月内帮助获得诺贝尔奖"和"AI 有非零概率杀死所有人"——这两件事在他的框架里不矛盾，因为他认为这是同一个技术趋势的两个面。值得单独拆解的是"2028年前 AI 自主训练下一代自己，概率 60%+"这个预测。这不是随口说的科幻——这是一个 AI 安全领域顶级研究者对**递归自我改进**（recursive self-improvement）时间线给出的明确概率估计。递归自我改进的含义：AI 不再需要人类研究员来设计下一代训练流程，而是由当前代模型自己生成训练数据、设计架构改进、验证优化效果。Anthropic 内部用 Claude 加速 Claude 预训练研究（Karpathy 回来做的正是这件事），就是这个方向的早期形式。Clark 给出"2028年前，60%+"这个概率，意味着 Anthropic 内部的推断是：递归自改进不是5-10年的问题，是2-3年的工程问题。如果这个预测的方向基本正确（哪怕概率打个5折），那么 2026-2028 年能建立的 AI 产品护城河，和"2028年之后再建"的难度完全不在同一量级。这是一个 Zico 受众——做 AI 产品、研究 AI 战略的人——真正需要思考的时间窗口问题。中文 AI 圈会报道这条消息，但会停在"Anthropic 联合创始人做了几个大胆预测"的新闻层，不会分析"60%/2028"背后的结构性含义。
- **Resonance hook**: 2026年5月21日，Anthropic 联合创始人 Jack Clark 在牛津大学 Institute for Ethics in AI 演讲：AI 将在 12 个月内协助完成诺贝尔奖级别的科学发现；AI 运营的公司将在 18 个月内产生数百万美元营收；2028年前 AI 自主设计训练下一代模型，概率 60%以上。他同时说：AI 存在"非零概率伤害所有人"的风险，这个风险没有消失。这四个预测来自同一个人，同一场演讲。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**: Zendesk 新闻稿（May 19，Relate 2026 Autonomous Service Workforce 发布）、TechRadar（May 19，Zendesk outcome-based pricing）、CMSWire（May 19，Zendesk Relate 2026 AI workforce）、diginomica（May 19，Zendesk verified resolutions）、Computer Weekly（May 19，Zendesk outcome pricing debut）；NPR（May 20，Meta 8,000 layoffs）、The Next Web（May 20，多篇，Meta layoffs + AI restructuring）、TechCrunch（May 20，Intuit 3,000 layoffs）、CNBC（May 20，Intuit Q3 earnings + CEO "nothing to do with AI"）、Yahoo Finance（May 20，Meta layoffs context）、Let's Data Science（May 20，Meta layoffs + Wang）；Resultsense（May 21，Jack Clark Oxford predictions）、TechCentral.ie（May 21，Jack Clark Nobel + AI-run companies）、Time Magazine（May 22，Jack Clark Oxford + AI safety）、Axios（May 7，Jack Clark intelligence explosion background）；llm-stats.com / aiflashreport.com（May 20-23，AI model releases tracker — no new frontier model in window beyond already-covered）；GitHub Trending（May 20-23）：RuView WiFi 空间感知（May 16-17 trending，但 GitHub project 无独立时效事件锚点）、FastGS CVPR 2026 Highlight（代码为 Nov 2025 发布，非近7天事件，排除）；arXiv（2605.10653 SAE World Congress 2026 Embodied AI insights — May 17发布，技术会议综述，无产品/发布锚点，排除）；Karpathy / Altman / Dario / Jim Fan / LeCun / Demis / Swyx（May 21-22）：无超越已选候选的独立新发言锚点（Karpathy May 19 已在5月20日 candidates 覆盖；Jack Clark May 21 = Candidate 3）；Google I/O 2026 延续报道（Antigravity 2.0 / Managed Agents on-demand）：已在5月19日 candidates Candidate 1 + 5月20-21日排除名单中，延续排除；OpenAI / Anthropic / Meta 5月20-22日后续发布更新：无独立新事件锚点（OpenAI IPO、Anthropic Q2 revenue、OpenAI Erdős 已在5月22日 candidates 覆盖）；Mustafa Suleyman "18个月白领工作全自动化"（Fortune Feb 13, 2026，超30天窗口，排除）；Cloudflare Agents Week 2026（April 13-17，超30天窗口，排除）；JPMorgan AI 核心基础设施重分类（January 2026，超30天窗口，排除）

- **Total signals found**: 18 evaluated

- **Why these 3**:
  - **Candidate 1（Zendesk Relate 2026 outcome pricing）**：时效4天（May 19），Zendesk 官方新闻稿 + TechRadar + CMSWire + diginomica 多方确认；Agent 经济柱：过去7天 candidates 完全未覆盖"企业 SaaS outcome pricing"事件（May 19-22 覆盖的是 OpenAI Erdős、Anthropic Q2、OpenAI IPO、SoftBank、Contextual AI、C2PA）；"$1.50/resolved conversation + 双重 AI 验证"是可独立验证的硬数字；"Shashi Upadhyay 原话 + Intercom $100M+ ARR on $0.99/resolution" 是两个具体可追溯锚点；中文 AI 圈对"Agent 定价单位从席位→输出量"这个结构性分析完全缺失；"验证层"（AI 验证 AI）这个产品设计问题对 Zico 受众（做 AI 产品的人）有直接操作价值。
  - **Candidate 2（Meta 8,000 + Intuit 3,000 同日裁员）**：时效3天（May 20），NPR + TechCrunch + CNBC + The Next Web 多方同日确认；组织形式变革柱：过去7天 candidates 未覆盖"AI 驱动组织结构重写"这个角度（最接近的是5月21日 Contextual AI acquihire，是人才并购角度，不重叠）；Meta $563 亿单季营收 + $1450 亿 AI 投入 + 8,000 裁员是可独立验证的三重数据组合；"'AI builder'/'AI pod lead' 职位重命名"是 Meta 的具体行动，不是泛泛战略声明；"Intuit CEO 说与 AI 无关 vs TechCrunch 说为了 AI"这个矛盾本身是可独立验证的叙事分歧（两个链接放一起就能看到）；Meta 把 7,000 人转入 AI pod 这个细节在中文媒体没有分析，报道停在"又裁员了"。
  - **Candidate 3（Jack Clark Oxford 演讲）**：时效2天（May 21），最新鲜；Resultsense + TechCentral.ie + Time Magazine（May 22）三方确认；深层思考柱：过去7天 candidates 覆盖了 OpenAI 做数学（May 22），Isomorphic Labs AI 做药物（May 20），均不重叠"AI 研究者对递归自改进时间线给出概率估计"这个角度；"2028年前60%+概率 AI 自主训练下一代"是极具体的可追溯预测，读者可验证来源；Jack Clark 是 Anthropic 联合创始人 + Import AI 创始人，在 AI 前沿研究者中可信度极高，不是 AI 焦虑贩卖者；"诺贝尔 + AI 公司 + 机器人 + 递归自改进"四个时间窗口同场出现，是对 2026-2028 产品战略最直接的参考框架；中文 AI 圈会停在"大胆预测"层，不会分析"60%/2028"背后的递归自改进工程可行性含义。

---

**Excluded signals**:
- OpenAI Erdős 80年猜想推翻（May 20）：已在5月22日 candidates Candidate 1 覆盖
- Anthropic Q2 $109 亿收入首次盈利（May 20）：已在5月22日 candidates Candidate 2 覆盖
- OpenAI IPO 秘密申报（May 21-22）：已在5月22日 candidates Candidate 3 覆盖
- Karpathy 加入 Anthropic（May 19）：已在5月20日 candidates Candidate 1 覆盖
- Google I/O 2026 延续侧面（Antigravity 2.0、Gemini 3.5 Flash GA、Managed Agents）：已在5月19日 candidates 整体覆盖，5月20-22日持续排除
- Mustafa Suleyman "18个月白领全自动化"（Fortune Feb 13, 2026）：超30天窗口
- Cloudflare 1,100 裁员 + AI 使用量增 600%（May 8）：超7天窗口（15天前），已作为 Candidate 2 背景上下文
- Cloudflare Agents Week 2026（April 13-17）：超30天窗口
- JPMorgan AI 核心基础设施重分类（January 2026）：超30天窗口
- FastGS CVPR 2026 Highlight（代码 Nov 2025 发布）：无近7天事件锚点，排除
- RuView WiFi 空间感知（May 16-17 trending）：GitHub 开源项目，无独立产品发布/时效事件锚点，弱于已选候选
- arXiv 2605.10653 SAE World Congress 2026 Embodied AI insights（May 17）：会议综述论文，无独立发布/产品锚点，排除
- Anthropic Claude for Small Business（May 13）：超7天窗口（10天前），且与 Anthropic Q2 revenue 叙事相关，被5月22日 candidates 隐含覆盖
- Meta Llama 4 消息：缺乏明确的 May 17-23 窗口内发布锚点，排除
- Swyx "Scaling without Slop" 2026 thesis：无明确时效锚点（日期不确定），排除
- Cognition AI / Agent Trace（January 2026 RFC）：超30天窗口
