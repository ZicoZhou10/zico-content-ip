---
date: 2026-07-18
status: pending_selection
---

# Today's Candidates

## Candidate 1: Moonshot AI 发布 Kimi K3——2.8万亿参数 MoE，「K3 Swarm Max」专为百级 Agent 并发编排设计，市场闪回 DeepSeek（July 16–17）

- **Event**: 2026年7月16日，**Moonshot AI**（月之暗面）无媒体发布会直接上线 **Kimi K3**，先行渠道为 Kimi Code 和 Kimi App，**Kimi Open Platform** API 同步开放。规格：（1）**2.8万亿（2.8T）总参数**，Stable LatentMoE 架构，每次推理激活 **896 个专家中的 16 个**，实际推理算力显著低于同等参数的密集模型；（2）**1M token 上下文**；（3）两个变体：**K3 Max**（日常 Agent 任务循环）和 **K3 Swarm Max**（大规模并发批处理，单次任务可扇出至**数百个并发子 Agent**，基于 Kimi Work 已有的 Agent 群编排能力扩展）；（4）**API 定价：$3.00/M input、$15.00/M output**；（5）自报基准：超过 Claude Opus 4.8 Max 和 GPT-5.5 High，在前端代码 Arena 评分上超过 Claude Fable 5，仅在少数测试中落后 GPT-5.6 Sol；（6）**开放权重版本承诺 7 月 27 日发布**。7 月 17 日，Axios 以《China just erased America's AI lead》为题报道，美国科技股盘中下跌——Fortune 称其引发**"DeepSeek 闪回"效应**，投资者识别出熟悉的模式：中国高质量开源模型出现 → 美国 AI 成本假设再次被冲击。

- **Source**: https://www.axios.com/2026/07/17/china-ai-kimi-k3-open-source-anthropic-opus | https://techcrunch.com/2026/07/16/moonshots-upcoming-kimi-3-is-expected-to-close-the-gap-with-anthropics-opus-4-8/ | https://venturebeat.com/technology/chinas-moonshot-ai-releases-kimi-k3-the-largest-open-source-model-ever-rivaling-top-u-s-systems | https://finance.yahoo.com/markets/stocks/articles/kimi-k3-just-triggered-deepseek-175532711.html | https://www.bloomberg.com/news/articles/2026-07-17/china-s-powerful-new-moonshot-ai-model-closes-gap-with-us-rivals

- **Timeliness**: 1–2天前（Moonshot AI 2026年7月16日发布；Axios / Fortune / Bloomberg 7月17日报道市场反应）

- **Topic pillar**: Agent经济

- **Zico's angle**: K3 Swarm Max 回答的是 Agent 经济里一个没被充分讨论的成本问题。

  先把数字还原。GPT-5.6 Sol 的 output 定价是 $15/M token。一个中等复杂度的 Agent 任务，假设 500 个并发子 Agent 各自消耗 5,000 个 output token，单次运行成本是 $37,500。这个数字让"Agent 经济"更像是"Agent 成本中心"——绝大多数想用 Agent 群做大规模任务的公司，在账期结束前就会退缩。

  DeepSeek 在 2025 年 1 月做的事是把这个成本方程的系数重写——高质量模型的 per-token 价格下降了 90%+。Kimi K3 Swarm Max 在做的是更进一步：不只是"便宜的前沿模型"，而是**一个架构上专为 Agent 群编排设计的前沿模型**。K3 Swarm Max 把单次任务扇出至数百个并发子 Agent，且在 MoE 稀疏激活架构下，并发成本相比密集模型有结构性优势。

  这不是"中国模型在基准测试上赶上了美国"的故事（中文媒体会这么写）。这是 **Agent 经济的基础设施成本曲线正在系统性下移**——上周 Nubia NaviX Ultra 告诉我们 Agent 的访问权壁垒在哪（App 生态不开放），这周 K3 Swarm Max 告诉我们 Agent 的成本壁垒正在哪个方向松动。

  市场的 DeepSeek 闪回是准确的模式识别。2025 年 1 月 DeepSeek 出现时，冲击的是"高能力模型需要高成本"这个假设；2026 年 7 月 Kimi K3 出现时，冲击的是"大规模 Agent 编排需要高成本"这个假设。两次冲击的结构相同：成本假设崩塌 → 原先不可行的 Agent 应用规模变得可行。

  对酷家乐场景的直接含义：如果你在考虑用 Agent 群自动化大批量设计任务，K3 Swarm Max 出现之前和之后的成本模型是两个不同的计算。

