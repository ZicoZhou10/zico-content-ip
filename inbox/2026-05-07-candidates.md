---
date: 2026-05-07
status: written
selected: candidate 1 → drafts/016-infra-pricing-moment-xhs.md
---

# Today's Candidates

## Candidate 1: OpenAI 把自己变成了一个 PE 基金——"The Deployment Company"用 17.5% 保底年回报圈了 190 亿

- **Event**: 2026年5月4日，OpenAI 正式宣布完成 "The Deployment Company"（内部代号 DeployCo）的资本关闭，募集规模超过 $40 亿，整体估值 $100 亿。锚定投资方为 TPG，参与方包括 Brookfield Asset Management、Advent International、Bain Capital、SoftBank、Dragoneer，合计 19 家机构投资人。OpenAI 自身注入 $5 亿初始股权，并保留追加 $10 亿的期权。结构核心细节：PE 投资人获得**五年期 17.5% 保底年化回报**（guaranteed annual return），这是软件行业几乎没有先例的承诺——基础设施（数据中心、电网）才用这种结构。交付模式：不卖软件许可证，而是向 PE 持仓的运营企业派驻 OpenAI 工程师团队，直接在客户组织内部重设工作流——Palantir 的"前向部署工程师"（Forward-Deployed Engineer，FDE）模式，规模化复制。OpenAI 持有 DeployCo 多数股权和运营控制权。The Next Web（5月4日）报道标题直接写明：DeployCo 是"2026年结构上最新颖的企业 AI 交易"。同日，Anthropic 宣布与 Blackstone、Goldman Sachs 成立平行的 $15 亿合资企业，Bain Capital 等多个 OpenAI DeployCo 投资方同时出现在 Anthropic 的名单上。
- **Source**: https://thenextweb.com/news/openai-deployco-finalized-10-billion-joint-venture | https://techcrunch.com/2026/05/04/anthropic-and-openai-are-both-launching-joint-ventures-for-enterprise-ai-services/ | https://techfundingnews.com/openai-bags-over-4b-to-build-deployment-company-with-tpg-brookfield-bain-for-enterprise-ai-rollout-report/
- **Timeliness**: 3 days ago（2026年5月4日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 中文媒体的报道重点是"OpenAI 又融了 $40 亿"，然后把 $100 亿估值和 19 家投资人列成清单，结束。但有一个细节被所有人略过：**17.5% 保底年回报**。这不是 SaaS 定价，这是基础设施定价。数据中心、光纤主干网、天然气管道才用这种结构。OpenAI 在说：AI 工程师驻场产生的价值，已经可预测到可以对外承诺保底回报——就像电网承诺稳定供电一样。这是一个巨大的认识论跨越：两年前 AI 还是"可能性工具"，今天 OpenAI 在说"回报已经可以量化承诺"。Palantir FDE 模式是关键前提。Palantir 用了十年让人相信"把工程师嵌入客户组织、深度重设流程"是可行的商业模式（当时被批为"不可扩展"）。OpenAI 现在在说：可扩展，PE 持仓的企业组合是天然的批量部署渠道——300 家 PE 持仓公司，等于 300 个并发的工程师驻场项目。更深的组织推论：如果 DeployCo 模式验证成功，AI 公司的标准商业形态会从"软件供应商"变成"嵌入式运营合伙人"——不是卖工具，是接管客户的关键业务环节。麦肯锡和埃森哲在过去 50 年里做的事，OpenAI 要用 AI 工程师在 PE 组合里重新做一遍。对做 AI 产品的人，这个结构有一个直接的产品启示：真正的企业护城河不是 API 接入，是嵌入流程之后的数据积累和切换成本。
- **Resonance hook**: OpenAI 新成立的 DeployCo 给 PE 投资人承诺了五年期 17.5% 保底年回报。这不是 SaaS 订阅，这是基础设施合同的定价逻辑。OpenAI 在说：AI 工程师嵌入你的公司产生的价值，已经稳定到可以对外承诺——就像数据中心承诺电力供应一样。AI 公司正在从软件供应商变成运营合伙人。
- **Recommended priority**: high

---

## Candidate 2: Anthropic 在 Wall Street 开了一场邀请制发布会——10 个金融 Agent 模板、Claude 接管 Excel 和 Outlook、Moody's 6 亿公司数据直接内嵌

