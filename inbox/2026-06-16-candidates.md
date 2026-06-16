---
date: 2026-06-16
status: pending_selection
---

# Today's Candidates

## Candidate 1: OpenAI 正式推出 Partner Network——$150M 押注"实施能力"，Accenture / McKinsey / BCG / Bain / PwC 同日入伙，300,000 认证顾问目标，官方宣告模型能力已不再是企业 AI 采用的主要障碍（June 14）

- **Event**: 2026年6月14日，OpenAI 正式发布 **OpenAI Partner Network**，投入 **$150M** 建立首个正式企业渠道计划。发布首日合作伙伴包括 **Accenture、Bain & Company、BCG、McKinsey & Company、PwC**，以及 Artium、Eliza 等，横跨管理咨询、系统集成、数据和技术服务。计划架构：三级合作体系（Select / Advanced / Elite），可在 Codex、网络安全、API、Agent 转型等专项中获得认证；年底目标：认证 **300,000 名顾问**。差异化机制：**Forward Deployed Experts（FDE）** 试点——OpenAI 工程师直接嵌入合作伙伴团队，与 Anthropic 现行合作计划不同。OpenAI 在官方新闻稿中写明：**"advances in model capabilities are no longer the primary barrier to enterprise AI adoption"**（模型能力的进步不再是企业 AI 采用的主要障碍）。背景：今年 2 月 23 日，OpenAI 曾与 McKinsey、BCG、Accenture、Capgemini 签署战略联盟协议（Frontier Alliance），本次 Partner Network 是从战略协议升级为标准化渠道体系。来源：**OpenAI 官方**（June 14）、**TechTimes**（June 15，《OpenAI Launches Partner Network: $150M Bet That Implementation Beats Model Power》）、Dataconomy、TipRanks、FourWeekMBA（《The Model Wars Are Over, the Harness Wars Just Started》）。
- **Source**: https://openai.com/index/introducing-openai-partner-network/ | https://www.techtimes.com/articles/318436/20260615/openai-launches-partner-network-150m-bet-that-implementation-beats-model-power.htm | https://dataconomy.com/2026/06/15/openai-launches-150-million-partner-network/ | https://fourweekmba.com/openai-partner-network-harness-wars/
- **Timeliness**: 2天前（2026年6月14日 OpenAI 官方发布；6月15日 TechTimes 等多方报道）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: OpenAI 在自己的新闻稿里说了一句很反常识的话：模型能力进步不再是企业 AI 采用的主要瓶颈。这句话出自一家以模型能力著称的公司，是值得细看的自我定位转变。

  OpenAI 现在的竞争策略越来越像一家渠道公司，不是一家模型公司。Partner Network 是 Salesforce 式的合作伙伴体系：咨询公司按等级排排坐，年度销售量、技术能力、联合销售次数决定你在哪个档位。Salesforce 用这个模型统治了 CRM 市场二十年。OpenAI 要拿这个工具打企业 AI 的最后一公里。

  McKinsey、BCG、Bain 同时加入同一个 Partner Network 是不寻常的。这三家通常不出现在同一家供应商的发布会上——因为它们在企业客户那里是互相竞争的顾问。OpenAI 把它们打包进同一个发布，暗示在 AI 实施这件事上，OpenAI 不认为顾问公司之间的竞争是核心问题，核心问题是让所有顾问都懂得怎么卖 OpenAI。

  Forward Deployed Experts 是这个计划里最值得关注的细节：OpenAI 工程师直接嵌入合作伙伴客户现场。这是 Stripe 当年打企业市场的路数——不是发文档，是派人。派人很贵，也很有效。这意味着 OpenAI 认为当前 AI 落地的主要问题不是文档不够好，是企业没有人能把这个东西真正用起来。

  但有一个问题 OpenAI 在发布里没回答：Accenture、McKinsey、BCG、Bain 同时也是 Anthropic 和 Google 的合作伙伴。这些咨询公司对任何一家 AI 供应商都不具有排他性。OpenAI 用 $150M 买到的是认证优先级和 FDE 嵌入资格，不是排他渠道。Anthropic 已经在企业份额上反超 OpenAI（Ramp 数据：41% vs 39.5%）——Partner Network 是 OpenAI 对这个趋势的正式回应。

