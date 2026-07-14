---
date: 2026-07-14
status: written
selected: candidate 2 → drafts/075-deployment-paradox-xhs.md
---

# Today's Candidates

## Candidate 1: Google、Microsoft、Salesforce、Snowflake、ServiceNow 联手推出 ARD 标准对抗 Anthropic MCP——五大企业软件巨头不愿把 AI 时代的"水管"交给竞争对手（July 12）

- **Event**: 2026年7月12日，The Information 独家报道：**Google、Microsoft、Salesforce、Snowflake、ServiceNow** 正式表态支持 **ARD（Agentic Resource Discovery）** 标准，明确将其定位为对抗 **Anthropic MCP（Model Context Protocol）** 的替代方案。ARD 规范由 Google 于 6月17日联合 Microsoft、Hugging Face 发布（技术支持方还包括 Amazon、Cisco、GitHub、Nvidia），但 Snowflake 和 ServiceNow 的正式背书及"反 MCP"叙事框架，由 The Information 在7月12日率先建立。背景：Anthropic 于 2024年11月发布 MCP，定义 AI Agent 如何连接企业数据和工具——**过去18个月内 MCP 已成为 AI Agent 接入企业系统的默认协议**。五大联盟公司共同控制的企业软件覆盖：Salesforce（CRM）、Snowflake（企业数据仓库）、ServiceNow（企业工作流）、Microsoft Azure、Google Cloud——几乎涵盖企业数据流向的所有关键节点。
- **Source**: https://unrot.co/blogs/today-top-10-ai-news-july-13-2026（引用 The Information 2026年7月12日独家） | https://cryptobriefing.com/ard-ai-standard-google-microsoft-salesforce/ | https://www.searchenginejournal.com/google-microsoft-back-draft-ai-agent-discovery-spec/579894/ | https://commandline.microsoft.com/agentic-resource-discovery-specification-ard/ | https://amdatalakehouse.substack.com/p/the-state-of-agentic-ai-standards
- **Timeliness**: 2天前（2026年7月12日，The Information 独家；7月13日 BuildFastWithAI / unrot.co 跟进报道）
- **Topic pillar**: AI产品战略
- **Zico's angle**: MCP 的护城河不是技术，是生态密度。Anthropic 把 MCP 做成默认协议的速度比任何人预期的都快：从2024年11月发布，到成为"AI Agent 接入企业工具的默认方式"，只用了18个月。这是一个典型的平台赢家信号——当竞争对手需要组成五家联盟才能应对你，说明你已经占住了有战略意义的协议层位置。

  但这个联盟的性质很特别，值得拆开看。ARD 和 MCP 在技术上定位不同：MCP 解决"Agent 如何连接工具和数据"，ARD 解决"Agent 如何跨组织发现彼此能力"——理论上互补。五家公司同时背书 ARD 并把它定性为"反 MCP"，是政治信号大于技术需求。他们真正担心的是：**Anthropic 的协议如果持续扩散，企业 AI 基础设施的入口就由一家模型公司控制了**，而 Salesforce/Snowflake/ServiceNow/Microsoft/Google 的护城河恰好建立在"企业数据流经我这里"这件事上。

  这件事的框架性意义：AI 产品战略的下一个竞争不在模型，在协议控制权。Google A2A（2024）、Anthropic MCP（2024年11月）、ARD（2026年6月）——三个协议，三方势力，争夺同一个位置：成为 AI Agent 时代的 TCP/IP。Anthropic 的优势是"先发的生态密度"；劣势是没有 Salesforce 和 ServiceNow 那种企业数据分发渠道。现在五大企业软件公司在说：AI 时代的水管，不归你管。

  Zico 的视角：在 酷家乐 做 AI 产品时，我们实际上是 MCP 的使用方——我们需要决定把 Agent 接入哪套协议。这件事直接影响产品选型：押 MCP 还是等 ARD？这不是技术决策，是政治押注。

- **Resonance hook**: 7月12日，The Information：Google、Microsoft、Salesforce、Snowflake、ServiceNow 组成联盟，正式背书 ARD 标准——目标是替代 Anthropic MCP。18个月前，MCP 还不存在。现在，控制全球大多数企业数据流向的五家公司——CRM、数据仓库、工作流、两朵最大的云——需要联手推出替代方案。Anthropic 最大的战略胜利，触发了最大的联盟反应。AI Agent 时代的基础协议之战，正式开始。
- **Recommended priority**: high

---

## Candidate 2: OpenAI Deployment Company 收购 Northslope——复制 Palantir "前向部署工程师"模式，把人嵌进企业内部（July 8）

