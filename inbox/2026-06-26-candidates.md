---
date: 2026-06-26
status: pending_selection
---

# Today's Candidates

## Candidate 1: OpenAI 与 Broadcom 发布"Jalapeño"——OpenAI 首颗自研推理芯片，用自己的 AI 设计，9个月完成 tape-out，直指 NVIDIA 的推理定价权（June 24）

- **Event**: 2026年6月24日，OpenAI 与 Broadcom 联合发布 **Jalapeño**，OpenAI 官方称之为"Intelligence Processor"——这是 OpenAI 有史以来第一颗自研 AI 芯片，为 LLM **推理（inference）**专项设计。关键数据：从设计启动到 tape-out 只用了 **9个月**（行业 ASIC 开发通常需要 2-4 年）；早期测试显示比当前最优解具备显著更高的 **performance-per-watt**；芯片设计本身由 OpenAI 自家 AI 模型协助完成；定位是"massive reticle-sized ASIC"（全掩模尺寸）；计划 **2026年底开始部署**，目标是与 Microsoft 和其他合作伙伴建立**吉瓦级（gigawatt-scale）数据中心**。明确边界：Jalapeño 只用于 inference，**pre-training 仍依赖 NVIDIA**。NVIDIA 目前仍是 OpenAI 最大硬件供应商和重要投资方，但此次发布意味着 OpenAI 在推理层不再是 NVIDIA 的专属客户。**多方来源确认**：OpenAI 官方博客（6月24日）、TechCrunch（6月24日）、CNBC（6月24日）、Tom's Hardware（6月24日）、VentureBeat（6月24日）、Yahoo Finance（6月24日）、CNN Business（6月24日）、HotHardware（6月24日）。
- **Source**: https://openai.com/index/openai-broadcom-jalapeno-inference-chip/ | https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/ | https://www.cnbc.com/2026/06/24/openai-and-broadcom-reveal-jalapeno-first-ai-chip-in-partnership.html | https://www.tomshardware.com/tech-industry/artificial-intelligence/broadcom-and-openai-unveil-custom-built-jalapeno-inference-processor-openais-first-chip-is-a-massive-reticle-sized-asic-built-in-an-ultra-fast-nine-month-development-cycle | https://venturebeat.com/infrastructure/openai-unveils-first-custom-ai-inference-chip-jalapeno-with-broadcom-and-its-development-was-sped-up-with-openais-own-models/
- **Timeliness**: 2天前（2026年6月24日，OpenAI 官方发布）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 这件事有两层值得单独分析，不要合在一起看。

  第一层：**9个月做完一颗 ASIC**，这本身已经是一个结构性信号。业内 ASIC 开发通常需要 2-4 年。OpenAI 用自己的 AI 模型辅助完成了芯片设计——这是 AI 第一次以 AI-assisted engineering 的方式加速了硬件开发周期。如果这个方法论可以复制，AI 加速的不只是软件，而是整个芯片迭代速度。

  第二层，也是更值得产品策略层分析的：**OpenAI 把 NVIDIA 的推理业务切走了一半**。OpenAI 的 ChatGPT 每天服务数十亿次查询——这些查询绝大多数都是 inference（推理），不是 training（训练）。NVIDIA 的 GPU 对 training 做了深度优化，但 inference 的工作负载模式完全不同：更短的 batch size、更高的 I/O 频率、特定的 attention pattern。Jalapeño 是 OpenAI 根据自己的 ChatGPT 工作负载从零设计的——它比通用 GPU 更懂自己的模型。

  这和苹果 2020年做 Apple Silicon 是同一个战略逻辑：当你既做软件又做芯片，优化空间是纯硬件公司看不见的。苹果不需要英特尔把 Mac 性能提升 50%，苹果把 macOS 和芯片的 ISA 协同设计，一年内性能提升三倍。OpenAI 的 Jalapeño 在说：我的 inference 比你 NVIDIA 更懂我的 GPT。

  更大的趋势：**前沿 AI 实验室正在变成半导体公司**。不是建自己的晶圆厂，而是定义定制 ASIC：Google 有 TPU、Amazon 有 Trainium、Microsoft 在做 Maia、苹果有 Neural Engine、现在 OpenAI 有 Jalapeño。这意味着 NVIDIA 的护城河从"唯一选择"变成了"训练阶段的优选"。推理市场，这个比训练大得多的长期市场，正在被瓜分。做 AI 产品的人要问一个问题：**我的 AI 推理成本，正处于被哪家公司的芯片战略所决定的阶段？**