- **Resonance hook**: 6月14日，OpenAI 花 $150M 发布了一个官方渠道计划，把 Accenture、McKinsey、BCG、Bain、PwC 同日打包进发布名单。新闻稿里有一句话值得单独拎出来看："模型能力的进步，不再是企业 AI 采用的主要障碍。" OpenAI 自己说的。300,000 名认证顾问目标，Salesforce 三级体系，OpenAI 工程师直接嵌入客户现场的 Forward Deployed Experts 试点。模型战争那一页，OpenAI 认为已经翻过去了。
- **Recommended priority**: high

---

## Candidate 2: NVIDIA Cosmos 3 正式发布——首个 Physical AI 开源全模态模型（文字 / 图像 / 视频 / 环境音 / 动作序列），双塔架构统一推理与生成，将机器人训练周期从数月压缩至数天（June 1）

- **Event**: 2026年6月1日，NVIDIA 在 **GTC Taipei / Computex 2026** 正式发布 **Cosmos 3**，同日宣布 **Isaac GR00T Reference Humanoid Robot**（参考人形机器人平台）。**Cosmos 3** 是全球首个为 Physical AI 而生的开源全模态模型（Open Omnimodel），两个主力变体同日发布：**Cosmos 3 Nano**（16B参数，8B Reasoner + 8B Generator）和 **Cosmos 3 Super**（64B参数，32B + 32B），另有 2B 的 **Cosmos 3 Edge** 变体宣布后续推出。技术架构：**Mixture-of-Transformers（MoT）双塔设计**——Reasoner Tower（自回归视觉语言模型，负责理解图像/视频/文字中的运动、物体交互、时空关系）+ Generator Tower（扩散模型，负责生成物理准确的视频和动作输出）。五种模态（文字、图像、视频、环境音、动作序列）+ 五种使用模式（文字生成视频、VLM推理、前向动态建模、逆向动态建模、动作策略生成）共存于单一架构。核心指标：机器人 sim-to-real 训练周期从**数月压缩至数天**；在 Physics-IQ、PAI-Bench、R-Bench（世界生成）和 RoboLab、RoboArena（动作策略）等基准上均排名开源第一。**Isaac GR00T Reference Humanoid Robot**：集成 Unitree H2 Plus 底盘 + Sharpa Wave 五指触觉手 + NVIDIA Jetson Thor 板载计算，**75 个自由度**，五大机构首批承诺采用：**斯坦福大学、ETH Zurich、Allen Institute for AI、UC San Diego ARCL、NVIDIA Research**。来源：**NVIDIA 官方博客**（June 1）、HPCwire（June 1，《NVIDIA Launches Cosmos 3, the Open Frontier Foundation Model for Physical AI》）、Interesting Engineering（《NVIDIA launches Cosmos 3, chip-fab tools and humanoid robot platform》）、Hugging Face 官方（《Welcome NVIDIA Cosmos 3》）、Jim Fan LinkedIn（"2026 will go down in history as the first year that Large World Models lay real foundations for robotics"）。
- **Source**: https://blogs.nvidia.com/blog/nvidia-gtc-taipei-computex-2026-news/ | https://www.hpcwire.com/aiwire/2026/06/01/nvidia-launches-cosmos-3-the-open-frontier-foundation-model-for-physical-ai/ | https://huggingface.co/blog/nvidia/cosmos-3-for-physical-ai | https://interestingengineering.com/ai-robotics/nvidia-physical-ai-cosmos3-humanoid-robots-tsmc | https://www.humanoidsdaily.com/news/nvidia-gtc-nvidia-and-sharpa-unveil-isaac-gr00t-reference-humanoid-robot
- **Timeliness**: 15天前（2026年6月1日 NVIDIA 官方 GTC Taipei 正式发布；Cosmos 3 权重 5月31日上线）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: 以前做机器人需要四个分开的模型：Cosmos Predict（世界生成）、Cosmos Transfer（条件生成）、Cosmos Reason（场景理解）、Cosmos Policy（动作策略）。Cosmos 3 把这四件事放进了一个架构。这不只是工程上的简化，是一个关于"理解和行动是否应该分离"的架构判断。

  双塔设计是这个判断的物化：Reasoner Tower 负责"搞清楚发生了什么"，Generator Tower 负责"决定接下来做什么/生成接下来会发生什么"。两个塔共享同一套对物理世界的理解，Reasoner 的输出直接作为 Generator 的条件。机器人看到一个物体，Reasoner 理解它的物理属性（重量、材质、运动轨迹），Generator 输出对应的抓取动作序列。这两件事以前在两个分开的模型里发生，现在在一个模型的两个子塔里发生。训练时它们共享 world representation，推理时它们共享中间特征——这是 sim-to-real 误差消失的根本原因：因为用来生成仿真环境的 world model 和用来决策动作的 policy model 现在是同一套 world model。

  对做 3DGS 和空间 AI 的人，Cosmos 3 还有一个更深的含义：它的视频输入可以是任意视角的场景录像，这意味着 3DGS 渲染出的合成视角可以直接作为 Cosmos 3 的训练数据。你在 NeRF/3DGS 里建好一个场景，用 Cosmos 3 Generator 生成这个场景里机器人的动作视频，再用 Cosmos 3 Reasoner 解析动作并生成 policy——这是一条从空间表示到机器人行为的完整链路，以前每个环节都需要独立的模型和工程对接。

  Jim Fan 说 2026 年是大世界模型为机器人学奠基的第一年。Cosmos 3 是那个基础层。

