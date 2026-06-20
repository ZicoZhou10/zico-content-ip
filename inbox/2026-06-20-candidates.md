---
date: 2026-06-20
status: pending_selection
---

# Today's Candidates

## Candidate 1: General Intuition 以游戏视频训练空间智能 Agent，$3亿融资 $20亿估值——Jeff Bezos + Eric Schmidt 押注「游戏数据是物理 AI 最被低估的资产」（June 18）

- **Event**: 2026年6月18日，**General Intuition**（纽约，空间智能 + 世界模型初创）正式宣布以 **$20亿估值融资约 $3亿**，由 **Khosla Ventures 和 General Catalyst** 领投，**Jeff Bezos 和 Eric Schmidt** 跟投，距离其 2025年10月以 **$1.34亿种子轮**从 **Medal** 游戏视频平台剥离成立仅 8 个月。核心数据：Medal 平台有 **1,000万月活用户**，每年生成 **20亿个游戏视频片段**（first-person gameplay clips），涵盖 Fortnite、Valorant 等主流游戏。General Intuition 的核心论点：这 20 亿个第一人称交互视频是训练具身 AI 和世界模型最理想的数据集——**因为它是在物理约束下（重力、碰撞、惯性）、由真实人类操控、带有意图标注的空间时序数据**。产品定位：世界模型作为训练场，Agent 作为产品——收入绑定 AI 能做什么，而不是绑定平台能渲染什么。来源：**TechCrunch**（June 18，《General Intuition in talks to raise $300M at around $2B valuation》）、**SiliconANGLE**（June 18，《Game-clip AI startup General Intuition in talks to raise $300M at $2B valuation》）、**TheNextWeb**（《General Intuition raising $300M for AI trained on gaming data》）、**The AI Insider**（June 19，《General Intuition in Talks to Raise $300M at $2B Valuation to Advance Spatial AI Agent Training》）、**Startup Fortune**（《General Intuition is raising $300 million on the bet that gaming data is AI's most underrated asset》）。
- **Source**: https://techcrunch.com/2026/06/18/general-intuition-in-talks-to-raise-300m-at-around-2b-valuation/ | https://siliconangle.com/2026/06/18/game-clip-ai-startup-general-intuition-talks-raise-300m-2b-valuation/ | https://thenextweb.com/news/general-intuition-300m-world-models-gaming-data | https://theaiinsider.tech/2026/06/19/general-intuition-in-talks-to-raise-300m-at-2b-valuation-to-advance-spatial-ai-agent-training/ | https://startupfortune.com/general-intuition-is-raising-300-million-on-the-bet-that-gaming-data-is-ais-most-underrated-asset/
- **Timeliness**: 2天前（2026年6月18日 TechCrunch + SiliconANGLE + TheNextWeb 同日多方报道；6月19日 The AI Insider 跟进）
- **Topic pillar**: Agent经济（+ 空间智能前沿）
- **Zico's angle**: General Intuition 回答的不是"用什么架构训练物理 AI"，是"用什么数据训练物理 AI"。这两个问题以前被混在一起讨论，现在它们开始分叉。

  当前物理 AI / 具身智能的训练数据来源有三条路：**合成物理仿真**（NVIDIA Cosmos、Genesis、Isaac Sim——对物理定律建模，生成任意数量场景）、**真实世界机器人采集**（Boston Dynamics Atlas、Figure 01——真实但贵、慢、风险高）、**人类已有的视频数据**（YouTube、互联网视频——便宜但没有交互性、没有意图标注）。General Intuition 的论点：这三条路都有缺陷。合成仿真有 sim-to-real gap；真实机器人采集无法规模化；互联网视频里没有人"因为重力"做出决策的意图上下文。

  游戏视频解决了什么？玩家在每一帧都在做决策——"我感知到对手在左边，我预判他的移动，我做出这个操作"。这是在物理约束下（游戏引擎仿真真实物理）由人类生成的意图 + 动作对（intent-action pairs）。20 亿个视频，10 万小时以上的精细操控数据，每一秒都是"人类如何在空间中感知 - 预测 - 行动"的训练信号。

  这对 Zico 的 3DGS / 空间智能背景直接相关：3D 重建（NeRF、3DGS）解决的是"如何理解空间"，具身 AI 解决的是"如何在空间中行动"。General Intuition 的押注是：从游戏数据里学会"在空间中行动的先验知识"，比从合成物理仿真里学更快、更真实。如果这个论点成立，游戏平台（Medal、Twitch、YouTube Gaming）积累的人类游戏数据将成为物理 AI 竞争的关键资源——比芯片更难复制。

  $20亿估值、8 个月种子到 A 轮的节奏、Jeff Bezos + Eric Schmidt 同时押注——这三个信号合在一起，说明这个论点在顶级 VC 圈正在被认真对待，不只是一个早期假设。