- **Event**: 2026年5月5日，Anthropic 在纽约举办邀请制金融服务行业发布会，Jamie Dimon（摩根大通 CEO）出席并为 Claude 背书。三项核心发布：① **10 个金融工作流 Agent 模板**：面向银行、保险公司、资产管理机构和 Fintech，覆盖路演手册（pitchbook）起草、财务报表审阅、信贷备忘录（credit memo）撰写、合规升级（compliance escalation），用户可在 Anthropic Console 直接部署，无需从头搭建 Agent；② **Claude 全面接入 Microsoft 365**：Claude 可作为单一 Agent 横跨 Excel、PowerPoint、Word、Outlook 同时运行，在四个应用之间携带完整上下文——Excel 里建的财务模型自动关联到 PowerPoint 里的分析幻灯片，Outlook 里的邮件线索可以直接调用 Word 里的备忘录。Excel、PowerPoint、Word 的 Add-In 正式 GA，Claude for Outlook 进入 Beta；③ **Moody's 数据原生集成**：Moody's 将其全平台嵌入 Claude，用户无需离开 Claude 界面即可访问超过 **6 亿家公司**的信用评级和风险数据。背景：前一天（5月4日），Anthropic 与 Blackstone、Hellman & Friedman、Goldman Sachs 宣布成立 $15 亿合资企业，同时也有 Apollo Global、General Atlantic、Leonard Green、GIC、Sequoia Capital 参与，用于向中型市场企业直接派驻团队。Fortune（5月4日）、CNBC（5月4日）、Axios（5月5日）均有详细报道。
- **Source**: https://fortune.com/2026/05/04/anthropic-claude-consulting-industry-joint-venture-blackstone-goldman-sachs/ | https://www.cnbc.com/2026/05/04/anthropic-goldman-blackstone-ai-venture.html | https://fortune.com/2026/05/05/anthropic-wall-street-financial-services-agents-jamie-dimon/ | https://www.axios.com/2026/05/05/anthropic-wall-street-dimon-amodei
- **Timeliness**: 2 days ago（发布会：2026年5月5日；JV 公告：5月4日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 中文媒体把这件事报道成"Anthropic 又融了 $15 亿，进军金融"，然后结束。但产品层的三个细节被完全忽略了，而这三个细节才是 Anthropic 真正在下的棋。第一：**10 个具体工作流的 Agent 模板，不是通用 Claude**。信贷备忘录 Agent 和合规升级 Agent 是两个完全不同的场景，有完全不同的风险约束和输出格式要求。Anthropic 在说：我们不是给你一个"可以做任何事的 Claude"，我们给你一个"已经调好了信贷备忘录场景的 Claude"。这是从"水平平台"到"垂直工作流工具"的产品策略转换——Salesforce 用这个策略打败了通用 CRM，Anthropic 在复制同一个剧本。第二：**Moody's 6 亿公司数据的意义是"上下文预加载"**。金融分析师现在去 Claude 处理一个客户信用评估，不需要先解释"信用评级是什么"——Moody's 的数据已经在里面了。这是数据飞轮护城河的正确建法：不是"我的模型更聪明"，而是"用户最需要的数据已经内嵌在我的工作流里"。第三：**Microsoft 365 全栈上下文**（Excel→PPT→Word→Outlook 连通）把 Anthropic 从"对话框 AI"变成"文档层 AI"。高盛分析师的日常工作：早上看 Outlook 邮件 → 打开 Excel 建模型 → 用 PowerPoint 做展示 → 发 Word 版本报告。Claude 现在横跨这四个环节，意味着一个分析师的完整工作流可以由 Claude 串联。这不是生产力提升，这是工作流重组。
- **Resonance hook**: Anthropic 在纽约开了一场邀请制发布会，Jamie Dimon 出席背书。他们发了三样东西：10 个金融工作流 Agent 模板（包含信贷备忘录 Agent 和合规升级 Agent）、Claude 同时接管 Excel/PPT/Word/Outlook 的跨应用上下文、Moody's 6 亿公司信用数据直接内嵌进 Claude。这不是"ChatGPT 可以帮你写财务报表"——这是 AI 接管高盛分析师的完整日常工作流。
- **Recommended priority**: high

---

## Candidate 3: Google 在内部测试一个叫 Remy 的 24/7 主动型 AI Agent——Google I/O 前两周的定向泄露