- **Resonance hook**: 6月24日，OpenAI 和 Broadcom 发布 Jalapeño，OpenAI 有史以来第一颗自研芯片。只用了9个月，芯片设计过程中有 OpenAI 自己的 AI 在帮忙。定位不是和 NVIDIA 的 H200 竞争——而是专门替换掉 ChatGPT 推理环节里的 NVIDIA。OpenAI 在用苹果 Apple Silicon 的逻辑做芯片：软件和芯片协同设计，比任何通用方案都更懂自己的模型。训练还是 NVIDIA，推理开始不一定是了。
- **Recommended priority**: high

---

## Candidate 2: Anthropic 致信白宫，指控 Alibaba 旗下 Qwen 团队用 25,000 个假账号、2,880 万次 Claude 对话蒸馏其模型能力——史上最大已记录蒸馏攻击（June 24）

- **Event**: 2026年6月24日，Bloomberg 和 CNBC 同日披露：**Anthropic** 于 6月10日向美国参议院银行委员会（寄给参议员 **Tim Scott 和 Elizabeth Warren**）以及**白宫**发出一封公开信，指控 **Alibaba（阿里巴巴）旗下 Qwen AI 实验室**的关联运营者在 **2026年4月22日至6月5日**期间，动用约 **25,000 个欺诈账号**，对 Claude 模型发起 **28,800,000次（2,880万次）**对话请求，系统性提取 Anthropic 模型的能力输出，并将这些输出用于训练 Qwen 模型——Anthropic 将此定性为"**对 Anthropic 迄今记录的最大规模蒸馏攻击**"。Anthropic 说明：此次攻击目标是 Anthropic 最前沿能力，包括**软件工程、多步推理和网络安全任务**（即 Mythos Preview 模型的核心能力）；攻击方法称为"**对抗性蒸馏（adversarial distillation）**"——通过系统性查询提取竞争对手模型的推理模式和输出结构，用以训练自己的模型，本质上是让数千亿美元的美国 AI 投资成为中国竞争者的训练语料。对比规模：2026年2月那次（涉及 DeepSeek、MiniMax、Moonshot AI）是 16,000,000 次交换、约 24,000 个假账号——本次 Alibaba 超出前者约 80%。Anthropic 称 Alibaba "无视了特朗普政府的警告"。立法回应：参议员 **Bill Hagerty 和 Andy Kim** 计划向必过国防立法提出修正案，将被发现非法访问美国 AI 模型输出的中国企业列入黑名单或制裁。来源：Bloomberg（6月24日首发）、CNBC（6月24日，附视频报道）、Tom's Hardware（6月24日）、The Next Web（6月24日）、The Street（6月24日）、AI Weekly（6月24日）、Tweaktown（6月24日）、InfoWorld（6月24日）。
- **Source**: https://www.bloomberg.com/news/articles/2026-06-24/anthropic-accuses-alibaba-of-illicitly-accessing-its-ai-models | https://www.cnbc.com/2026/06/24/anthropic-alibaba-distillation-campaign.html | https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropic-claims-that-chinas-alibaba-illicitly-distilled-its-models-from-april-to-june-2026-says-effort-involved-25-000-fake-accounts-and-28-8-million-exchanges-on-claude | https://thenextweb.com/news/anthropic-accuses-alibaba-distillation-claude-qwen | https://www.thestreet.com/technology/alibaba-accused-harvesting-anthropic-technology-ai-us-china
- **Timeliness**: 2天前（2026年6月24日，Bloomberg + CNBC 同日首发）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 这件事的核心问题不是"偷没偷"，而是：**前沿 AI 模型的"护城河"到底是什么形态的资产？**

  Alibaba 没有盗取 Anthropic 的源代码、没有获取模型权重、没有拿到训练数据。他们做的事情是：通过25,000个账号、用6周时间让 Claude 回答了2,880万个问题，然后用这些问答对来训练 Qwen。这在技术上是"用 API 查询模型"——和任何 ChatGPT Plus 用户的操作没有本质区别，只是规模不同。

  这暴露了一个法律和战略上的双重空白：**传统 IP 保护（专利、商业秘密、版权）对模型行为签名（behavioral signature）几乎没有覆盖**。一个模型在特定推理任务上展示的行为模式——它怎么分解问题、怎么结构化回答、怎么处理代码调试——可以通过大量系统性查询被提取出来，转化成另一个模型的训练数据。没有哪条现有法律清晰地说这是非法的。

  更值得关注的是规模的演变曲线：2月（DeepSeek/MiniMax/Moonshot）16M次，4月至6月（Alibaba）28.8M次。在 Anthropic 已经公开记录了2月攻击、并向政府披露的情况下，Alibaba 仍然进行了更大规模的攻击。这说明被发现的代价，对攻击方来说小于收益。

  立法层（Hagerty + Kim 国防修正案）的介入是关键信号：这件事已经不在商业法庭解决，而是直接跨入了国家安全立法轨道。"哪些行为构成对美国 AI 模型的违法访问"将会得到一个法律定义——而这个定义会影响全球每一家调用竞争对手 API 做对比测试的 AI 公司的边界。

  对做 AI 产品的人，这件事给了一个直接的产品策略信号：**当 API 访问本身成为战略攻击向量，速率限制、行为检测、查询指纹分析将成为前沿模型的核心基础设施，不再是可选的反滥用工具**。Anthropic 能记录下 2,880 万次查询来自 25,000 个假账号，说明它有这个检测能力——但检测出来之后怎么办，目前没有清晰的法律依据。这个真空正在被国防立法填补。