- **Event**: 2026年7月8日，Axios 独家报道：**OpenAI Deployment Company**（2026年5月成立，$40亿启动资金）宣布收购应用 AI 公司 **Northslope**，这是 OpenAI Deployment Company 成立以来的第二笔收购（首笔为 Tomoro）。Northslope 创始团队来自 **Palantir**，核心业务是 FDE（Forward-Deployed Engineer，前向部署工程师）——把工程师直接嵌入客户组织内部，帮助企业在实际运营场景中构建 AI 系统。收购后，OpenAI Deployment Company 的 FDE 团队规模将扩大至**数百人**。Terms 未披露。此前 OpenAI 已在 5月将 $40亿专用资本配置到 Deployment Company，用于收购和扩张企业 AI 部署能力。The Next Web 标题直接点出核心：**《OpenAI buys Northslope to sell AI adoption, not models》**。Palantir 的 FDE 战略是其企业护城河的核心来源——工程师深度嵌入政府和企业内部，使其软件难以被替换，不是因为技术更好，而是因为"工程师已经和组织融合了"。
- **Source**: https://www.axios.com/2026/07/08/openai-deployment-company-northslope-acquisition | https://thenextweb.com/news/openai-northslope-acquisition-enterprise-ai-deployment | https://app.dealroom.co/news/feed/openai-deployment-arm-acquires-northslope-to-expand-enterprise-ai-implementation-services
- **Timeliness**: 6天前（2026年7月8日，Axios 独家）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: The Next Web 的标题道出了这件事的真实逻辑：**OpenAI 卖的不是模型，是 AI adoption（采用）**。这个区别比表面看起来重要得多。

  先还原 Palantir 的 FDE 模式为什么有效。Palantir 的核心竞争力从来不是软件——是把工程师嵌入客户内部，理解操作场景，在里面建系统这件事本身。嵌进去之后，工程师理解了业务流程，建了定制化工具，这时候"换一个供应商"的成本变成了"重新培训一套懂我业务的工程师"。这是结构性锁定，不是技术锁定。

  OpenAI 现在在复制这个逻辑。它的判断是：**模型能力达到一定门槛之后，阻碍企业真正用好 AI 的瓶颈不是模型能力，而是部署能力**——怎么把 AI 接进现有工作流，怎么处理历史数据，怎么让非技术部门的人真正用起来。这些问题不能靠 API 文档解决，需要人坐在客户旁边一起搞。

  这件事对 Zico 的组织形式变革框架有一个直接的反直觉含义：AI 越强，"用好 AI"这件事反而越需要专业人力——不是开发者，而是懂业务流程的部署工程师。**AI automation 不减少服务人力，它重新定义了服务人力的类型**。OpenAI 收购 Palantir 出身的团队，是对这个判断的最直接押注。

  中文媒体会报"OpenAI 收购企业AI公司"，不会分析：**这是 AI 公司承认"卖模型"不够，需要复制 Palantir 20年打磨的"嵌入式服务"护城河——而嵌入式服务的本质是靠人的深度驻扎，不是靠技术壁垒。**

- **Resonance hook**: 7月8日，Axios：OpenAI Deployment Company 收购了一家由 Palantir 人创办的公司，叫 Northslope，专门做 FDE——把工程师嵌入企业内部，帮企业真正部署 AI。The Next Web 的标题：OpenAI buys Northslope to sell AI adoption, not models。Palantir 的护城河从来不是软件，是"工程师嵌进了你的组织"这件事本身。OpenAI 现在决定复制这个模式。AI 越强，在企业内部"如何真正用好"反而变成了更大的瓶颈——这是 OpenAI $40亿 Deployment Company 和今天这笔收购背后的判断。
- **Recommended priority**: high

---

## Candidate 3: 美国空军备忘录：承包商须在9月1日前清除 Anthropic 所有产品——Anthropic 在起诉美国政府以保住"不用于自主武器"的红线（July 9）

