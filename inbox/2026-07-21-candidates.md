---
date: 2026-07-21
status: written
selected: candidate 1 → drafts/082-android-agent-surface-xhs.md
---

# Today's Candidates

## Candidate 1: EU DMA 正式命令 Google 向 ChatGPT 和 Claude 开放 Android 系统级入口——Gemini 独占的唤醒词、Home 键触发、全屏读取权将向所有 AI 助手开放（July 16–20, 2026）

- **Event**: 2026年7月16日，欧盟委员会依据《数字市场法》（DMA）采纳两项具有立即法律约束力的命令：（1）**Google 必须向竞争对手 AI 助手开放 Android 上当前 Gemini 独占的 11 个系统级功能**——包括唤醒词识别（wake word detection，操作系统音频层）、Home 键长按触发、全屏内容读取（screen reading）、跨 App 任务执行（cross-app execution）；（2）**Google 必须从 2027年1月起向竞争 AI 服务商共享匿名化 Google Search 查询、点击和排名数据**。受益方直接包括：**OpenAI ChatGPT、Anthropic Claude、Perplexity**。Android 全球移动操作系统市场份额约 **70%**，全球约 **30 亿台** 设备运行 Android。实施时间线：Google 须于 2026 年 8 月底提交合规申请表，2027 年 8 月 1 日前在 Android 18 上向所有合资格 AI 助手开放全部 11 项功能。不合规罚款上限为 Alphabet 全球年收入的 **10%**（潜在超过 **300 亿美元**）。2026年7月9日，欧盟法院驳回 Google 最后一项法律抗辩，给予 18 天合规期——这是 7 月 16 日命令的直接前提。TechTimes 在 2026年7月20日发布全面实施分析。来源：CNBC（7月16日）、TechTimes（7月16日、7月20日）、The Next Web（7月16日）、Unite.AI、Business Standard（7月20日）。
- **Source**: https://www.cnbc.com/2026/07/16/google-required-to-open-up-to-ai-search-engine-rivals-under-eu-mandated-changes.html | https://www.techtimes.com/articles/321118/20260720/eu-orders-google-break-geminis-android-lock-search-data-sharing-starts-january.htm | https://thenextweb.com/news/google-eu-android-gemini-rivals-dma | https://www.techtimes.com/articles/320760/20260716/eu-gives-rival-ai-assistants-system-level-android-access-google-reserved-gemini.htm | https://www.business-standard.com/technology/tech-news/how-eu-s-dma-puts-apple-and-google-on-different-paths-for-smartphone-ai-126072000734_1.html
- **Timeliness**: 5天前（命令采纳日 7月16日）；7月20日 TechTimes 全面分析（1天前）
- **Topic pillar**: Agent经济
- **Zico's angle**: 唤醒词识别、Home 键触发、全屏读取、跨 App 执行——这四个功能加在一起，是 AI 助手作为移动端 Agent 的完整动作表面（action surface）。

  先把差距说清楚。一个只能在对话框里接受文字输入的 AI，和一个可以实时读取你的屏幕、响应你的声音、按下 Home 键就能启动、然后跨 App 完成多步骤任务的 AI——这两者之间的差距，不是能力差距，是架构差距。前者是工具，后者是 Agent。

  Gemini 目前在 Android 上独占的，正是这套 Agent 基础设施。不是因为 Google 的模型能力更强，而是因为 Google 既做模型又做操作系统——它把 Agent 的动作入口绑定在了自己的 AI 上。ChatGPT 和 Claude 不是因为不够强而没有唤醒词触发，是因为 Android 的系统 API 层不对外开放。

  EU 的 DMA 命令把这个绑定切断了。2027年8月起，在欧盟地区，ChatGPT、Claude、Perplexity 可以注册自己的唤醒词，可以响应 Home 键长按，可以读取屏幕内容，可以跨 App 执行任务。动作表面从 Gemini 专属变成了开放市场。

  这件事对 Agent 经济的直接含义：当所有 AI 助手获得相同的 OS 级动作入口，竞争从「谁有更好的分发特权」变成「谁在这个动作表面上能做更多」。一旦 Claude 和 ChatGPT 在 Android 上有了 screen reading 能力，Agent 能力的上限不再受限于 Google 的 API 开放意愿，而是受限于各自的推理能力和 Tool use 设计质量。

  这也有一个被忽视的战略含义：Search 数据共享（2027年1月起）意味着 Claude 和 ChatGPT 在回答实时搜索类问题时，可以从 Google 的检索排名数据中受益——这不只是竞争公平问题，是 AI 回答质量的数据基础设施重新分配。

  中文报道会说「欧盟罚 Google」——不会分析：**EU DMA 把 Android 的 Agent 动作表面从 Gemini 的护城河变成了开放竞争赛道。这是移动端 Agent 经济分发格局的结构性重写，不是监管故事。**

