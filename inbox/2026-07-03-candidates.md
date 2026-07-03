---
date: 2026-07-03
status: pending_selection
---

# Today's Candidates

## Candidate 1: NVIDIA 昨天开源 ASPIRE 机器人技能库——Jim Fan：训练范式从梯度下降变成技能蒸馏，双臂移交任务成功率从 20% 升至 92%（July 1）

- **Event**: 2026年7月1日（昨天），NVIDIA 正式开源 **ASPIRE**（Agentic Skills Discovery for Robotics），一个让机器人通过"失败→修复→蒸馏"循环积累可复用技能的训练系统。论文同日发布于 arXiv（编号 **2607.00272**，2606年6月30日预印）。核心机制：ASPIRE 基于 **Code as Policy** 范式——机器人执行任务时记录完整轨迹，遇到失败后分析原因、迭代修复程序，最终将调试出的解决方案蒸馏成"Skills"——一个可被未来任务直接调用的永久技能库。关键实验数据：① **双臂物体移交任务（dual-arm object handover）**：无技能库时成功率 **20%**，技能库积累后跳升至 **92%**；② 长时程任务泛化测试中，技能库越大，新任务成功率持续稳定提升，呈现明显的 scaling 特征。**NVIDIA 机器人研究负责人 Jim Fan**（GR00T 项目联合负责人）在 X 上明确点明范式变化：**"Training shifts from gradient descent to skill refinement, and the training output changes from model weights to a continuously expanding skill library."** Jim Fan 的配套表述："当机器人完成第 100 个任务时，它终于不再像完成第 1 个任务时那样一无所知。"这是对传统 RL 机器人训练的直接批评——每次调试的经验过去都被丢弃。ASPIRE 代码和技能库已在 GitHub 上公开。同期背景：NVIDIA 在 2026年6月下旬还宣布了与 Boston Dynamics 合作将 Gemini Robotics-ER 1.6 集成进 Spot 机器狗，但 ASPIRE 是迄今最明确的"训练范式级别"声明。来源：**NVIDIA Research GEAR Lab 官方页面**（research.nvidia.com/labs/gear/aspire/）、**arXiv 2607.00272**（2026年6月30日预印，7月1日正式开源）、**Hugging Face Papers**（2607.00272，7月1日高亮收录）、**TechTimes**（2026年7月1日，《Robot Skill Library ASPIRE Gives Robots Memory: Handover Climbs to 92%》）、**Jim Fan X 帖子**（2026年7月1日）、**NVIDIA Newsroom**（《NVIDIA Accelerates Robotics Research and Development With New Open Models and Simulation Libraries》）。
- **Source**: https://research.nvidia.com/labs/gear/aspire/ | https://arxiv.org/abs/2607.00272 | https://huggingface.co/papers/2607.00272 | https://www.techtimes.com/articles/319443/20260701/robot-skill-library-aspire-gives-robots-memory-handover-climbs-92.htm | https://nvidianews.nvidia.com/news/nvidia-accelerates-robotics-research-and-development-with-new-open-models-and-simulation-libraries
- **Timeliness**: 2 天前（2026年7月1日，NVIDIA 开源 + Jim Fan 发帖）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: Jim Fan 那句话值得展开："训练输出从模型权重变成了持续扩展的技能库。"

  这是一个范式级别的声明，但它背后的逻辑在中文圈几乎没有被认真对待。

  过去十年的 AI 训练，无论是 LLM 的 pretraining 还是 RL 的策略优化，训练的终点都是一套固定的参数——模型权重。权重一旦锁定，就不再从新经验里学习（除非再次 fine-tune）。这个设计在语言模型上没什么问题，因为"回答问题"本身是无状态的。但在物理世界里，机器人每次执行任务都会遇到新的环境配置、新的故障模式、新的解法——而所有这些经验在旧范式下都被丢弃了。ASPIRE 做的事情，是把"调试-修复"的过程本身变成训练数据，把经验蒸馏成技能，而不是蒸馏成梯度。

  这不仅仅是机器人训练效率的提升，这是在回答一个更深的问题：**AI 的"学习"是什么？** 是在海量数据上优化一次参数，还是通过持续经验积累改变行为能力？ASPIRE 选择了后者，并用 20%→92% 的数字证明这条路可行。

  对 Zico 来说，这和空间智能产品的实际挑战有直接交集。酷家乐的 3DGS 和 Physical AI 场景里，AI 系统需要处理的是真实室内环境的无限变化——家具配置、光照条件、用户偏好的排列组合是无穷的。一个靠固定权重工作的模型，每遇到新配置就相当于"第一次见"。而 ASPIRE 指向的方向——把处理过某类配置的经验蒸馏成可调用的 Skill——恰好是空间 AI 从"演示产品"走向"实用系统"需要解决的核心问题之一。

  中文媒体会报"NVIDIA 开源了机器人技能库，成功率从 20% 升到 92%"，不会分析：**这是 Physical AI 训练范式的一次明确表态——梯度下降作为 AI 学习的唯一形式，正在被挑战。**