- **Resonance hook**: 7月16日，Moonshot AI 发布 Kimi K3——2.8万亿参数 MoE，K3 Swarm Max 单次任务可扇出数百个并发子 Agent。自报基准超过 Claude Opus 4.8，部分超过 Claude Fable 5。7月17日，Axios：「China just erased America's AI lead」，美国科技股闪回 DeepSeek。但这次闪回代表的不是"中国模型追上了美国"。它代表的是：大规模 Agent 并发运行的成本假设，正在被重写。

- **Recommended priority**: high

---

## Candidate 2: 前 OpenAI CTO Mira Murati 的 Thinking Machines 发布首款模型 Inkling——主动声明「不是最强」，975B 参数开源，Tinker 定制化平台才是真正的产品（July 15）

- **Event**: 2026年7月15日，**Thinking Machines Lab**（创始人：前 **OpenAI** CTO **Mira Murati**，2023 年离职创业，公司累计融资约 20 亿美元）发布首款自研模型 **Inkling**。规格：（1）**975B 总参数，41B 活跃参数**，稀疏 MoE 架构；（2）**原生四模态**：在 45 万亿（45T）token 的文本、图像、音频、视频混合数据上预训练，原生处理所有四种模态（无需拼接模块）；（3）**1M token 上下文**，Tinker 平台上提供 64K 和 256K 两种微调选项；（4）**开放权重（open-weight）**，完整权重已上传 Hugging Face；（5）同步发布 **Inkling-Small**（12B 活跃参数）；（6）**可调节思考努力（Controllable Thinking Effort）**：用户可在快速响应和深度推理之间拨动，推理成本是可控参数而非固定属性；（7）**Tinker 平台**：Inkling 在 Tinker 上开放企业领域微调，这是 Thinking Machines 的核心商业化路径。Murati 在发布声明中明确写道：**「Inkling 不是今天市场上最强的模型，无论开源还是闭源。」** TechCrunch 标题：《Thinking Machines amps up its bet against one-size-fits-all AI with its first open model, Inkling》。TechCrunch、Axios、Fortune、Bloomberg 同日报道。

- **Source**: https://techcrunch.com/2026/07/15/thinking-machines-amps-up-its-bet-against-one-size-fits-all-ai-with-its-first-open-model-inkling/ | https://www.axios.com/2026/07/15/mira-murati-thinking-machines-open-weight-model-inkling | https://fortune.com/2026/07/15/what-is-mira-murati-thinking-machines-first-ai-model-inkling/ | https://www.bloomberg.com/news/articles/2026-07-15/murati-s-thinking-machines-releases-first-ai-model-for-broad-use | https://www.marktechpost.com/2026/07/15/thinking-machines-lab-releases-inkling-a-975b-parameter-open-weights-multimodal-moe-with-41b-active-parameters-and-controllable-thinking-effort/ | https://thinkingmachines.ai/news/introducing-inkling/

- **Timeliness**: 3天前（2026年7月15日，TechCrunch / Axios / Fortune / Bloomberg 同日首发）

- **Topic pillar**: AI产品战略