- **Resonance hook**: 7月16日，欧盟命令 Google：你 Gemini 在 Android 上独享的唤醒词识别、Home 键触发、全屏读取、跨 App 执行——这四个系统级入口，ChatGPT 和 Claude 也得有。30 亿台 Android 设备，2027 年 8 月前全面开放。不合规罚款上限超 300 亿美元。Gemini 的护城河不是模型能力，是 OS 独占——EU 刚把这道门打开了。当每个 AI 助手都有同等的移动端动作表面，比的就只剩下：你用这个表面能做什么。
- **Recommended priority**: high

---

## Candidate 2: WAIC 2026 闭幕：四家中国 AI 实验室在同一窗口发布万亿参数模型，官方叙事从「参数竞争」切换到「产业交付」——Alibaba Qwen3.8 是这场协同的最新一笔（July 17–20, 2026）

- **Event**: 2026年7月17-20日，**第九届世界人工智能大会（WAIC 2026）**在上海举办，今日（7月20日）闭幕。大会期间超过 **300 个 AI 产品全球首发**，**29 个国家签署协议成立 WAICO（世界人工智能合作组织）**，习近平发表主旨讲话，联合国秘书长古特雷斯出席。最关键的产品动作：**2026年7月19日**，**Alibaba Qwen 团队** 在 WAIC 期间预发布 **Qwen3.8-Max-Preview**——**2.4 万亿参数**，多模态，声称性能「仅次于 Anthropic Claude Fable 5」（自报，无独立基准测试）。Qwen3.8-Max-Preview 立即在 Qoder（Alibaba AI 原生 IDE）、TokenPlan（AI 代码沙盒）、QoderWork（企业低代码协作平台）上以 **10% 折扣**对开发者开放。Alibaba Qwen 账号在 X 上表示将「very soon」开放权重。与此同时，同一两周窗口内，四家中国顶级 AI 实验室各自完成万亿参数发布：**Moonshot AI Kimi K3（2.8 万亿，7月16日）、Alibaba Qwen3.8（2.4万亿，7月19日）、MiniMax M3（MSA 架构，发布规格未披露）**，以及 SenseTime 和 iFlytek 各自在 WAIC 上首发新版旗舰。富途牛牛 WAIC 2026 现场报道标题：《大模型进入万亿参数时代，国内 AI 超算集群展开激烈角逐》。WAIC 官方主题定调：从「大模型单点突破」转向「全产业链系统性变现」。来源：SiliconANGLE（7月19日）、MarkTechPost（7月19日）、Futunn WAIC 2026 现场（7月20日）、Dataconomy（7月20日）、Pandaily（7月20日）、People's Daily（7月20日）。
- **Source**: https://siliconangle.com/2026/07/19/alibaba-previews-qwen3-8-claims-second-claude-fable-5/ | https://www.marktechpost.com/2026/07/19/alibaba-previews-qwen3-8-max-a-2-4-trillion-parameter-multimodal-model-days-after-moonshots-kimi-k3-open-weight-launch/ | https://news.futunn.com/en/post/76238059/live-from-waic-2026-large-models-enter-the-trillion-parameter | https://dataconomy.com/2026/07/20/qwen3-8-24t-parameters-alibaba-ai-model-launch/ | https://finance.biggo.com/news/7946b09f-3589-4999-9a49-3162a31b0c5a | http://en.people.cn/n3/2026/0720/c90000-20479401.html
- **Timeliness**: 1天前（Qwen3.8 预发布 7月19日；WAIC 2026 今日7月20日闭幕）
- **Topic pillar**: AI产品战略
- **Zico's angle**: WAIC 2026 的主题不是哪个模型的参数最多。是中国 AI 产业公开宣布了一次策略切换。

  先把切换说清楚。2025 年的 WAIC，中国 AI 公司争的是谁的旗舰模型评测分最高。2026 年 WAIC，官方叙事主动换挡——**"从参数竞争到产业交付"**。大会组委会和参会公司的核心话语是：不再说「我们的模型赶上了 GPT」，而是说「我们在制造业、金融、医疗里真实落地了多少」。这不是公关口径改变，是资金分配逻辑改变。

  Qwen3.8 的发布方式是这个策略的具象。2.4 万亿参数，没有独立评测数据，没有 license，没有活跃参数数——但立即嵌进了 Qoder（开发者 IDE）、TokenPlan（代码沙盒）、QoderWork（企业低代码平台）。Alibaba 不是在说「这是最好的模型」，是在说「这是 Qoder 生态的原生模型」。模型的价值通过平台分发，不通过 API 分发。这两种分发方式的差别在于：API 用户随时可以换供应商，平台用户换的代价包括迁移整个工作流。

  Kimi K3 的时机选择提供了另一个视角。Moonshot AI 的 K3 在 WAIC 开幕前一天发布（7月16日），有报道称是「与相关政府部门协调」的时机选择。这不是一家公司的产品策略，是一整个生态的协同节奏。当四家顶级实验室在同一个两周窗口各自发布万亿参数模型，表面上看是竞争，实际上是「中国 AI 产业链在 WAIC 窗口期完成了一次集体亮相」——对外的信息是：开源/开权重的中国模型已经达到美国前沿闭源模型的竞争水位，且性价比更高。

  对 AI 产品战略的具体含义：美国 AI 产业的竞争是「模型能力 vs 模型能力」（GPT-5.6 Sol vs Claude Fable 5）。中国 AI 产业的竞争正在变成「模型嵌入平台的深度 vs 平台生态的黏度」。如果你在为下一个 AI 应用选型，这两个逻辑会导出完全不同的供应商决策。

  Qwen3.8 没有评测数据，就敢自称「仅次于 Fable 5」——这个自信不来自模型能力，来自「反正我开权重，你自己跑就知道了」。这是开权重作为产品信号的最清晰运用。