- **Resonance hook**: 昨天，NVIDIA 开源了 ASPIRE——一个让机器人"记住怎么修自己犯的错"的训练系统。Jim Fan 的定义：训练输出不再是模型权重，是持续扩展的技能库。双臂移交任务成功率从 20% 跳到 92%。过去十年的 AI 学习，都是"训练一次、锁定参数、遇到新情况再训练"。ASPIRE 在问：为什么每次调试经验都要被丢掉？
- **Recommended priority**: high

---

## Candidate 2: California Governor Newsom 以 50% 折扣把 Claude 推给全州政府机构——Poppy AI 助手 7 月全面铺开，2800 名公务员已在使用（June 29）

- **Event**: 2026年6月29日，**加州州长 Gavin Newsom** 宣布加州与 **Anthropic** 达成"史上首个"州政府 AI 合作协议：全州所有州级机构、所有市和县政府，均可以 **50% 折扣**访问 Anthropic 的 Claude API。协议配套背景：加州自研政府 AI 助手 **Poppy**（命名自加州州花加州罂粟）已完成 pilot——在 67 个州级部门中超过 **2,800 名**公务员完成测试，覆盖预构建的政府场景工作流查询，7月将完成全州铺开；Claude 是构建 Poppy 所用的 10 个生成式 AI 模型之一，Anthropic-Newsom 协议将大幅降低 Poppy 后续扩展的调用成本。政治语境极为重要：① Newsom 此前已多次将加州定位为对抗 Trump 行政当局 AI 政策的"反向指针"——联邦政府以国家安全为由对 Anthropic 进行出口管制（Fable 5 被关停19天，6月12日-7月1日），加州政府同期选择将 Claude 设为全州官方 AI 工具，以政府采购的形式表态；② Anthropic 在 2026年上半年曾拒绝**五角大楼**的两项请求（解除安全护栏 + 全自主武器系统），由此被联邦定性为"供应链风险"；③ Newsom-Anthropic 协议实际上是州政府层面对 Anthropic 的政治信用背书，与联邦层面的管控叙事形成直接对冲。协议细节：TechCrunch（2026年6月29日）确认 50% 折扣、全州级覆盖；govtech.com 确认 Poppy 7月全面铺开时间表；福克斯商业频道（Fox Business）明确点名 Newsom 的政治定位意图。来源：**Governor of California 官方新闻稿**（2026年6月29日，《Governor Newsom announces a first-of-its-kind partnership》）、**TechCrunch**（2026年6月29日，《Anthropic and Gov. Newsom forge deal allowing California government to use Claude at half price》）、**GovTech**（2026年7月1日，《As Its Own AI Tool Expands, California Will Use Anthropic Too》）、**Fox Business**（2026年6月29日，《Newsom's office touts Anthropic 'partnership,' 50% discount on Claude AI for California agencies, localities》）、**GovTech Insider**（《State Strikes Anthropic Deal With Poppy Expansion Close Behind》）。
- **Source**: https://www.gov.ca.gov/2026/06/29/governor-newsom-announces-a-first-of-its-kind-partnership-providing-anthropic-tools-to-state-agencies-and-improving-services-for-californians/ | https://techcrunch.com/2026/06/29/anthropic-and-gov-newsom-forge-deal-allowing-california-government-to-use-claude-at-half-price/ | https://www.govtech.com/artificial-intelligence/as-its-own-ai-tool-expands-california-will-use-anthropic-too | https://www.foxbusiness.com/politics/newsoms-office-touts-anthropic-partnership-50-discount-claude-ai-california-agencies-localities | https://insider.govtech.com/california/news/state-strikes-anthropic-deal-with-poppy-expansion-close-behind
- **Timeliness**: 4 天前（2026年6月29日，Newsom 官方宣布）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 同一家 AI 公司，在同一周，同时经历了两件事：联邦政府关停它的旗舰模型（Fable 5，6月12日），以及一个州政府以历史上最大规模的政府 AI 采购协议之一给它做背书（加州，6月29日）。

  这不是巧合，这是 AI 基础设施政治化的一个清晰截面。

  加州的这项协议背后有两层逻辑，需要分开看。

  第一层是采购逻辑：**Poppy 是一个已经在2800名公务员中跑通了 pilot 的政府 AI 助手**，7月要全面铺开，加州需要降低调用成本——Anthropic 给 50% 折扣，两边都有利益。这是政府AI采购从"实验性项目"走向"常规基础设施"的一次标志性落地：过去政府 AI 项目通常是1-2年的 PoC，Poppy 在 67 个部门2800人 pilot 之后直接全州铺开，这个时间线比大多数企业 AI 部署还要快。

  第二层是政治逻辑：**Newsom 选择在 Fable 5 出口管制解禁的同一周宣布这个协议**，时机不是偶然的。加州长期在 AI 监管问题上跟联邦政府持不同立场——Newsom 主张监管应促进创新，而非阻碍；Trump 行政当局则把 AI 前沿能力视为国家战略资产加以管控。两种逻辑在同一个时间点交汇：联邦说"这个 AI 是国家安全风险"，加州说"这个 AI 是我们政府的官方工具"。

  对理解 AI 产品部署轨迹的人来说，这件事透露了一个重要信号：**政府是下一个大规模 AI 部署场景，但进入路径不是联邦政府，而是州政府**。美国联邦政府因为安全和采购流程的复杂性，AI 采购周期极长；加州作为 GDP 相当于全球第五大经济体的超级州，它的政府 AI 采购决定本身就是一个足够大的市场事件。Anthropic 和加州的协议，可能比任何一个联邦合同更能加速 Claude 在政府场景的标准化。

  中文媒体会报"美国加州政府用 Claude 了"，不会分析：**这是联邦-州两级政府在 AI 上的政策分裂第一次通过采购合同具象化——同一个 AI 公司，既是联邦眼中的受管控者，也是州政府眼中的官方伙伴**。