- **Resonance hook**: 6月1日，NVIDIA 在 GTC Taipei 发布 Cosmos 3：单一模型，同时处理文字、图像、视频、环境音、机器人动作序列，可同时作为输入和输出。以前做一个机器人 AI 系统要对接四个分开的模型；现在一个模型做完四件事。机器人仿真训练周期：从数月缩短到数天。斯坦福、ETH Zurich、Allen Institute、UC San Diego 和 NVIDIA Research 五家机构第一批承诺采用 Isaac GR00T Reference Humanoid。Jim Fan（NVIDIA Physical AI 负责人）说：2026 年将是大世界模型真正为机器人学奠基的第一年。
- **Recommended priority**: high

---

## Candidate 3: Anthropic Project Glasswing 扩展至 15 国 150 家关键基础设施机构——Mythos 在电力 / 水务 / 医疗 / 通信网络中自主运行，已找到 10,000+ 高危漏洞，AI Agent 首次成为关键基础设施的安全守门人（June 2）

- **Event**: 2026年6月2日，Anthropic 官方发布《Expanding Project Glasswing》，宣布将 **Project Glasswing** 扩展至超过 **150 家新机构**，覆盖 **15 个以上国家**。新增行业：电力、水务、医疗、通信、硬件（初始阶段未覆盖的领域）。Project Glasswing 的机制：向被选中的关键基础设施机构提供 **Claude Mythos Preview** 早期访问权，让它们的安全团队使用 Mythos 自主扫描代码库，寻找高危安全漏洞。截至发布时的累计数字：合作伙伴通过 Mythos 发现的高危或严重漏洞超过 **10,000 个**；另外，Mythos 在开源代码中独立发现了近 **3,900 个**高危或严重漏洞。Mythos 在某些场景下持续自主运行数周，充当自动化漏洞猎手。来源：**Anthropic 官方**（《Expanding Project Glasswing》、《Project Glasswing: An Initial Update》）、**CNBC**（June 2，《Anthropic expands Mythos to 150 additional organizations in more than 15 countries》）、**TechCrunch**（June 2，《Anthropic scales Claude Mythos to critical infrastructure in 15 countries》）、Cybersecurity Dive（《Anthropic shares Mythos with 150 more organizations, including critical infrastructure operators》）。
- **Source**: https://www.anthropic.com/news/expanding-project-glasswing | https://www.cnbc.com/2026/06/02/anthropic-mythos-ai-project-glasswing.html | https://techcrunch.com/2026/06/02/anthropic-scales-claude-mythos-to-critical-infrastructure-in-15-countries/ | https://www.cybersecuritydive.com/news/ai-anthropic-claude-mythos-project-glasswing-expand/821714/
- **Timeliness**: 14天前（2026年6月2日 Anthropic 官方 + CNBC + TechCrunch 发布）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 10,000+ 高危漏洞是一个数字，也是一个劳动力替代的信号。一家顶级安全机构的渗透测试团队，一年能发现多少高危漏洞？几十个，能到三位数已经是顶尖团队。Mythos 在 Glasswing 合作伙伴里发现了 10,000+，开源代码里另找了 3,900 个，还在以数周为单位持续运行。这不是 AI 辅助安全分析师工作，是 AI Agent 作为独立生产单元在运转。

  Agent 经济的讨论大多数停留在"AI 帮你写代码""AI 帮你查资料"的层面。Project Glasswing 代表的是另一个量级：Mythos 在电力网、水务系统、医疗基础设施的代码库里自主工作，发现的每一个漏洞都是一个潜在灾难的预防。Mythos 不是生产力工具，是安全基础设施的一部分。

  Glasswing 背后有一个 Anthropic 不太说明但很清楚的逻辑：最先让 Mythos 看到最敏感系统的人，最能影响 Mythos 下一步的训练方向。让关键基础设施团队用 Mythos 做安全扫描，Anthropic 在建立一个超出消费市场的、和真实高价值系统深度绑定的数据和信任积累。这是企业护城河的早期形态，不只是 CSR。

  还有一个反差值得拎出来：6月2日 Anthropic 宣布 Mythos 保护全球 15 国关键基础设施；6月12日，美国商务部要求 Anthropic 全球关闭 Fable 5 和 Mythos 5。同一个模型，既是被 15 国信任的安全守门人，又是被美国政府出口管制的对象。Agent 经济的政治学开始出现了。