- **Resonance hook**: 7月19日，WAIC 2026 期间，Alibaba 发布 Qwen3.8——2.4 万亿参数，没有评测数据，没有 license，直接嵌进了 Qoder（AI 原生 IDE）和 QoderWork（企业低代码平台），声称「仅次于 Claude Fable 5」。同一个两周内：Kimi K3（2.8T）、MiniMax M3、SenseTime 新旗舰，四家顶级实验室同窗口发布。WAIC 官方叙事今年换了：不是「我们的模型追上 GPT 了」，是「产业交付，全产业链变现」。这不是参数军备竞赛，是中国 AI 产业在对外宣布一次集体策略切换——从评测竞争，到生态锁定。
- **Recommended priority**: high

---

## Candidate 3: CuspAI 完成 4.5 亿美元 B 轮——Bezos + Nvidia + UK 政府联合押注 AI 材料发现，LeCun 和 Hinton 同时在顾问委员会（July 20, 2026）

- **Event**: 2026年7月20日，英国剑桥 AI 初创公司 **CuspAI** 宣布完成 **4.5 亿美元（约合 3.38 亿英镑）Series B** 融资，估值 **26 亿美元**（9 个月前 Series A 估值仅 5.2 亿美元，9 个月涨 5 倍）。领投方：**Kleiner Perkins**（硅谷顶级 VC）和 **New Enterprise Associates（NEA）**；跟投方：**英国政府**、**Jeff Bezos 投资基金（Bezos Expeditions）**、**AMD Ventures**、**Lux Capital**。战略合作：**Nvidia**（为 CuspAI 的 AI 材料计算网络提供 GPU 基础设施）。**顾问委员会**：**Yann LeCun**（Meta 首席 AI 科学家，深度学习三巨头之一）、**Geoffrey Hinton**（2024 年诺贝尔物理学奖得主，AI 领域声望最高的两人之一同时挂名）。联合创始人：**Max Welling**（深度学习研究员）。核心产品：**AI Materials Foundry**——客户输入所需材料的物理特性（如特定半导体参数、碳捕获效率指标），AI 系统在巨大的材料化学空间中搜索候选化合物，输出可实验验证的候选方案。联盟合作伙伴超过 **48 家**，包括 **Nvidia、Meta、Hyundai**。现有应用：芯片制造用新型半导体材料、固态电池电解质、工业用碳捕获化合物。CNBC 标题：《Bezos backs CuspAI as startup teams up with Nvidia to hunt for chipmaking materials》（2026年7月20日）。来源：CNBC（7月20日）、Yahoo Finance（7月20日）、KFGO / Reuters（7月20日）、CryptoBriefing（7月20日）、Tech Funding News（7月20日）。
- **Source**: https://www.cnbc.com/2026/07/20/bezos-cuspai-new-chip-materials-nvidia.html | https://finance.yahoo.com/technology/ai/articles/bezos-backs-ai-startup-discover-050020599.html | https://kfgo.com/2026/07/20/uk-government-bezos-back-cuspais-450-million-round-as-startup-seeks-to-discover-new-materials/ | https://cryptobriefing.com/bezos-invests-cuspai-450m-funding-round/ | https://techfundingnews.com/cuspai-400m-series-b-2-6b-valuation-bezos-materials-search/
- **Timeliness**: 1天前（2026年7月20日，CNBC / Yahoo Finance / Reuters 同日首发）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: AI 正在设计制造下一代芯片所需的原材料。这件事的结构，是 AI 第一次在自己的物理供应链上闭环。

  先把传统路径还原。更好的 AI → 需要更好的芯片 → 更好的芯片需要新型半导体材料 → 新型材料的发现需要材料科学家在实验室里花 10-15 年时间逐步筛选。这个流程里，每一步都是人类主导的，每一步的瓶颈都是人的时间和认知带宽。

  CuspAI 把 AI 插入了「材料发现」这一步。AI 在化合物空间里搜索候选材料——这个空间的规模，超出了任何人类研究团队穷尽的范围。Nvidia 为这个搜索提供 GPU，意味着它同时是搜索工具的运行基础设施，也是搜索结果（新型芯片材料）的潜在受益者。这个利益结构让 Nvidia 成为 CuspAI 的天然战略伙伴，而不仅仅是客户。

  LeCun 和 Hinton 同时出现在顾问委员会这件事值得特别注意。这两个人在 AI 领域的分歧是公开的：LeCun 认为当前 LLM 路径无法达到 AGI，对 AI 存在风险的判断最为保守；Hinton 是最早公开呼吁 AI 安全警惕的「教父」之一，2024 年因 AI 风险立场离开 Google。他们在几乎所有 AI 战略判断上都站在不同阵营——但两人同时选择了 CuspAI。这个交集的意义：**把 AI 用于加速物理世界的科学发现，是技术乐观派和技术悲观派都认可的 AI 正向用途**。这不是小事。

  Zico 的 3DGS 和 Physical AI 框架里，这件事是「AI 从数字空间向物理世界渗透」的又一个具体路径。不是 AI 控制机器人执行动作，而是 AI 在比任何实验室都大的化合物空间里做基础科学发现——然后把发现交给人类实验室验证和制造。这是 AI 作为「认知加速器」在物理科学领域的实体化。

  如果成功，这个闭环意味着：AI 发现新材料 → 新材料制成更好的芯片 → 更好的芯片训练更强的 AI → 更强的 AI 发现更好的材料。这个正反馈回路，第一次在数字世界之外找到了真实的锚点。