- **Resonance hook**: 6月29日，加州州长 Newsom 宣布：全州所有政府机构，以半价使用 Claude。同一周，联邦政府刚刚解除了对 Claude Fable 5 长达19天的全球禁令。同一个 AI 公司，联邦叫停它，加州选它。Poppy，一个已经在2800名加州公务员里 pilot 的 AI 助手，7月全面铺开。政府 AI 采购正在发生，入口在州，不在联邦。
- **Recommended priority**: high

---

## Candidate 3: OpenAI 用自家 AI 设计了自己的第一块芯片——Jalapeño 推理芯片 9 个月完成 tape-out，目标是把推理成本砍掉一半（June 24）

- **Event**: 2026年6月24日，**OpenAI 与 Broadcom** 联合发布 **Jalapeño**——OpenAI 历史上首款自研 AI 推理芯片（ASIC），基于 TSMC 3nm 工艺制造，专为 LLM 推理（inference）场景优化，面积接近光刻极限（reticle-sized）。核心参数与细节：① **开发周期：9个月**从设计到 tape-out，Broadcom 描述为"AI芯片史上最快的高性能ASIC开发周期"；② 架构：脉动阵列（systolic array）+ 8栈 HBM 内存，通过 2.5D interposer 封装，最小化计算和内存之间的数据移动延迟（推理延迟的主要来源）；③ 目标：**比当前 NVIDIA GPU 推理性能/瓦特高出显著幅度**，OpenAI 内部目标是将推理成本降低约 50%；④ **关键元信息**：Jalapeño 的设计过程本身使用了 OpenAI 自己的 AI 模型——OpenAI 用 AI 设计了 AI 的基础设施；⑤ 部署计划：2026年底小批量上线，2027-2028年全面铺开，OpenAI 与 Broadcom 承诺 2026年底至2029年间共部署 **10 吉瓦（10 GW）** 的此类加速器算力；⑥ **Microsoft 将采购约 40% 的首批产量**（Microsoft 是 OpenAI 最大投资方和云基础设施合作方，Jalapeño 将在 Azure 数据中心部署）；⑦ 定位明确：**Jalapeño 仅用于推理，不替代 NVIDIA GPU 用于训练**——OpenAI 仍是 NVIDIA 最大训练算力客户之一。来源：**OpenAI 官方博客**（2026年6月24日，《OpenAI and Broadcom unveil LLM-optimized inference chip》）、**TechCrunch**（2026年6月24日，《OpenAI unveils its first custom chip, built by Broadcom》）、**CNBC**（2026年6月24日，《OpenAI and Broadcom reveal Jalapeno, first AI chip in partnership》）、**VentureBeat**（2026年6月24日，《OpenAI unveils first custom AI inference chip, Jalapeño, with Broadcom — and its development was sped-up with OpenAI's own models》）、**Tom's Hardware**（2026年6月24日，《Broadcom and OpenAI unveil custom-built Jalapeño inference processor》）、**Medium/Noah Bean**（《OpenAI and Broadcom's Jalapeño Is Not an Nvidia Story. It's a Unit Economics Story.》）。
- **Source**: https://openai.com/index/openai-broadcom-jalapeno-inference-chip/ | https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/ | https://www.cnbc.com/2026/06/24/openai-and-broadcom-reveal-jalapeno-first-ai-chip-in-partnership.html | https://venturebeat.com/infrastructure/openai-unveils-first-custom-ai-inference-chip-jalapeno-with-broadcom-and-its-development-was-sped-up-with-openais-own-models | https://www.tomshardware.com/tech-industry/artificial-intelligence/broadcom-and-openai-unveil-custom-built-jalapeno-inference-processor-openais-first-chip-is-a-massive-reticle-sized-asic-built-in-an-ultra-fast-nine-month-development-cycle
- **Timeliness**: 9 天前（2026年6月24日，OpenAI + Broadcom 官方联合发布）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 中文媒体的报道基本停在"OpenAI 要对抗 NVIDIA"的叙事框架上，但这个框架是错的。

  Jalapeño 不是训练芯片，是推理芯片。OpenAI 并没有计划用 Jalapeño 替代 NVIDIA 做模型训练——它仍然是 NVIDIA 最大的训练算力客户之一，这一点没有任何改变。所以"挑战 NVIDIA"这个叙事从一开始就选错了维度。

  Jalapeño 的真实意图是：**解决 OpenAI 商业模式的单位经济学问题**。

  逻辑是这样的：ChatGPT、Claude Code、Codex 这类产品，核心成本是推理成本（用户每发一条消息，模型就要跑一次 forward pass）。推理成本直接决定产品是否能盈利——GPT-5.5 的推理成本如果高于用户支付意愿的上限，这个产品就是在每笔交易上亏损。OpenAI 的目标是让每次 ChatGPT 回复、每次 Codex 任务执行，比现在用 NVIDIA H100 便宜 50%。推理成本降一半，意味着要么同等成本服务两倍用户，要么同等收入获得两倍利润率。

  这才是 Jalapeño 的商业逻辑核心：**它是 OpenAI 从"烧钱换份额"到"单位经济学正向"的关键路径之一**。这也解释了为什么 Microsoft 会承购约 40% 的首批产量——Microsoft 在 Azure 上运行 OpenAI 的推理服务，推理成本每降一分都直接改善 Azure OpenAI 服务的毛利率。

  还有一个细节值得单独拎出来：**Jalapeño 的设计过程本身用了 OpenAI 的 AI 模型来加速**。这是"AI 设计 AI 基础设施"第一次以商用芯片的形式被公开披露。9个月完成 tape-out（业界通常需要18-24个月），部分原因就在于此。这不是彩蛋，这是 AI 开始加速自身基础设施迭代速度的一个实证数据点。

  中文媒体会报"OpenAI 出了自己的芯片"，不会分析：**Jalapeño 不是硬件竞争故事，是单位经济学故事——以及 AI 用来设计 AI 芯片这件事本身，意味着下一代 AI 基础设施的迭代速度将不再受制于人类的设计周期。**