- **Resonance hook**: 6月18日，一家 8 个月的 AI 初创公司 General Intuition 融资 $3亿，估值 $20亿。它训练 AI 用的数据：每年 20 亿个游戏视频，来自 Medal 平台 1,000 万月活玩家。论点：玩家在游戏里的每一帧决策——感知空间 + 预判 + 操控——是训练物理 AI 理解空间的最好数据集。Jeff Bezos 和 Eric Schmidt 都押注了。合成仿真有 sim-to-real gap，机器人真实采集无法规模化，YouTube 视频没有交互意图。游戏数据可能是中间那条路。
- **Recommended priority**: high

---

## Candidate 2: Noam Shazeer 离开 Google 加入 OpenAI——Transformer 发明者的职业轨迹跟踪着前沿模型研究在哪里（June 18）

- **Event**: 2026年6月18日，**Noam Shazeer** 在 X 上宣布离开 **Google DeepMind**，正式加入 **OpenAI**。Shazeer 的职业路径：**2000年加入 Google**，在 Google Brain 共事超过 **20年**，2017年与 Vaswani 等人合著 **《Attention Is All You Need》**（Transformer 架构论文，目前引用量超过 12 万次），2021年**离开 Google** 联合创办 **Character.AI**（消费级 AI 对话产品），2024年 **Google 以 $27亿** 许可费协议将他和团队带回，负责 **Gemini** 系列模型并担任 VP of Engineering + 联合负责人，2026年6月18日**再次离开 Google**，加入 OpenAI。同日，OpenAI 还宣布招募 **Dean Ball**（前 Trump 白宫 AI 政策官员）。背景：OpenAI 已秘密提交 IPO S-1，Goldman Sachs + Morgan Stanley 担任承销商，预计估值超过 $1万亿。来源：**TechTimes**（June 18，《Transformer Architect Behind Gemini Jumps to OpenAI After Google Spent $2.7B》）、**TechCrunch**（June 18，《OpenAI is bringing on some big guns in the lead-up to its IPO》）、**IBTimes UK**（《Who Is Noam Shazeer? The AI Genius Whose Defection From Google to OpenAI Just Reset the Industry》）、**Startup Fortune**（《Noam Shazeer, the man who invented the transformer, is now working for OpenAI》）、**CryptoBriefing**（《Noam Shazeer joins OpenAI after leaving Google》）、**eciks.org**（《Transformer co-inventor and Google's Gemini leader Noam Shazeer is moving to OpenAI》）。
- **Source**: https://www.techtimes.com/articles/318613/20260618/transformer-architect-behind-gemini-jumps-openai-after-google-spent-27b.htm | https://techcrunch.com/2026/06/18/openai-is-bringing-on-some-big-guns-in-the-lead-up-to-its-ipo/ | https://www.ibtimes.co.uk/ai-pioneer-noam-shazeer-leaves-google-openai-1803432 | https://startupfortune.com/noam-shazeer-the-man-who-invented-the-transformer-is-now-working-for-openai/ | https://cryptobriefing.com/noam-shazeer-joins-openai-leaves-google/
- **Timeliness**: 2天前（2026年6月18日 TechTimes + TechCrunch + IBTimes + Startup Fortune 同日多方报道）
- **Topic pillar**: AI产品战略
- **Zico's angle**: Shazeer 的职业移动不是一个人的选择，是前沿模型研究重心在哪里的实时信号。

  2021 年他离开 Google，当时 Google 在大模型研究上资源最多、论文最多，但 GPT 系列在商业化速度上已经领先。他看到了什么？可能是：在一家大公司里做模型研究，和在一家为此而存在的公司里做，产出的速度和质量不同。Character.AI 的结果是一个消费级对话产品，有用户，但不是前沿模型研究的最佳位置。

  2024 年他回到 Google，$27亿。那个时机是：Gemini 需要一个能与 GPT-4 竞争的架构领头人，Shazeer 是最合适的人。两年后他又离开了。

  Gemini 3.5 在某些评测上已经和 Claude 及 GPT-5.x 并列，Google 的模型能力不是问题。那他为什么走？最直白的解释是 IPO 股权，OpenAI 上市前的期权价值远大于 Google 的 RSU。但如果只是钱，2024 年 Google 用 $27亿把他买回来的价格就已经足够了。他再次离开，说明还有第二个因素：他在 OpenAI 看到的某种研究方向，在 Google 的框架里做不了，或者做得更慢。

  这是一个很具体的产品策略信号，不是只关于 Shazeer 个人：**当架构发明者从正在用他发明的架构赢得市场份额的公司，移向正在打 IPO 的竞争对手，这个移动本身就是一条信息**——关于他对下一个模型架构创新在哪里的判断，或者关于他对当前架构竞争已经进入收益递减阶段的判断。

  中文 AI 圈会把这件事报道为"Transformer 发明者加入 OpenAI"，停在这里。更值得讨论的是：在当前模型架构相对稳定（各家都在 Transformer 变体上迭代）的阶段，他的移动是在追逐 token，还是在追逐下一个架构的机会？