- **Zico's angle**: Murati 主动声明「不是最强」，这是产品战略宣言，不是能力披露。

  先把背景还原。Murati 离开 OpenAI 时是 CTO——她比任何人都清楚 OpenAI 模型能力的天花板在哪。她用了两年时间和约 20 亿美元，做出了一个明确选择「不追最强」的模型。这个选择不是资源约束，是方向性的产品赌注。

  赌注的逻辑：如果 AI 价值链的竞争优势在「谁的基础模型最强」，那你要和 OpenAI、Google DeepMind、Anthropic 正面硬刚——这场仗极难赢。但如果竞争优势在「谁能帮企业把模型最高效地适配到自己的领域」，那你需要的不是最强模型，而是**最适合定制化的模型 + 最好的定制化平台**。Inkling 是分发载体，Tinker 才是真正的产品。

  产品架构里藏着三个信号。一，开放权重：把采用门槛降到零，最大化分发覆盖，逻辑是「先让你用上，再让你付费定制」。二，可调节思考努力：把推理成本的控制权交给用户——「这个任务值不值得深度推理」是业务判断，不应该是模型的固定属性；这个设计假设企业用户会搭建差异化的工作流，而不是统一用一个设定。三，四模态原生预训练：大多数企业的实际数据是文档 + 图像 + 音频 + 视频的混合，四模态预训练比单模态更适合做企业领域微调的起点——这是刻意为 Tinker 设计的基础。

  类比：这是 AI 时代的「吉列刀片模型」——把剃须刀（Inkling 基础模型）免费开源，赚刀片（Tinker 定制化服务）的钱。竞争对手是 Hugging Face 的开源微调生态 + 各大云厂商的 fine-tuning API，而不是 GPT-5.6 Sol 或 Claude Fable 5。

  对 AI 产品战略的一般含义：这件事提供了一个判断框架——**基础模型层的价值在下沉，定制化和集成层的价值在上浮**。Thinking Machines 用产品结构对这个判断下注了。当最了解 OpenAI 能力天花板的人选择不跟 OpenAI 打同一场比赛，这个选择值得认真解读。

- **Resonance hook**: 7月15日，Mira Murati（前 OpenAI CTO）的 Thinking Machines 发布首款模型 Inkling——975B 参数开源，原生四模态，1M token 上下文。发布声明里，Murati 直接写：「Inkling 不是今天市场上最强的模型，无论开源还是闭源。」不是道歉，是产品策略宣言：模型是免费的分发入口，Tinker（定制化平台）才是真正要卖的东西。当最懂 OpenAI 天花板的人选择不打同一场比赛，这个选择意味着什么？

- **Recommended priority**: high

---

## Candidate 3: 深度学习三巨头 CEO 同一周公开呼吁 AI 监管收敛——Altman 要 IAEA、Hassabis 要 FINRA、Amodei 要 FAA，三个方案有同一个隐藏功能（July 14–16）

- **Event**: 2026年7月14-16日，三家最大前沿 AI 实验室 CEO 在同一周内先后公开发表监管立场，方向空前一致。**Demis Hassabis（Google DeepMind）** 于7月14日接受 Axios 独家专访，呼吁建立「FINRA 式 AI 标准机构」——行业出资、联邦监管的自律机构，从自愿预发布审查开始，可升级为强制性市场准入规则，要求「年内成立」；**Sam Altman（OpenAI）** 在《金融时报》发表署名文章，呼吁「IAEA 式 AI 国际论坛」——以美国为主导，通过「模型访问权」和「市场准入」作为杠杆，认证各国、各公司和各安全标准；**Dario Amodei（Anthropic）** 呼吁「FAA 式 AI 联邦监管机构」——有权从第一天起直接阻止过危险模型发布的联邦机构。2026年7月16日，**Axios** 将三人立场汇总为封面报道《Behind the Curtain: AI godfathers converge on regulations》，称这是三人**首次在书面上共同确认「前沿 AI 需要监管」**的判断。三人的明确共识：（1）前沿模型应接受公开发布前的**外部审查**（打破行业原有的自我申报惯例）；（2）需要一个有**国际权威**的监管机构（三个提案均为**美国主导**）；（3）以国家安全（生化武器、网络攻击）为紧迫理由框架。

- **Source**: https://www.axios.com/2026/07/16/ai-regulations-openai-anthropic-google | https://www.axios.com/2026/07/14/demis-hassabis-ai-regulation-google-deepmind | https://www.cnbc.com/2026/07/14/google-deepmind-demis-hassabis-us-led-ai-standards-body.html | https://thenextweb.com/news/ai-godfathers-frontier-ai-regulation-converge

- **Timeliness**: 2–4天前（Hassabis 独家 7月14日；Axios 汇总报道 7月16日首发）

- **Topic pillar**: 深层AI思考