- **Resonance hook**: 6月2日，Anthropic 宣布 Project Glasswing 扩展到 15 个国家、150 家机构，覆盖电力、水务、医疗、通信网络。Claude Mythos 在这些系统的代码库里已经自主运行了一段时间，找到了 10,000 个以上的高危漏洞——开源代码另外还有 3,900 个。顶尖渗透测试团队一年能找到几十个。Mythos 在做同一件事，只是以不同的速度和规模。10天后，美国商务部要求 Anthropic 关闭 Mythos 5。
- **Recommended priority**: medium

---

## Scan summary

- **Sources scanned**:
  - TechCrunch AI category（June 2026 最新文章扫描）
  - VentureBeat（June 14-16 最新 AI 报道）
  - OpenAI 官方（《Introducing the OpenAI Partner Network》，June 14）
  - TechTimes（June 15，《OpenAI Launches Partner Network: $150M Bet That Implementation Beats Model Power》）
  - Dataconomy（June 15，《OpenAI Unveils First Official Partner Program With $150M Backing》）
  - FourWeekMBA（《The Model Wars Are Over, the Harness Wars Just Started》）
  - TipRanks（《OpenAI Launches $150 Million Partner Network》）
  - Pulse2（《OpenAI Launches A Partner Network》）
  - NVIDIA 官方博客（June 1，GTC Taipei Computex 2026 发布）
  - HPCwire（June 1，《NVIDIA Launches Cosmos 3, the Open Frontier Foundation Model for Physical AI》）
  - Hugging Face 官方（《Welcome NVIDIA Cosmos 3: The First Open Omni-model for Physical AI》）
  - Interesting Engineering（《NVIDIA launches Cosmos 3, chip-fab tools and humanoid robot platform》）
  - Humanoids Daily（《NVIDIA GTC: NVIDIA and Sharpa Unveil Isaac GR00T Reference Humanoid Robot》）
  - DataNorth（《NVIDIA Launches Cosmos 3: Open Physical AI Omnimodel》）
  - Jim Fan LinkedIn / NVIDIA GEAR Lab（"2026 will go down in history as the first year that Large World Models lay real foundations for robotics"）
  - NVIDIA Research（Cosmos 3 technical report，2026-6-1）
  - Anthropic 官方（《Expanding Project Glasswing》，《Project Glasswing: An Initial Update》）
  - CNBC（June 2，《Anthropic expands Mythos to 150 additional organizations in more than 15 countries》）
  - TechCrunch（June 2，《Anthropic scales Claude Mythos to critical infrastructure in 15 countries》）
  - Cybersecurity Dive（《Anthropic shares Mythos with 150 more organizations》）
  - BuildFastWithAI（June 15，《AI News Today June 15 2026: 16 Biggest Stories》）
  - Hacker News Trends June 2026（mean.ceo 分析）
  - arXiv 2506.22355（《Embodied AI Agents: Modeling the World》，June 2026）
  - ChatGPT 1 billion MAU（DemandSage + IndexBox + US News Money，June 2026；May 2026 达成，超7天，排除）
  - OpenAI Sora 关闭（April 26 web/app 停止，超30天，排除）
  - Figure AI BotQ 1 robot/hour（April/May 1 宣布，超30天，排除）
  - Microsoft Phi-4-Reasoning-Vision-15B（March 4 发布，超30天，排除）
  - Fable 5 系统提示词泄露 / Pliny the Liberator（June 10，6天前；角度与 June 14 candidates 政府关闭令（含 jailbreak 起因）高度联动——今日已有 Anthropic Glasswing 覆盖深层AI思考柱和 NVIDIA Cosmos 3 覆盖，timeliness 相近情况下让位于 Glasswing 的独立叙事；可作为备选）
  - Karpathy "magnitude 9 earthquake" tweet（December 2025，超30天，排除）
  - G7 AI 峰会具体成果（June 15 Day 1 尚无 AI 承诺产出，G7 主要 AI 结论预计 June 16-17，明日再扫）
  - GPT-5.6（无已确认发布日期锚点，排除）
  - Anthropic Fable 5 / Mythos 5 恢复访问（截至今日仍未恢复，无新事件锚点）
  - Swyx 2026 thesis（"coding agents breaking containment"；无精确 June 14-16 事件锚点，排除）
  - Boston Dynamics Atlas + Gemini Robotics（WWDC 周报道，June 8-9 已扫描窗口，排除重复）
  - EngineAI T800（已在 2026-06-15 candidates 覆盖，排除重复）
  - LiteLLM CVE-2026-42271（已在 2026-06-15 candidates 覆盖，排除重复）
  - Anthropic Agent SDK 计费拆分（已在 2026-06-15 candidates 选定为 draft 046，排除重复）
  - Anthropic Fable 5 政府关闭令（已在 2026-06-14 candidates 覆盖，排除重复）
  - OpenAI Ona 收购（已在 2026-06-14 candidates 覆盖，排除重复）
  - Ramp AI Index Anthropic 超 OpenAI（已在 2026-06-14 candidates 覆盖，排除重复）