- **Resonance hook**: 6月18日，Noam Shazeer 宣布离开 Google 加入 OpenAI。他是 2017年《Attention Is All You Need》的共同作者之一——Transformer 架构的发明者，ChatGPT、Gemini、Claude 底层结构的设计者。2021年他离开 Google 创业，2024年 Google 花 $27亿把他买回来做 Gemini，两年后他再次离开。每次移动都是他对"前沿研究在哪"的判断。这次他选了 OpenAI，就在 OpenAI IPO 前夕。
- **Recommended priority**: high

---

## Candidate 3: FERC 强制 6 大电网给 AI 数据中心开绿色通道——美国联邦机构正式确认电力是 AI 扩展的新瓶颈（June 18）

- **Event**: 2026年6月18日，**美国联邦能源监管委员会（FERC）** 向六大区域电网运营商——**PJM Interconnection、MISO（Midcontinent ISO）、SPP（Southwest Power Pool）、CAISO（California ISO）、ISO-NE（ISO New England）、NYISO（New York ISO）**——同步发出定制化执法令（Section 206 orders），要求六家电网证明其 **AI 数据中心能够及时且有序地接入输电系统**，否则需修改联网规则。关键条款：AI 数据中心需**自行承担联网建设成本**；FERC 同步为电网科技创业公司开放"替代输电技术"（固态变压器、超导输电线等）参与空间。背景：此次执法令直接响应 2025年 **DOE 部长 Chris Wright** 的请求，目标是"大幅加速 AI 等大负荷用户的电网接入"。**德克萨斯州不在覆盖范围**内（ERCOT 在 FERC 管辖范围之外）。同期数据：**微软 2026年全年资本开支预计达 $1,900亿**，其中 $250亿增量来自内存和存储组件涨价（AI 基础设施需求驱动）；全球 AI 数据中心用电量正在以每年 40%+ 速度增长。来源：**TechCrunch**（June 18，《AI data centers just got a government-mandated fast lane to the grid》）、**TheNextWeb**（《FERC fast-tracks data centre grid connections》）、**The Energy Magazine**（June 19，《US to Fast-Track AI Data Centers as Power Bottleneck Becomes National Priority》）、**American Action Forum**（《FERC Data Center Orders Accelerate Grid Connection》）、**Yahoo Finance / TechCrunch**（《AI data centers just got a government-mandated fast lane to the grid》）。
- **Source**: https://techcrunch.com/2026/06/18/ai-data-centers-just-got-a-government-mandated-fast-lane-to-the-grid/ | https://thenextweb.com/news/ferc-data-centre-grid-fast-lane-ai | https://theenergymag.com/news/2026-06-19/united-states-fast-track-ai-data-center | https://www.americanactionforum.org/insight/ferc-data-center-orders-accelerate-grid-connection/
- **Timeliness**: 2天前（2026年6月18日 TechCrunch + TheNextWeb 发布；6月19日 The Energy Magazine 跟进）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: AI 扩展的瓶颈从芯片转移到了电力。FERC 的这道命令是美国联邦机构第一次明确承认这件事。

  过去两年关于 AI 竞争的讨论集中在算力：H100、B200、GB200、CoWoS 封装产能、TSMC 3nm 良率。这些讨论把芯片当成瓶颈。但在 2025-2026 年实际的大模型训练实践中，另一个约束已经悄悄浮出水面：数据中心**接入电网的排队时间**，在美国某些地区已经是 7-10 年。你有钱买芯片，有土地建数据中心，但没有电，机器没法运转。

  FERC 的六道执法令，是联邦层面首次把 AI 数据中心的用电接入定性为**全国优先事项**。这和出口管制是同一个政策框架的两面：一面是**限制谁能访问前沿 AI**（出口管制 Fable 5、H100 禁运），另一面是**确保美国自己的 AI 基础设施不受电网限制**。两件事加在一起，指向同一个目标：**确保美国在 AI 扩展的每一层物理基础设施（芯片 + 电力 + 联网带宽）上的控制权**。

  对做 AI 产品的人，这里有一个更直接的信号：如果电力是新的扩展约束，那么推理效率（tokens per watt，而不只是 tokens per second）将成为 AI 产品选型的核心指标之一。Anthropic 的 Fable 5 和 OpenAI 的 GPT-5.6 之争，不只是能力之争，也是功耗效率之争。**数据中心运营商会因为推理效率不同而偏好不同的模型**——而这个偏好对模型提供商的营收直接相关。

  中文 AI 媒体几乎不报道 FERC 层面的政策动态。但中国做 AI 基础设施的公司（字节、腾讯、百度的算力团队）面临同样的电力约束——只是在中国的政策框架下，而非 FERC。