- **Resonance hook**: 6月24日，Bloomberg 独家：Anthropic 致信白宫和参议院，指控 Alibaba 旗下 Qwen 团队用 25,000 个假账号在 6 周内向 Claude 发起 2,880 万次查询，系统性提取模型能力来训练 Qwen。Anthropic 说这是迄今最大规模的蒸馏攻击，超过了2月那次 DeepSeek/MiniMax/Moonshot 的联合攻击。Alibaba 没有盗取代码或权重——只是大规模用 API，把 Claude 的行为输出喂给了自己的模型。传统 IP 法对这件事几乎没有覆盖。参议员正在写国防立法。
- **Recommended priority**: high

---

## Candidate 3: LeCun 告诉 CNBC：xAI "有点失败"，OpenAI 和 Anthropic 面临"大泡沫爆炸"风险——投资人正在补贴用户用 AI，这无法持续（June 18）

- **Event**: 2026年6月18日，**Yann LeCun**（深度学习三巨头之一、AMI Labs 创始人、前 Meta 首席 AI 科学家）在 CNBC 专访中发表两项重要判断：① 关于 xAI："xAI is kind of a failure（xAI 有点是个失败），说实话，因为创始团队已经离开了"——LeCun 指出 Elon Musk 现在"处于非常、非常困难的境地，很难招到顶级 AI 人才"；xAI 背景数据：SpaceX AI 部门（包含 xAI）2026年 Q1 运营亏损 **$25亿**，在同期 Grok 4 能力评估中落后于 GPT-5.5 和 Claude Fable 5；② 关于 AI 泡沫："如果 AI 实验室不削减成本、提高价格，正在面临'**大泡沫爆炸**'风险"。具体表述："价格在涨，但运行成本下降速度不够快——所有这些公司都在亏钱，大多数用户的 AI 使用实际上是由投资人买单的。这无法持续太久"；他们"要么提价，要么削减成本，否则就会有大泡沫爆炸"。LeCun 本人目前在 AMI Labs（2026年3月完成 **$10亿融资**，估值 **$35亿（pre-money）**），研究方向是世界模型（world models）——而非当前主流的 LLM scaling 路径。CNBC 报道（6月18日）、The Next Web（6月18日）、AI Weekly（6月18日）、Startup Fortune（6月18日）、Memeburn（6月18日）多方确认。
- **Source**: https://www.cnbc.com/2026/06/18/yann-lecun-elon-musk-xai-failure-ai-labs-bubble-risk.html | https://thenextweb.com/news/yann-lecun-xai-failure-ai-bubble-explosion | https://aiweekly.co/node/3149 | https://startupfortune.com/yann-lecun-calls-xai-a-failure-as-elon-musks-lab-pivots-from-frontier-ai-to-renting-out-servers/ | https://memeburn.com/godfather-of-ai-calls-xai-a-failure-warns-of-ai-bubble/
- **Timeliness**: 8天前（2026年6月18日，CNBC 专访）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: LeCun 说的这两件事，表面上是独立的，底层是同一个判断：**当前主流 AI 实验室的商业模式，正在依赖投资人补贴来掩盖真实的经济结构问题**。

  先看 xAI。LeCun 的诊断是"创始团队离开了，Elon 招不到顶级 AI 人才"。这个表述是一个组织信号，不只是人才信号。当一家公司在算力（Colossus 2，NVIDIA GB300）、资金（SpaceX 现金流）上都有显著优势时，仍然面临顶级研究者不愿加入的困境——说明 AI 顶级人才的择业逻辑已经不是资源导向，而是"这里能不能做到最重要的工作"。这是和 Google DeepMind（Shazeer + Jumper 一周内离职）完全不同的问题，但根因相似：**拥有算力不等于拥有研究重力**。

  再看泡沫论。LeCun 的数学很直接：OpenAI 最近披露的 2025 年亏损是 $50亿。如果它靠 $20/月的 ChatGPT Plus 和 $200/月的 Pro 订阅维持 8 亿月活，而重度用户的实际推理成本远高于订阅价格，那么实质上是在用 Softbank、Microsoft、Apple 的投资补贴这些用户的 AI 使用——就像 Uber 早期的每公里实际成本是订单价格的2倍。Uber 存活靠的是"最终成本会下来"的假设；AI 实验室的赌注是"scaling 会持续让推理变便宜"。但 Jalapeño 和 Trainium 的发布恰恰说明这件事并非自然发生——需要定制芯片才能解决推理成本问题，而 LeCun 的判断是这还不够快。

  LeCun 自己的押注（AMI Labs，世界模型）是一个反 scaling 的赌注：他认为当前 transformer + scaling 路径会触到能力天花板，世界模型需要结构化的物理先验，不是更多的语言数据。在他自己的替代方案完成之前，他指出的问题在哪里都不会消失。

  这个角度在中文 AI 圈完全缺席。中文媒体会报道"LeCun批评Elon的AI公司失败了"，不会分析"投资补贴的商业模式在可持续性上的边界在哪里"，也不会把 LeCun 的批评和他的 AMI Labs 押注放在同一个分析框架里看。