- **Zico's angle**: 当三个激烈竞争者在同一周公开呼吁「给我们监管」，这件事需要用竞争逻辑解读，不能用安全逻辑解读。

  先把表面叙事放一边。三人确实有真实的安全担忧——他们建造的东西确实很危险，生化武器和网络攻击的风险是真实的，不是 PR 话术。但安全担忧不能解释**为什么三个竞争对手在同一周、同一方向发声**，且三个方案都指向「美国主导的监管机构」。

  三个提案有一个共同的隐藏功能：**把「你已经有前沿模型能力」变成进入监管权力中心的门票**。FAA 模型（Amodei）：监管机构要评估模型是否够安全才能发布，评估能力来自哪里？来自有前沿模型的公司。FINRA 模型（Hassabis）：行业自律意味着现有大公司写规则，后来者执行规则——Hassabis 明确说「从自愿审核开始，硬化成强制性市场准入」，谁是规则写手，谁就是市场准入的守门人。IAEA 模型（Altman）：控制「模型访问权」的实体可以认证其他国家和公司——OpenAI 成为认证杠杆的中心节点。

  三个结构的共同点：进入监管核心的门票，是「你已经是前沿模型提供者」。监管框架如果按这个逻辑建立，实质上是把当前市场结构固化成了进入壁垒——不是用技术护城河，而是用**监管护城河**。

  时机选择是另一个信号。同一周，习近平在 WAIC 推动 WAICO（世界 AI 合作组织，上海总部）——中国要多边框架。Altman / Hassabis / Amodei 的三个提案全部是美国主导的单边框架。两个方向完全对立，争的是同一件事：谁来定义 AI 治理的规则书。Axios 封面报道出现在 WAIC 同一周，不是巧合——这是 AI 规则书写权争夺的两个棋局同步落子。

  对 Zico 的「AI 作为新物种」框架：这一周，AI 正式进入制度竞争阶段。技术竞争决定谁最强，制度竞争决定谁制定标准。最终控制 AI 生态位的，可能不是做出最强模型的公司，而是成功把自己写进治理框架的公司。

- **Resonance hook**: 7月14-16日，Altman、Hassabis、Amodei 在同一周先后公开呼吁 AI 监管——Altman 要 IAEA、Hassabis 要 FINRA、Amodei 要 FAA。Axios 汇总：三人首次在书面上一致确认「前沿 AI 需要监管」。表面叙事：科技领袖负责任地呼吁监管。另一个读法：三个提案共享同一个隐藏功能——把「你已经有前沿模型」变成进入监管权力中心的门票。监管框架一旦建立，当前市场结构就被固化成了进入壁垒。这不是安全共识，是护城河建设。同一周，习近平在 WAIC 推 WAICO（AI 版 WTO，上海总部）。两个棋局同步落子。

- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**:
  - Axios（2026年7月17日，《China just erased America's AI lead》Kimi K3 市场反应；7月16日，《Behind the Curtain: AI godfathers converge on regulations》AI 监管收敛；7月16日，DeepMind 生物安全计划；7月15日，Thinking Machines Inkling；7月14日，Demis Hassabis AI regulation 独家专访）
  - TechCrunch（7月16日，Kimi K3；7月15日，Thinking Machines Inkling；7月8日，AI startup 收入增速）
  - VentureBeat（7月16日，Kimi K3 最大开源模型）
  - Fortune（7月17日，Kimi K3 DeepSeek shock；7月16日，Kimi K3 Fable-level；7月15日，Thinking Machines Inkling）
  - Bloomberg（7月17日，Kimi K3；7月15日，Thinking Machines Inkling）
  - Yahoo Finance / Tom's Hardware / CNBC（Kimi K3 市场反应与规格）
  - MarkTechPost（7月16日，Kimi K3 架构细节；7月15日，Inkling 技术参数）
  - simonwillison.net（7月16日，Kimi K3 + Inkling 综述）
  - thinkingmachines.ai（Inkling 官方博客）
  - The Next Web（7月16日，AI godfathers regulation convergence）
  - CNBC（7月14日，Hassabis US-led AI standards body）
  - BuildFastWithAI（7月17日、7月14日 AI News Today 日报，辅助核实信号）
  - Distill Intelligence（7月17日 AI Leaders Weekly Briefing）
  - llm-stats.com / kie.ai（Kimi K3 基准测试和定价确认）
  - awesomeagents.ai（K3 Swarm Max agent orchestration 用途说明）
  - MacRumors / 9to5Mac / AppleInsider（7月17日，Apple vs. OpenAI 法律升级——40名前员工收到保存信）
  - CNBC / Fortune / Axios（7月14日，IBM 股价暴跌25%——AI 资本支出转移信号）
  - whitehouse.gov / The Record / CNN（7月14日，White House Gold Eagle AI 网络安全漏洞清算所）
  - BuildFastWithAI（7月14日，PrismML Bonsai 27B on iPhone 17 Pro）
  - Anthropic.com / MIT Technology Review（6月30日，Claude Science 发布——超出7天窗口，排除）
  - GitHub Trending tools：OSSInsight、Trendshift（July 15–17 snapshot）
  - Pandaily（6月 Embodied AI model explosion——边界模糊，排除）
  - arXiv《Self-Evolving World Models for LLM Agent Planning》、《Qwen-AgentWorld》等（June/July world model 研究波，无具体7天内时效事件锚点，排除）