- **Resonance hook**: 7月20日，剑桥 AI 初创公司 CuspAI 融资 4.5 亿美元，估值 26 亿。Bezos 投，Nvidia 战略合作，英国政府参投。顾问委员会两个名字：LeCun 和 Hinton——深度学习最具代表性的「乐观派」和「悲观派」，在这件事上站在同一边。CuspAI 做的是：你给出材料特性需求（比如芯片用半导体参数），AI 在化合物空间里帮你找候选物质。下一代芯片的原材料，正在由 AI 来找。AI 正在加速自己的物理供应链。当 LeCun 和 Hinton 都投票给同一个方向，那个方向值得看一眼。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**:
  - BuildFastWithAI（2026年7月20日，16 Biggest Stories：EU DMA Google、WAIC 闭幕、Gemini 3rd delay）
  - TechTimes（7月16日、7月20日：EU DMA Google Android binding orders + 全面分析）
  - CNBC（7月16日：Google DMA compliance；7月20日：Bezos CuspAI Nvidia）
  - The Next Web（7月16日：EU prepares to force Google）
  - Business Standard（7月20日：EU DMA puts Apple and Google on different paths）
  - SiliconANGLE（7月19日：Alibaba Qwen3.8 preview）
  - MarkTechPost（7月19日：Qwen3.8-Max 2.4T multimodal）
  - Dataconomy（7月20日：Qwen3.8 launch）
  - Futunn WAIC 2026 现场报道（7月20日：万亿参数时代、产业交付叙事）
  - BigGo Finance（7月20日：WAIC 2026 Preview 从模型竞争到产业交付）
  - People's Daily（7月20日：中国大模型再次震撼世界）
  - Pandaily（7月20日：Qwen3.8 开放权重策略）
  - Yahoo Finance / KFGO / Reuters / CryptoBriefing / TechFundingNews（7月20日：CuspAI $450M）
  - TechStartups（7月20日 综合 Top Tech News：Alibaba、Bezos、Blackstone、Google、Nvidia）
  - LLM Stats（July 2026 模型更新：Qwen3.8-Max-Preview 规格核实）
  - Anthropic.com / Anthropic Research（Claude Code Expertise 论文 6月16日——排除，超窗口）
  - Future of Life Institute（AI Safety Index Summer 2026，7月7日——排除，超14天）
  - Illinois SB 315（7月6日——排除，超14天）
  - Karpathy AutoResearch（2026年3月——排除，超窗口）
  - Oracle 30,000 layoffs（2026年3月——排除，超窗口）
  - WAICO（主要事件 7月16-17日，已在 7月18日候选中覆盖——排除重复）
  - Gemini 3.5 Pro 三次延误（7月16日，已在 7月17日候选中覆盖——排除重复）
  - aiagentstore.ai（AI Agents News Week of July 19, 2026——无具体7天内有时效锚点的 Agent 事件，排除）
  - arXiv（Embodied AI / World Models July 2026 论文波——无具体7天内时效事件锚点，排除）