- **Event**: 2026年7月9日，**Breaking Defense** 获得内部备忘录并率先报道：美国空军研究实验室（**AFRL**）向所有承包商发出指令，要求在 **2026年9月1日** 前从系统中清除全部 Anthropic 产品——比国防部全系统清除 Anthropic 的最终期限（9月底）**提前近一个月**。背景：Anthropic 在 2025年7月与五角大楼签署了价值 **$2亿**、为期两年的合同，成为第一家将前沿 AI 模型接入保密网络的 AI 实验室。合同中，Anthropic 坚持保留两条"红线"：（1）Claude 不得用于**大规模监控美国公民**；（2）不得用于**无人干预、能自主选择并攻击目标的武器系统**。五角大楼要求删除这两条限制，Anthropic 拒绝，五角大楼随即对 Anthropic 发出**"供应链安全风险"指定令**——这是美国历史上**首次对本国企业发出此类指定令**。目前 Anthropic 正在通过法律途径起诉政府撤销该指定令，临时禁令目前仍然有效。同期，华尔街日报（WSJ）报道了五角大楼与 Anthropic 高管私信通讯内容的大量泄露。The Hill、CBS News 同日跟进报道。
- **Source**: https://breakingdefense.com/2026/07/air-force-pushing-contractors-to-purge-anthropic-by-sept-1-memo/ | https://thehill.com/policy/defense/5778840-pentagon-anthropic-ai-dod-hegseth/ | https://www.cbsnews.com/news/pentagon-ai-anthropic-memo-remove-from-key-systems/ | https://en.wikipedia.org/wiki/Anthropic%E2%80%93United_States_Department_of_Defense_dispute
- **Timeliness**: 5天前（2026年7月9日，AFRL 备忘录发出；Breaking Defense / The Hill / CBS News 同日多家一线媒体报道）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: 这件事值得说的不是"AI 公司和军方吵架"。值得说的是：**Anthropic 在捍卫的那两条红线，已经成为一次公开的压力测试——验证 AI 安全原则在主权压力下还能否存在。**

  先把事件的结构说清楚。Anthropic 的可接受用途政策明确禁止两件事：大规模监控本国公民、完全自主的致命武器（无人在回路）。五角大楼想要一个"任何合法用途"的合同条款，本质上是要取消这两条限制。Anthropic 拒绝——不是战略原因，是原则原因。五角大楼的回应不是"那我们换个供应商"，而是**把 Anthropic 定为国家安全供应链风险**——历史上第一次对本国公司使用这个武器。然后 Anthropic 起诉了政府。

  这是 AI 安全原则遭遇最大外部压力的公开案例，比任何学术研究或评级体系都更真实。FLI 的 AI 安全指数（7月7日）测量的是自愿披露下的安全承诺——Anthropic 最高分 C+，但自愿承诺的可信度是存疑的。空军清除令是一个不同量级的压力：**当拒绝自主武器原则的代价是失去$2亿合同并被政府列为安全威胁，AI 公司还会坚持吗？**

  Anthropic 的回答目前是：会。但这场博弈还没结束。如果法院判决对政府有利，会有压力让 Anthropic 妥协；如果 Anthropic 胜诉，这将成为一个先例：AI 安全原则能在主权压力下存活。两种结局都是 AI 治理史上的节点。

  对 Zico 的"AI 作为新物种"框架：一个新物种如果不能对使用自己的"规则"说不，它在权力结构中只是工具。Anthropic 正在测试一个命题：AI 公司能否在行为层面拥有原则，而不是只在文件里拥有原则。

  中文媒体会报"美国 AI 公司和政府闹翻"，不会问：**当一家 AI 公司拒绝让超级大国的军队用它的模型，并且被列为国家安全威胁、起诉政府——这是 AI 安全原则在最硬的环境里的第一次实战，结果将决定未来所有 AI 公司在面对主权客户时的谈判边界。**