- **Event**: 2026年5月6日，Business Insider 报道 Google 正在内部测试一个名为"Remy"的 AI Agent，目前处于"狗粮阶段"（dogfooding，员工内部使用测试）。Remy 的内部定义：**"your 24/7 personal agent for work, school, and daily life, powered by Gemini"**。关键特性：① **主动监控**（proactive monitoring）——Remy 不等用户发指令，而是持续监控用户关心的事项并主动行动；② **深度 Google 生态整合**：横跨 Gmail、Google Calendar、Google Docs、Google Drive、Google Keep、Google Tasks；③ **偏好学习**：随时间了解用户工作方式，调整行动策略；④ **跨域任务处理**：可同时处理工作、学校、个人生活场景，不局限于单一垂直。AI News（5月6日）补充：Google 将 Remy 定位为自己版本的 OpenClaw 替代品——"Remy elevates the Gemini app into a true assistant"。背景：Google I/O 大会预计在 2026 年 5 月下旬举行，AI Agent 被业内广泛预期为本次 I/O 的核心主题。PYMNTS（5月6日）将 Remy 与 Microsoft OpenClaw、OpenAI OpenClaw 替代方案并列，认为"Big Tech's Personal AI Agents Are Coming for the to-Do List"。Remy 当前尚无官方发布时间表，Google 未正式确认。
- **Source**: https://www.eweek.com/news/google-gemini-remy-ai-agent/ | https://www.artificialintelligence-news.com/news/google-remy-ai-agent-gemini-user-control/ | https://michaelbriancotter.wordpress.com/2026/05/06/google-tests-remy-ai-agent-for-gemini-as-focus-turns-to-user-control/
- **Timeliness**: 1 day ago（2026年5月6日）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 中文媒体会在 Google I/O 官宣后报道 Remy，写"Google 发布个人 AI Agent 挑战 Siri"，加一张功能对比图，结束。但 Remy 的核心信号在今天（I/O 前两周）比 I/O 当天更清晰：**"主动型 Agent"（proactive agent）和"被动型助理"（on-demand assistant）是两种根本不同的产品哲学**，而这个区别在 Remy 的内部定义里说得非常直白——不是"你问我答"，是"我在监控、我在行动"。现有的所有主流 AI 工具——ChatGPT、Claude、Gemini——都是被动的：用户打开对话框，输入问题，得到回答。Remy 要做的不是这个。Remy 要做的是：在你还没打开对话框之前，它已经处理好了你今天早上会遇到的三个问题。这是"环境 AI"（ambient AI）vs "工具 AI"（tool AI）的分叉点。Google 有一个独特的优势：它已经拥有用户的 Gmail（10年邮件历史）、Calendar（全部行程）、Drive（所有文档）、Maps（出行习惯）、YouTube（兴趣偏好）。Remy 不需要"学习"用户——它只需要被允许调用 Google 已经存储的关于你的所有数据。问题是：用户愿意授权吗？Google Assistant 在 2019-2021 年做过同样的尝试，失败了，原因是"功能不够强，用户不愿意给权限"。Remy 的赌注是：2026 年的 Gemini 够强了，用户会换算成新的价值方程式——"把我的数据给你 = 你替我做完我不想做的事"。这个赌注对不对，是 Google I/O 后最值得观察的实验。
- **Resonance hook**: Google 内部正在测试一个叫 Remy 的 AI Agent，内部描述是"你的 24/7 个人 Agent，处理工作、学校和生活"。它不等你发指令——它在监控，它在行动。距离 Google I/O 还有两周。ChatGPT、Claude、Gemini 现有的所有版本都是被动的：你问，它答。Remy 要做的是：在你开口之前，它已经处理完了。
- **Recommended priority**: medium（仍处于内部测试阶段，非官方发布；但时效最强、信息增量高，且 Google I/O 窗口使其时间价值高于平均）

---

## Scan summary