- **Total signals found**: 约 20 个独立信号评估，含：EU DMA Google Android binding orders（7/16）、Qwen3.8-Max WAIC preview（7/19）、CuspAI $450M Bezos Nvidia（7/20）、WAIC 2026 闭幕 + WAICO（7/16-20，主体已覆盖 7/18）、Gemini 3.5 Pro 3rd delay（7/16，已覆盖 7/17）、Illinois SB 315（7/6，超窗口）、Future of Life Institute AI Safety Index（7/7，超窗口）、Karpathy AutoResearch（3月，超窗口）

- **Why these 3**:
  - **Candidate 1（EU DMA Google Android，7月16-20日）**：**Agent经济柱**——该柱上次入选 7月20日（Acemoglu 诺贝尔经济学家改变立场）和 7月18日（Kimi K3 Swarm Max 成本结构），今日角度完全不同（OS 系统级入口 = Agent 动作表面，EU 监管正在重写移动端 Agent 分发格局）；7月16日 binding orders，7月20日 TechTimes 全分析，时效合规；ChatGPT/Claude/Perplexity 受益方都是具体真实公司；中文媒体报「欧盟又对谷歌开罚了」，不会分析「OS 系统级 API 开放如何改变 Agent 在移动端的动作表面，以及 Search 数据共享如何重写 AI 检索能力的数据基础设施」；**HIGH 优先级**。
  - **Candidate 2（WAIC 2026 + Qwen3.8 + 中国 AI 策略切换，7月17-20日）**：**AI产品战略柱**——该柱上次入选 7月19日（Grok 4.5 + Cursor 数据飞轮）和 7月18日（Thinking Machines Inkling），今日角度完全不同（WAIC 官方叙事从参数竞争切换到产业交付，Qwen3.8 通过平台嵌入而非 API 做模型分发）；Qwen3.8 7月19日发布（2天前），WAIC 今日闭幕；四家中国实验室同窗口发布有 Futunn 等多家新闻源确认；中文媒体会报「阿里发布最大参数模型」，不会分析「从参数军备竞赛到生态锁定的策略切换，以及开权重作为平台分发载体的产品逻辑」；**HIGH 优先级**。
  - **Candidate 3（CuspAI $450M Bezos + Nvidia + LeCun/Hinton，7月20日）**：**深层AI思考柱**——该柱上次入选 7月20日（GPT-5.6 Sol Ultra 数学证明）、7月19日（Cosmos 3 Edge）、7月18日（AI监管三巨头护城河），角度完全不同（AI 发现芯片材料 = AI 在自己的物理供应链上闭环，这是 AI 作为新物种跨越数字-物理边界的具体实例）；今日7月20日首发，时效最强；LeCun + Hinton 同时顾问是高度反常的共识信号（顶级分歧者的交集 = 高信息量）；中文媒体会报「Bezos 投资了一家英国 AI 公司」，不会分析「AI 正在发现自己运行所需的物理材料，这个正反馈回路的深层含义」；**HIGH 优先级**。
  - **排除信号**：WAICO 7/16-17（7月18日扫描已覆盖）；Gemini 3.5 Pro 3rd delay 7/16（7月17日已覆盖）；AI Safety Index 7/7（超14天窗口）；Illinois SB 315 7/6（超14天窗口）；Karpathy AutoResearch（3月，超窗口）；Oracle layoffs（3月，超窗口）；AI协作实践柱（无具体7天内时效事件锚点，Anthropic Claude Code Expertise 论文 6月16日超窗口）。
  - 三者覆盖三个不同主题柱（Agent经济 / AI产品战略 / 深层AI思考），时效分别为5天+1天分析 / 1-2天 / 1天，与过去3天已入选候选无重叠（Agent经济：OS动作表面 vs 成本结构/经济学家立场；AI产品战略：中国平台生态切换 vs 数据飞轮/定制化路径；深层AI思考：AI物理供应链闭环 vs 数学证明/边缘世界模型/监管护城河）。