- **Resonance hook**: 6月18日，美国联邦能源监管委员会向 6 大电网发出强制令：必须让 AI 数据中心快速接入电网。AI 训练集群的用电需求每年增长 40% 以上，但电网联网排队在美国某些地区已经等到 2033 年。微软今年光内存和存储就多花了 $250亿，因为 AI 基础设施需求。芯片不再是唯一瓶颈了，电力才是接下来 2-3 年 AI 竞赛的地基。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**:
  - TechCrunch（June 18，《General Intuition in talks to raise $300M》、《OpenAI is bringing on some big guns in the lead-up to its IPO》、《AI data centers just got a government-mandated fast lane to the grid》、《The 11 standout startups from YC's Demo Day, according to VCs》）
  - SiliconANGLE（June 18-19，《Game-clip AI startup General Intuition in talks to raise $300M》、《Databricks' new agentic coworker Genie One》）
  - TheNextWeb（June 18，《FERC fast-tracks data centre grid connections》、《General Intuition raising $300M for AI trained on gaming data》）
  - TechTimes（June 18，《Transformer Architect Behind Gemini Jumps to OpenAI After Google Spent $2.7B》、June 16《GPT-5.6: OpenAI Chief Scientist Calls It a Meaningful Leap》）
  - The AI Insider（June 19，《General Intuition in Talks to Raise $300M》、《OpenAI Hires Transformer Co-Author Noam Shazeer》）
  - IBTimes UK（《Who Is Noam Shazeer? The AI Genius Whose Defection From Google to OpenAI Just Reset the Industry》）
  - Startup Fortune（《General Intuition is raising $300 million on the bet that gaming data is AI's most underrated asset》、《Noam Shazeer, the man who invented the transformer, is now working for OpenAI》）
  - CryptoBriefing（《Noam Shazeer joins OpenAI after leaving Google》）
  - The Energy Magazine（June 19，《US to Fast-Track AI Data Centers as Power Bottleneck Becomes National Priority》）
  - American Action Forum（《FERC Data Center Orders Accelerate Grid Connection》）
  - Yahoo Finance（June 18，《AI data centers just got a government-mandated fast lane to the grid》）
  - Databricks 官方（《Genie One launch at Data + AI Summit 2026》，June 16/18）
  - SD Times（《Databricks releases agentic coworker Genie One》）
  - StorageNewsletter（June 18，Databricks Data + AI Summit 2026 recap）
  - BusinessStandard / DeccanHerald / BusinessToday（June 18-19，Dario Amodei India AI Summit incident）
  - BeInCrypto / Rappler（June 18，Noam Shazeer Google → OpenAI）
  - llm-stats.com（LLM News June 2026 全局扫描）
  - wavespeed.ai（June 2026 AI Launch Wave，全局信号扫描）
  - dentro.de/ai（June 2026 AI news roundup）
  - aiweekly.co（Google AI News June 2026）
  - avihacker.substack.com（DeepMind 1M token Gemini 动态）
  - OSS Insight + ByteByteGo（GitHub Trending AI repos June 2026）
  - arXiv cs.LG / cs.MA（June 2026 current list，世界模型和 Agent 推理论文综述）
  - Mezha.net（YC Demo Day Spring 2026 standout startups）
  - OpenAI 官方（GPT-5.6 状态：Polymarket 83% 概率 June 22-28，无官方发布，排除）