- **Sources scanned**: X/Twitter（Karpathy 5月6-7日无独立新锚点；Altman/OpenAI 官方博客；Demis Hassabis/Hassabis-LeCun 争论为1月 Davos 事件，超窗口；Jim Fan 无5月新锚点）、GitHub Trending（TradingAgents 金融多 Agent 框架5月4日；Agency-Agents May 2026；无单点爆发式项目）、Hacker News 2026-05-05至05-07 前页（OpenAI DeployCo 结构讨论；Anthropic Wall Street 发布；Google Remy 泄露报道；GPT-5.5 Instant 讨论延续）、OpenAI 官方（The Deployment Company finalized May 4；Bloomberg/TechCrunch/The Next Web/Business Standard 详细报道）、Anthropic 官方（Financial Services briefing May 5；Fortune/CNBC/Axios/WinBuzzer 报道链）、Google DeepMind（Genie 3 为 January 2026 项目，超7天窗口；Remy 为 Business Insider 5月6日最新报道）、arXiv cs.AI（AutoResearchBench 2604.25256，4月30日，已超3天临界且深层思考柱近期高频；Memory for Autonomous LLM Agents 综述，March 2026，超窗口）
- **Total signals found**: 18 evaluated
- **Why these 3**:
  - **Candidate 1（OpenAI DeployCo）**：时效3天（5月4日），7天窗口内；The Next Web、TechCrunch、Bloomberg 多主流媒体同日报道；17.5% 保底年回报是"发现式钩子"最强细节——可独立验证，读者能在 Bloomberg 确认，具体数字创造自我传播验证行为；组织形式变革柱：5月4日 candidates 用 Meta AI-Pods（算力 vs. 人力竞争），本篇是"AI 公司组织形态从软件供应商变成嵌入式运营合伙人"，两者逻辑方向完全不同；Palantir FDE 模式的溯源对比（Palantir 十年前被批"不可扩展"→现在 OpenAI 规模化复制）构成反共识自白式钩子；中文圈将"$40 亿融资"和"17.5% 保底"混为一谈，后者的组织论文含义几乎零覆盖。
  - **Candidate 2（Anthropic Wall Street）**：时效2天（5月5日发布会），Fortune/CNBC/Axios 同日报道；AI 产品战略柱：5月5日 candidates 用 GPT-5.5 Instant 默认模型（OpenAI 产品哲学），本篇是 Anthropic 的垂直 Agent 模板策略 + 数据生态建法，两者不同公司、不同产品层、不同角度，无重叠；"10 个具体工作流 Agent 模板"是可验证的产品发现式锚点（用户可以去 Anthropic Console 查）；Moody's 6 亿公司数据内嵌 + Microsoft 365 跨应用上下文是信息增量最高的细节，中文媒体均未拆解；$15 亿 JV（5月4日）+ 10 个 Agent 模板（5月5日）构成"分发渠道 + 产品武器"双层论证结构，叙事完整。
  - **Candidate 3（Google Remy）**：时效最强（1天，5月6日），AI News/eWeek/PYMNTS 同日报道；Agent 经济柱：5月5日 candidates 用 AWS Connect 垂直 Agent 产品线（企业 B2B），本篇是"主动型个人 Agent 的 C 端范式"，方向完全不同；"主动监控 vs. 被动问答"框架是最清晰的产品哲学切分点——ChatGPT/Claude/Gemini 现有版本全部被动，Remy 主动；Google I/O 两周前的泄露意味着内容的时间窗口极高（I/O 公告后中文媒体会大量跟进，Zico 在此时输出信息差分析是最优时机）；Google Assistant 2019-2021 失败史与 Remy 的相似赌注构成反直觉叙事线索。

- **Excluded signals**:
  - Anthropic Pentagon 排除（5月1日）：5月6日 candidates Candidate 1 已完整覆盖，排除
  - GPT-5.5 Instant 默认模型（5月5日）：5月6日 candidates Candidate 2 已覆盖，排除
  - Musk xAI 蒸馏承认（4月30日）：5月6日 candidates Candidate 3 已覆盖，排除
  - Musk v. Altman Week 2 / Brockman 证词（5月5-6日）：5月6日 candidates 同一庭审（Week 1 已选为 draft 009），Brockman 证词是戏剧细节（Musk 借调 OpenAI 员工给 Tesla/Autopilot 团队工作；Brockman $300 亿股权但从未捐款）—— 有趣但中文媒体覆盖已达饱和，且此前三天已用庭审两次，排除
  - Google DeepMind Genie 3（January 2026 项目，部分 Ultra 用户 2026年1月29日可访问）：超出7天窗口，排除
  - Karpathy "99.9% of web content will be AI-optimized"（LLM Wiki 相关，April 3 2026）：约34天前，超窗口；Karpathy AI 协作实践柱已在5月5日 candidates 覆盖 Agentic Engineering 框架（近期使用），排除
  - TradingAgents GitHub trending（5月4日，TauricResearch 多 Agent 金融交易框架）：可验证锚点弱，无单点事件触发，与 Candidate 2 Anthropic 金融 Agent 话题高度重叠，排除
  - AutoResearchBench arXiv 2604.25256（4月30日）：深层思考柱近期高频（5月3-5日均有使用），且无 Zico 独特视角切入点，排除
  - LeCun/Hassabis AGI 争论（1月 Davos）：约3个半月前，远超窗口，排除