- **Resonance hook**: 6月18日，CNBC 专访 Yann LeCun：xAI "有点是个失败"，因为创始团队走了，Elon 现在招不到顶尖 AI 人才。AI 实验室正在面临"大泡沫爆炸"风险——投资人正在补贴大多数用户的 AI 使用，成本下降速度跟不上。LeCun 的替代方案是 AMI Labs，做世界模型，不做 LLM scaling。一个 AI 行业里资历最深的批评者，在说当前 AI 实验室的经济模型有结构性问题，同时在下一个完全不同方向的赌注。
- **Recommended priority**: medium-high

---

## Scan summary

**Sources scanned**:
- OpenAI 官方博客（openai.com/index/openai-broadcom-jalapeno-inference-chip/，6月24日，Jalapeño 芯片官方发布）
- TechCrunch（6月24日，《OpenAI unveils its first custom chip, built by Broadcom》）
- CNBC（6月24日，《OpenAI and Broadcom reveal Jalapeño, first AI chip in partnership》）
- Tom's Hardware（6月24日，《Broadcom and OpenAI unveil custom-built Jalapeño inference processor》，ASIC 技术细节）
- VentureBeat（6月24日，《OpenAI unveils first custom AI inference chip, Jalapeño, with Broadcom》，AI辅助设计细节）
- Yahoo Finance / Startup Fortune / HotHardware / CNN Business（6月24日，Jalapeño 多方确认）
- Bloomberg（6月24日，《Anthropic accuses Alibaba of 'illicitly' accessing AI models》，蒸馏攻击首发）
- CNBC（6月24日，《Anthropic accuses Alibaba of campaign to 'brazenly' and 'illicitly' extract AI capabilities》）
- Tom's Hardware（6月24日，《Anthropic claims Alibaba used 25,000 fake accounts and 28.8 million exchanges》，数字确认）
- The Next Web（6月24日，《Anthropic accuses Alibaba of running largest distillation campaign against Claude》）
- The Street（6月24日，《The secret letter triggering a U.S.-China AI showdown》，立法背景）
- AI Weekly（6月24日，蒸馏攻击确认）
- Tweaktown / InfoWorld / 247WallSt / ZeroHedge / CryptoBriefing（6月24-25日，蒸馏攻击多方跟进）
- X/Interesting Engineering（6月24日，参议院信件 6月10日日期确认）
- CNBC（6月18日，《Godfather of AI blasts Musk's xAI as 'failure,' says labs are risking a 'big bubble explosion'》，LeCun 专访原文）
- The Next Web（6月18日，《Yann LeCun calls xAI a 'failure', warns of AI bubble》）
- AI Weekly（6月18日，《Yann LeCun Calls xAI 'a Kind of Failure'》）
- Startup Fortune（6月18日，xAI 关键细节：创始团队离职、Q1 $25亿亏损背景）
- Memeburn / TrendingTopics / CNBC Africa（6月18日，多方确认）
- GPT-5.6（无 OpenAI 官方确认；Polymarket 6月22-28发布概率已从83%跌至18%，现指向7月底；排除）
- Claude Tag on Slack（Anthropic 发布 Claude 企业团队 Slack beta 集成，产品功能类，无独立战略叙事锚点，排除）
- Karpathy Loop / AutoResearch（2026年3月7日发布，超30天窗口，排除）
- Anthropic Mythos NSA 红队测试（已在6月24日候选全面覆盖，排除）
- DeepMind 人才双离职（Shazeer + Jumper，已在6月24日候选全面覆盖，排除）
- Gemini 3.5 Pro 延期（已在6月25日候选全面覆盖，排除）
- Reflection AI SpaceX $63亿（已在6月25日候选全面覆盖，排除）
- GitHub Trending AI（awesome-ai-agents-2026 汇总型清单无精确锚点；Gemini-cli 6月发布，无独立叙事强度，排除）
- arXiv June 2026（World-Model-Augmented Web Agents、DynaWeb、Agentic Reasoning for LLMs——均为学术论文合集无独立高传播单篇事件锚点，排除）
- HN top AI posts June 25-26（Anthropic Alibaba 蒸馏攻击为主导话题，已纳入 Candidate 2；Jalapeño chip 讨论活跃，已纳入 Candidate 1；其余为技术讨论无独立事件锚点，排除）
- Agentjacking 安全攻击披露（June 2026，新 AI 安全攻击类别，无精确 6月24-26 独立强锚点，排除）
- Altman AI costs 表态（"AI成本是大问题"，无精确6月24-26锚点，排除）
- Dario India Summit 评论（6月18日，无独立叙事强度，排除）