- **Total signals found**: 约 35 个信号评估

- **Why these 3**:

  - **Candidate 1（General Intuition $300M，June 18）**：时效 2天，TechCrunch + SiliconANGLE + TheNextWeb + The AI Insider 四方来源确认；Agent经济 + 空间智能前沿双柱命中：过去3天该方向在 June 18 Google Antigravity（数字 Agent 执行平台）和 June 15 EngineAI T800（物理 Agent 制造层）中覆盖过——今日角度根本不同：这是"物理 AI 的训练数据层"，争的是谁的数据能最有效地教 AI 理解空间；General Intuition 把"游戏平台积累的 20 亿人类第一人称操控数据"定位成物理 AI 竞争的资产（而非算法或算力），这个论点在中文 AI 圈几乎没有被分析过；Bezos + Schmidt 双押注是话题性担保；与 Zico 在 酷家乐 的 3DGS / 空间智能一线经验高度对应，可以带出真实的产品判断视角；HIGH 优先级。

  - **Candidate 2（Noam Shazeer 加入 OpenAI，June 18）**：时效 2天，TechTimes + TechCrunch + IBTimes UK + Startup Fortune + CryptoBriefing 五方来源确认；AI产品战略柱：过去3天该柱在 June 16 OpenAI Partner Network（$150M 渠道战略）和 June 16 OpenAI Deployment Simulation（产品信任方法论）中覆盖——今日角度根本不同：不是 OpenAI 的产品或策略，而是用 Shazeer 的职业轨迹追踪前沿模型研究重心转移；中文 AI 圈报道停在"Transformer 发明者加入 OpenAI"事实层面，没有分析 Google $27亿买回 + 2年后再次离开这个序列的含义；"架构师迁移是前沿研究位置的先行指标"这个分析框架是 Zico 可以首发的中文视角；HIGH 优先级。

  - **Candidate 3（FERC 电网执法令，June 18）**：时效 2天，TechCrunch + TheNextWeb + The Energy Magazine + American Action Forum 四方来源确认；深层AI思考柱：过去3天该柱在 June 17 G7 AI 午餐（地缘政治框架）和 June 18 Mastra 供应链攻击（安全层）中覆盖——今日角度完全不同：这是"AI 扩展的物理基础设施瓶颈"，从"芯片稀缺"到"电力稀缺"的叙事转型；中文 AI 媒体极少覆盖 FERC 级别的美国能源政策，但电力约束对中国 AI 公司同样成立（字节、腾讯、百度算力团队面临相同约束，只是政策框架不同）；联邦政府同时做"出口管制"和"电网开绿灯"这个结构性矛盾——统一解读为"控制 AI 物理基础设施的每一层"——是一个可以独立展开的深层判断；HIGH 优先级。