- **Total signals found**: 约 45 个评估

- **Why these 3**:

  - **Candidate 1（OpenAI Partner Network，June 14）**：时效 1-2 天，OpenAI 官方 + TechTimes + Dataconomy + FourWeekMBA 多方确认；AI产品战略柱：过去3天该柱未被选中（最近一次在 June 13 G7 AI 主权角度）；今日角度独特：OpenAI 在自己的新闻稿里说"模型能力不再是主要障碍"，且 $150M + 300K 认证顾问的渠道投入 + FDE 试点 = OpenAI 从模型公司向渠道公司转型的首个正式动作；Accenture/McKinsey/BCG/Bain/PwC 同日入伙是可验证的硬事实；中文 AI 圈普遍把此事报为"又一个合作伙伴计划"，未讨论"模型战争结束、渠道战争开始"的产品战略含义；HIGH 优先级。

  - **Candidate 2（NVIDIA Cosmos 3，June 1）**：时效15天（在30天窗口内），NVIDIA 官方 + HPCwire + Hugging Face + Interesting Engineering 多方确认；深层AI思考柱：过去3天该柱在 June 14 Fable 5 政府关闭（监管政治角度）中被覆盖——今日角度根本不同，这是 Physical AI 的架构突破（单一 MoT 双塔统一推理与生成，训练周期月→天），不是监管政治；Zico 在做 3DGS/Physical AI 产品，Cosmos 3 的 Reasoner-Generator 双塔与 3DGS 空间表示的技术交叉点是 Zico 独有的视角，中文 AI 圈对 Cosmos 3 的报道停留在"新发布的 NVIDIA 模型"层面，未讨论双塔架构对 sim-to-real 误差的根本解法，也未讨论与 3DGS 的连接；HIGH 优先级。

  - **Candidate 3（Anthropic Project Glasswing 扩展，June 2）**：时效14天（在30天窗口内），Anthropic 官方 + CNBC + TechCrunch + Cybersecurity Dive 四方确认；Agent经济柱：过去3天该柱在 June 13 GitLab Agentic Era（软件组织重构）和 June 12 NEURA Robotics（物理 Agent）中被覆盖——今日角度不重叠：这是 AI Agent 作为关键基础设施安全层（autonomous vulnerability hunter at infrastructure scale）的具体案例；10,000 个高危漏洞这个数字是可验证的量化输出，Glasswing + 10天后 Mythos 被出口管制的时间反差在中文 AI 圈几乎没有讨论；MEDIUM 优先级（时效14天略旧；但 Agent 经济柱的独立叙事成立，信息密度高）。