- **Resonance hook**: 7月9日，美国空军研究实验室向所有承包商发备忘录：9月1日前，清除系统中所有 Anthropic 产品。背后原因：Anthropic 不肯让 Claude 用于自主武器，拒绝了五角大楼的合同修改要求——五角大楼把 Anthropic 列为"国家安全供应链风险"。这是美国历史上第一次对本国企业使用这个定性。Anthropic 的回应：起诉美国政府。拒绝自主武器的代价是失去 $2亿合同，被列为国家威胁，被逼出军方系统。这是 AI 安全原则在最硬环境里的第一次实战，不是白皮书，不是评级——是法庭和备忘录。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**:
  - unrot.co（2026年7月13日，《Top 10 AI News July 13 2026》——引用 The Information 2026年7月12日独家关于 ARD vs MCP 联盟）
  - BuildFastWithAI（2026年7月13日，《AI News Today July 13 2026: 15 Biggest Stories》）
  - CryptoBriefing（《Google, Microsoft, and Salesforce back new AI software standard to counter OpenAI and Anthropic》）
  - SearchEngineJournal（《Google, Microsoft Back Draft AI Agent Discovery Spec》）
  - Microsoft Command Line（《Introducing the Agentic Resource Discovery specification》，2026年6月17日 ARD 发布）
  - amdatalakehouse Substack（《The State of Agentic AI Standards in 2026: MCP, A2A, WebMCP, OSI》）
  - Axios（2026年7月8日，独家，《OpenAI deployment arm to acquire Northslope》）
  - The Next Web（《OpenAI buys Northslope to sell AI adoption, not models》）
  - Dealroom.co（OpenAI Northslope 收购报道）
  - Breaking Defense（2026年7月9日，《Air Force pushing contractors to purge Anthropic by Sept. 1: Memo》）
  - The Hill（2026年7月9日，《Military commanders given deadline to remove Anthropic products》）
  - CBS News（2026年7月9日，《Internal Pentagon memo orders military commanders to remove Anthropic AI technology from key systems》）
  - Wikipedia（《Anthropic–United States Department of Defense dispute》——背景梳理）
  - Nvidia RAISE Summit 2026 官方页面（Jim Fan 7月8日演讲——主体内容为"VLAs are dead / World Action Model"，但确认 Jim Fan 的核心 WAM 论点首发于 Sequoia AI Ascent 2026（4月30日），超出7天窗口，排除）
  - eventual.ai（《VLAs are dead, long live World Action Models》——总结 Jim Fan 旧话题，时效不足，排除）
  - Hacker News 2026年7月12日 front page（#21 Nvidia/CoreWeave/Nebius circular financing——信号较强但为金融结构分析，无清晰产品战略角度，排除）
  - Bloomberg（2026年7月2日，《OpenAI proposes giving US government a 5% stake》——超出7天窗口12天，排除）
  - TechTimes（2026年7月4日，《Pentagon Blacklisted Anthropic》首发——10天前，超出7天窗口；但7月9日 AFRL 备忘录为新事件，在窗口内）
  - OpenAI GPT-Live（2026年7月8日，TechCrunch 报道——信号强但7月11日已评估排除过（该日候选scan中提到GPT-Live），且属 AI协作实践柱，今日三选均有更强替代）
  - Anthropic Claude Corps（$150M，1000 fellows，$85K/年，Forbes 6月18日主发布——超出7天窗口，Spectrum Local News 7月9日补充报道信号较弱，排除）
  - Meta Watermelon 匹配 GPT-5.5（时间锚点不明确，排除）
  - Chinese AI 模型30-46% US企业 API 流量（7月9日/7月12日候选scan中已被覆盖，排除）

- **Total signals found**: 约22个信号评估

- **Why these 3**:
  - **Candidate 1（ARD vs MCP 企业软件联盟，7月12日 The Information）**：**AI产品战略柱**——过去3天该柱覆盖为：Apple vs OpenAI 硬件商业机密（7月13日）、微软 MAI 替换 Anthropic/OpenAI（7月12日）、ChatGPT Work 产品架构（7月11日）。今日角度完全不同：协议层控制权争夺（不是硬件、不是成本路由、不是产品形态）；五大企业软件公司联盟对抗 Anthropic 协议生态是本周最大 AI产品战略新闻；信息差极大（中文媒体不会把"MCP 已成企业默认协议"和"五大公司反制"放在同一个分析框架里）；The Information 独家，7月13日多家跟进；**HIGH 优先级**。
  - **Candidate 2（OpenAI Northslope FDE 模式，7月8日 Axios）**：**组织形式变革柱**——过去3天该柱仅7月12日覆盖（美联储 Andreessen AI生产力任务组），今日角度完全不同（宏观货币政策 vs. 企业 AI 部署组织模式）；Palantir FDE 模式是理解 OpenAI 这次收购的唯一正确框架，而中文媒体几乎不会用这个框架；The Next Web 标题直接点出核心："OpenAI 卖的不是模型，是 adoption"；与 Zico 的"AI-Native 组织三阶段"框架直接共鸣（过渡期需要大量人工嵌入）；6天前，在7天窗口内；**HIGH 优先级**。
  - **Candidate 3（美国空军 AFRL 清除 Anthropic 备忘录，7月9日 Breaking Defense）**：**深层AI思考柱**——过去3天该柱覆盖为：FLI AI安全指数 C+（7月11日）、人形机器人三重 IPO（7月12日）；今日角度完全不同且更激烈：不是评分、不是资本市场定价，而是 AI 安全原则遭遇最强现实压力（主权政府 + 百亿合同）；Anthropic 在起诉美国政府这件事本身是最强的"AI 安全原则实战"数据点；Breaking Defense + The Hill + CBS News 三路来源，5天前；与 Zico 的"AI 作为新物种能否有原则"框架深度共鸣；中文媒体只会报"美军封禁 Anthropic"，不会分析"这是 AI 安全原则在主权压力下的第一次边界测试"；**HIGH 优先级**。
  - 三者覆盖三个不同主题柱（AI产品战略 / 组织形式变革 / 深层AI思考），时效性均在7天窗口内（2天 / 6天 / 5天），与过去3天已入选/已评估的候选无重叠。