**Total signals found**: 约 31 个信号评估

**Why these 3**:

- **Candidate 1（OpenAI Jalapeño，6月24日）**：时效最强（2天），OpenAI 官方 + TechCrunch + CNBC + Tom's Hardware + VentureBeat 五方来源确认；**AI产品战略柱**：过去3天 SELECTED 分别覆盖了 AI协作实践（6月25日）、AI产品战略（6月24日，Nadella learning loop）、Agent经济（6月23日）——今天角度完全不重叠："OpenAI 首颗自研推理芯片在9个月内完成 tape-out，用 AI 辅助设计，直接切入 NVIDIA 的推理业务"是全新的硬件层战略叙事；Jalapeño 的「AI辅助芯片设计」细节 + 「推理/训练分层」这两个具体机制在中文媒体完全没有深度分析（中文媒体会报道"OpenAI做芯片了"，不会分析"为什么是推理而不是训练"）；与 Zico 的 AI 产品战略认知（"AI 基础设施的垂直整合"、"护城河从模型能力层下移至硬件层"）直接对应；HIGH 优先级。

- **Candidate 2（Alibaba 蒸馏攻击，6月24日）**：时效最强（2天），Bloomberg + CNBC + Tom's Hardware + TheNextWeb + The Street 五方以上来源确认；**组织形式变革柱**：过去3天 SELECTED 均未覆盖此柱（6月25日 AI协作实践，6月24日 AI产品战略，6月23日 Agent经济）——最大空白柱；"对抗性蒸馏"（adversarial distillation）这个行为不是传统 IP 盗窃，是通过 API 大规模提取行为签名，目前没有法律定义，正在被国防立法填补——这个机制分析在中文媒体完全缺席（中文媒体会停在"中美 AI 对抗"的地缘政治层面，不会分析什么是可保护的 AI 资产以及当前的法律真空）；Anthropic 能记录 2,880 万次查询的系统性行为检测能力本身是一个重要信号；Senators Hagerty + Kim 国防修正案是可追踪的立法进展；HIGH 优先级。

- **Candidate 3（LeCun xAI + AI 泡沫，6月18日）**：时效8天（略超7天理想窗口，30天内可接受），LeCun 是 Tier 1 来源（深度学习三巨头之一，CNBC 专访），CNBC + TheNextWeb + AI Weekly + Startup Fortune + Memeburn 五方确认；**深层AI思考柱**：过去3天均未被 SELECTED 用于此柱（6月25日 AI协作实践，6月24日 AI产品战略，6月23日 Agent经济）；LeCun 对 xAI 和 AI 实验室泡沫的批评提供了一个与 Karpathy（加入 Anthropic）完全相反的视角——一个深度学习创始人认为当前 AI 实验室在烧投资人的钱补贴用户，这和 Anthropic $965亿估值 + OpenAI IPO 筹备同时进行的背景形成强烈张力；"投资补贴的商业模式边界"在中文 AI 圈几乎没有系统分析；与 AMI Labs 世界模型押注的关联是完整的叙事链；MEDIUM-HIGH 优先级（时效略旧为唯一弱点，内容质量和来源权威性均高）。