- **Resonance hook**: 6月24日，OpenAI 和 Broadcom 发布了 Jalapeño——OpenAI 第一块自研 AI 芯片，9个月完成 tape-out。但 Jalapeño 不是"打 NVIDIA"，它只做推理，不做训练。它要解决的是 ChatGPT 和 Codex 每次回复的算力成本——目标是降 50%。还有一个细节：这块芯片的设计过程本身用了 OpenAI 自己的 AI 模型来加速。AI 开始设计自己的基础设施。
- **Recommended priority**: medium-high

---

## Scan summary

**Sources scanned**:
- llm-stats.com（2026年7月更新，《AI Updates Today July 2026》）
- buildfastwithai.com（2026年7月1日，《AI News Today July 1 2026: 15 Biggest Stories》）
- dentro.de（2026年7月，《AI News - July 2026: Key Events & Releases》）
- NVIDIA Research GEAR Lab（research.nvidia.com/labs/gear/aspire/，2026年7月1日）
- arXiv 2607.00272（2026年6月30日预印，ASPIRE 论文）
- Hugging Face Papers（2607.00272，2026年7月1日高亮）
- TechTimes（2026年7月1日，《Robot Skill Library ASPIRE Gives Robots Memory: Handover Climbs to 92%》）
- NVIDIA Newsroom（《NVIDIA Accelerates Robotics Research and Development With New Open Models and Simulation Libraries》）
- Jim Fan X/Twitter（2026年7月1日，ASPIRE 开源帖）
- Governor of California 官方新闻稿（2026年6月29日）
- TechCrunch（2026年6月29日，《Anthropic and Gov. Newsom forge deal》）
- GovTech（2026年7月1日，《As Its Own AI Tool Expands, California Will Use Anthropic Too》）
- Fox Business（2026年6月29日，Newsom Anthropic deal 报道）
- GovTech Insider（《State Strikes Anthropic Deal With Poppy Expansion Close Behind》）
- OpenAI 官方博客（2026年6月24日，《OpenAI and Broadcom unveil LLM-optimized inference chip》）
- TechCrunch（2026年6月24日，Jalapeño 报道）
- CNBC（2026年6月24日，Jalapeño 报道）
- VentureBeat（2026年6月24日，Jalapeño 报道）
- Tom's Hardware（2026年6月24日，Jalapeño 技术分析）
- Medium / Noah Bean（《Jalapeño Is Not an Nvidia Story. It's a Unit Economics Story.》）
- arXiv 2606.24597（2026年6月24日，Qwen-AgentWorld，排除：9天窗口 + 深层AI思考柱与 ASPIRE 重叠）
- Google Blog（2026年6月30日，Nano Banana 2 Lite + Gemini Omni Flash，排除：生成式媒体赛道，与 Zico 主题柱契合度低）
- Qualcomm 官方（2026年6月24日，Modular 收购协议，排除：信息增量不及 Jalapeño + 中文媒体覆盖度更低但叙事层次相似）
- xAI / SpaceX S-1（Anthropic 计算合同，排除：披露时间为5月20日，超出30天窗口）
- OpenAI IPO S-1（2026年6月8日，排除：超出7天最优窗口且叙事停在财务层面，无产品/战略新增量）
- Karpathy AutoResearch Loop（排除：2026年3月发布，超出30天窗口）
- Karpathy / Altman X 7月1-2日帖子（无独立可锚定新帖，排除）
- GitHub Trending AI tools（7月汇总，无独立叙事锚点可用于候选）