- **Total signals found**: 约25个信号评估

- **Why these 3**:
  - **Candidate 1（Kimi K3 K3 Swarm Max，7月16-17日）**：**Agent经济柱**——该柱上次入选7月17日（Nubia NaviX Ultra，角度：App生态封锁 Agent 访问权）；今日角度完全不同（大规模 Agent 并发的成本结构正在系统性降低）；K3 Swarm Max 专为数百并发子 Agent 设计，是 Agent 经济成本基础设施层的新事件；DeepSeek 闪回有市场价格数据支撑（Axios、Fortune 多源）；1-2天前，本次扫描最高时效性；中文媒体报「中国模型追上美国」，不会分析「Agent 并发成本曲线下移对 Agent 经济可行性门槛的影响」；**HIGH 优先级**。
  - **Candidate 2（Thinking Machines Inkling，7月15日）**：**AI产品战略柱**——该柱上次入选7月16日（唐杰内部信/中国AI出口限制，供应链主权风险）；今日角度完全不同（「主动不追最强 = 产品赌注，Tinker 定制化才是真产品」）；Murati 的身份（前 OpenAI CTO）赋予「主动放弃追最强」极强的信号权重；TechCrunch、Axios、Bloomberg 同日报道，信源可靠；3天前；中文媒体报「Murati 发布首款模型」，不会分析「开源基础模型作为分发工具、Tinker 定制化平台作为真正商业化路径」的战略逻辑；**HIGH 优先级**。
  - **Candidate 3（AI监管三巨头收敛，7月14-16日）**：**深层AI思考柱**——该柱最近入选7月16日（NY 数据中心禁令，AI治理的能源基础设施层）；今日角度完全不同（AI治理的制度层竞争：三家AI公司监管共识背后的护城河逻辑）；Axios 7月16日汇总报道是首次三人同时书面共识的记录；时机与同周 WAIC / WAICO 推进形成对读；中文媒体报「美国 AI 领袖支持监管」，不会分析「监管框架的隐藏功能是把当前市场结构固化为进入壁垒」；2-4天前；**HIGH 优先级**。
  - **排除信号**：IBM -25%（7月14日，4天前，强事件但AI产品战略/组织形式变革角度今日已被Inkling和调度占据，可留明日；Apple vs. OpenAI法律升级，7月17日，无清晰Zico主题柱契合点）；Claude Science（6月30日，超窗口）；PrismML Bonsai 27B（7月14日，边缘AI里程碑，但AI协作实践柱今日休息）；Gold Eagle White House（7月14日，与Zico五柱契合度偏低）；Embodied AI model explosion（无精确时效锚点）。
  - 三者覆盖三个不同主题柱（Agent经济 / AI产品战略 / 深层AI思考），时效性分别为1-2天 / 3天 / 2-4天，与过去3天已入选候选无重叠（Agent经济角度从访问权→成本结构；AI产品战略从中国AI供应链风险→美国AI定制化平台策略；深层AI思考从能源基础设施层监管→制度竞争护城河逻辑）。