**Total signals found**: 约 22 个信号评估

**Why these 3**:

- **Candidate 1（NVIDIA ASPIRE，7月1日）**：**深层AI思考柱**——时效最强（2天前），Tier 1 源（NVIDIA 官方 + Jim Fan X，Jim Fan 是 playbook 明确列出的 KOL 之一）；20%→92% 的具体数字是发现式钩子；"训练输出从模型权重变成技能库"这一范式声明在中文媒体完全停在性能数字层面，无任何深度范式分析；与 Zico 的空间智能/Physical AI 背景（酷家乐 3DGS）有直接交集；7月1日 ASPIRE 开源也与 Fable 5 同日全球恢复形成同日双重发布节点，增加时效锚定价值；过去3天候选（Agents-A1 / Gemini 2.5 Deep Think）均已覆盖深层AI思考柱但聚焦在推理 scaling 和模型能力，ASPIRE 聚焦的是**训练范式**，角度完全不同；**HIGH 优先级**。

- **Candidate 2（Anthropic + California Newsom，6月29日）**：**组织形式变革柱**——时效4天（可接受），角度与7月2日已选中的 Fable 5 故事完全不同（Fable 5 = 联邦管控 AI 基础设施，Newsom = 州政府以采购形式为 Anthropic 背书）；两个故事放在一起形成完整叙事张力：同一家公司，同一周，被联邦管控 + 被州政府采购；Poppy 2800人 pilot → 全州铺开是 AI 进入政府组织的具体数据锚点；"联邦 vs 州政府的 AI 政策分裂"这一叙事在中文圈完全缺失（中文媒体只会报"美国政府又有新 AI 动向"）；与 Fable 5 故事（昨天 063 草稿）可构成"三部曲"第二篇（Fable 5 = AI 基础设施的脆弱性 → Newsom = AI 在政治地理中的分裂部署）；**HIGH 优先级**。

- **Candidate 3（OpenAI Jalapeño，6月24日）**：**AI产品战略柱**——时效9天（略超7天最优窗口，但30天窗口内可接受），该柱最近选中时间约在7月1日（Claude Science Workbench），角度不同（工作流 vs 单位经济学）；"AI 设计 AI 芯片"这一元信息点在中文媒体几乎零覆盖（媒体集中在"OpenAI 对抗 NVIDIA"叙事，完全忽视了 Jalapeño 仅做推理 + 设计用 AI 加速这两个关键点）；单位经济学框架（推理成本 → 商业模式 → 产品可持续性）与 Sonnet 5 tokenizer 隐性成本候选（6月30日）形成同主题下不同层次的呼应；Microsoft 购入40%产量这一供应链细节揭示了 Azure OpenAI 商业逻辑，信息增量高；**MEDIUM-HIGH 优先级**。
