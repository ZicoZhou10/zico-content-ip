---
date: 2026-07-05
status: pending_selection
---

# Today's Candidates

## Candidate 1: 美团 LongCat-2.0 揭开"Owl Alpha"面纱——在 OpenRouter 匿名拿了两个月第一，1.6T 参数用国产芯片从头练完（June 30）

- **Event**: 2026年6月30日，**美团**（Meituan）旗下 LongCat AI 实验室在 GitHub、Hugging Face 和官方平台正式开源 **LongCat-2.0**——同时揭开了一个持续两个月的秘密：这就是在 OpenRouter 上以匿名身份"**Owl Alpha**"运行的那个模型。在被揭开前，Owl Alpha 已在 OpenRouter 达成：**Hermes Agent Workspace 调用量排名第一、Claude Code 工作流排名第二、OpenClaw 部署量排名第三**，单日峰值 **559 亿 token**，两个月累计约 **10.1 万亿 token**（月均同比增长 242%）。技术规格：1.6 万亿参数 MoE 架构，每 token 平均激活 480 亿参数（动态在 330-560 亿之间），原生 **100 万 token 上下文**，MIT 开源许可。训练基础设施：**5 万张国产 ASIC**（非 NVIDIA）完成从预训练到推理的全流程，预训练数据量超 **35 万亿 token**，无回滚或不可恢复的 loss spike。性能：**SWE-bench Pro 59.5**（超过 GPT-5.5 的 58.6、Gemini 3.1 Pro 的 54.2，低于 Claude Opus 4.7 和 4.8）。定价：正常 API **$0.75/M input、$2.95/M output**，发布期促销价 **$0.30/M input、$1.20/M output**，缓存 context 读取免费。另有一个细节：Justin Sun 的 B.AI 平台在封禁期间一直作为 LongCat-2.0 的中转访问入口之一，覆盖部分被 Anthropic 封锁的用户。来源：**VentureBeat**（2026年6月30日，《Meituan open sources LongCat-2.0, the 1.6T, near-frontier agentic coding model that's been leading OpenRouter — trained entirely on Chinese chips》）、**Decrypt**（2026年6月30日，《LongCat-2.0: The Stealth AI Model That Was Quietly Topping OpenRouter All Along》）、**KuCoin**（《Owl Alpha on OpenRouter Revealed as Meituan's LongCat-2.0-Preview with 11T Monthly Token Throughput》）、**SiliconANGLE**（2026年6月30日，《China's Meituan open-sources massive LongCat-2.0 AI model, saying it was trained on domestic chips》）、**CryptoBriefing**（《Meituan reveals LongCat-2.0, undercuts GPT-5.5 and Claude Sonnet 5 on pricing》）、**Yahoo Tech**（《LongCat-2.0: The Stealth AI Model That Was Quietly Topping OpenRouter All Along》）。
- **Source**: https://venturebeat.com/technology/meituan-open-sources-longcat-2-0-the-1-6t-near-frontier-agentic-coding-model-thats-been-leading-openrouter-trained-entirely-on-chinese-chips | https://decrypt.co/372579/longcat-2-0-meituan-ai-stealth-model-openrouter | https://www.kucoin.com/news/flash/owl-alpha-on-openrouter-revealed-as-meituan-s-longcat-2-0-preview-with-11t-monthly-token-throughput | https://siliconangle.com/2026/06/30/chinas-meituan-open-sources-massive-longcat-2-0-ai-model-saying-trained-on-domestic-chips/ | https://cryptobriefing.com/meituan-longcat-2-undercuts-gpt-claude-pricing/
- **Timeliness**: 5 天前（2026年6月30日，开源发布 + Owl Alpha 揭幕）
- **Topic pillar**: Agent经济
- **Zico's angle**: 这件事最值得说的不是"美团做了大模型"，是**一个匿名模型在 OpenRouter 拿了两个月第一，背后是外卖公司**。

  Agent 工具市场的逻辑和消费者 AI 市场完全不同。消费者 AI 靠品牌认知驱动（用 ChatGPT 因为知道 OpenAI），Agent 工具市场靠调用结果驱动——开发者和企业选工具看的是：任务完成率、成本、上下文长度。Owl Alpha 在 Hermes Agent Workspace 拿了两个月第一，靠的不是"美团背书"，是因为它在实际 agentic 任务里比其他选项更好。被揭开身份后，月均调用量仍在增长，这说明开发者选择它是因为它有用，不是因为它有名字。

  这对 Agent 经济的产品策略有一个直接的含义：**匿名竞争是 Agent 市场的合法策略**。在消费者 AI 里，你不敢匿名——用户付费需要信任品牌。在 Agent API 市场里，你可以匿名两个月拿第一，因为唯一的信任信号是"这个 API 在我的工作流里有没有输出正确结果"。这也解释了为什么 LongCat 选择匿名入场而不是直接官宣——先用结果建立占有率，再用身份加固它。

  还有一层：**5 万张国产 ASIC，35 万亿 token 预训练，从头到尾不用 NVIDIA**。这不是概念验证，是一个在 SWE-bench Pro 59.5 处于可量化生产水准的系统。DeepSeek V4 Pro 推理用国产芯片，但训练仍然依赖 NVIDIA——LongCat-2.0 是目前公开披露的第一个**训练和推理全流程**用国产算力完成、且有第三方可验证性能（OpenRouter 真实调用量）的万亿参数模型。

  中文媒体会报"美团 AI 模型开源，全国产芯片"，不会分析：**这是 Agent API 市场里"用结果建立占有率"策略的一个完整案例——以及为什么外卖公司的 AI lab 能在编程 Agent 赛道悄悄拿第一。**

- **Resonance hook**: 2026年6月30日，美团开源了 LongCat-2.0，同时揭开了一个秘密：过去两个月在 OpenRouter 拿第一的匿名模型 Owl Alpha，就是它。Hermes Agent Workspace 调用量第一，Claude Code 工作流排名第二，日均 559 亿 token，全程没有人知道背后是谁。SWE-bench Pro 59.5，超过 GPT-5.5。5 万张国产 ASIC，35 万亿 token，不用 NVIDIA，从头到尾。发布促销价 $0.30/M input。外卖公司的模型，悄悄拿了 Agent 编程赛道两个月的第一。
- **Recommended priority**: high

---

## Candidate 2: 法院文件披露：向 Anthropic 施压要求接受自主武器的五角大楼官员，同期持有 Perplexity 和 xAI 数百万美元股票（July 2）

- **Event**: 2026年7月2日，美国加州北区联邦法院公开解封一批**内部往来邮件**，揭示了 Anthropic 与美国国防部谈判破裂的完整过程。核心发现：**国防部副部长（研究与工程）Emil Michael**——谈判中最强硬地要求 Anthropic 去除 AI 安全护栏的那位官员——在施压期间同时持有：① **Perplexity AI 股票价值 200-1000 万美元**（Anthropic 直接竞争对手）；② **xAI（马斯克旗下）股票 50-100 万美元**，并于 2026年1月9日以 **500-2500 万美元出售**。争议核心：国防部要求 Anthropic 允许两种用途——**全自主武器系统**（无人类决策节点）和**国内监控项目**。Anthropic CEO **Dario Amodei** 的立场始终未变：这两类应用不在合作范围之内，其他"所有合法用途"均可接受。国防部的反要求是"**all lawful uses**"——用法律用语包住了 Amodei 明确拒绝的两个类别。2026年1月，Michael 发邮件给 Amodei，暗示对方有"**最后一次机会对齐核心原则**"，Amodei 重申了同样的两条底线，谈判宣告破裂。此后国防部将 Anthropic 列入"供应链风险"名单，Anthropic 提起诉讼，法院于4月8日拒绝临时阻止 DoD 对 Anthropic 的黑名单措施。Anthropic 官方博客发布声明《Where things stand with the Department of War》。来源：**TechTimes**（2026年7月4日，《Pentagon Blacklisted Anthropic Over Autonomous Weapons Limits: Emails Reveal "Very Close" Talks》）、**TechCrunch**（2026年3月20日首发，《New court filing reveals Pentagon told Anthropic the two sides were nearly aligned — a week after Trump declared the relationship kaput》）、**The Next Web**（《Anthropic–Pentagon emails reveal the real fight》）、**CNBC**（2026年4月8日，《Anthropic loses appeals court bid to temporarily block Pentagon blacklisting》）、**Anthropic 官方博客**（《Where things stand with the Department of War》）、**Congress.gov CRS 报告**（《Pentagon-Anthropic Dispute over Autonomous Weapon Systems: Potential Issues for Congress》）、**EFF**（《The Anthropic-DOD Conflict》）。
- **Source**: https://www.techtimes.com/articles/319713/20260704/pentagon-blacklisted-anthropic-over-autonomous-weapons-limits-emails-reveal-very-close-talks.htm | https://techcrunch.com/2026/03/20/new-court-filing-reveals-pentagon-told-anthropic-the-two-sides-were-nearly-aligned-a-week-after-trump-declared-the-relationship-kaput/ | https://thenextweb.com/news/anthropic-pentagon-emails-amodei-michael-guardrails | https://www.cnbc.com/2026/04/08/anthropic-pentagon-court-ruling-supply-chain-risk.html | https://www.anthropic.com/news/where-stand-department-war | https://www.congress.gov/crs-product/IN12669
- **Timeliness**: 3 天前（2026年7月2日，法院文件公开解封）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: 这件事的核心不是 Anthropic 对抗五角大楼，是**一个在谈判桌对面持有竞争对手股票的政府官员，试图通过监管权力去除 AI 安全护栏**。

  先把利益冲突的结构说清楚：Emil Michael 是美国国防部负责研究与工程的副部长，在政府职责上是"代表国家评估 AI 军事能力和供应链安全"的官员。但他同时持有 Perplexity AI（Anthropic 的直接竞争对手，相同目标客户、相同价格带）价值数百万美元的股票，以及 xAI（马斯克旗下，另一家 Anthropic 竞争对手）的股票，并在谈判期间以 500-2500 万美元变现了后者。

  这不是道德问题，是结构性问题：**当负责"AI 供应链安全评估"的官员同时是 AI 公司竞争对手的股东，他所谓的"国家安全判断"无法被区分于"竞争利益判断"**。他把 Anthropic 列入供应链风险名单，加速了 Anthropic 失去政府合同的进程；这对他持有股票的竞争对手是直接利好。无论他的主观动机是什么，这个结构本身就是问题。

  然后是 AI 安全护栏作为"价值主张"的现实测试：Amodei 拒绝的两条——全自主武器和国内监控——是 Anthropic 公开的安全承诺的核心部分。他在谈判中没有动摇。结果是：Anthropic 因为坚持安全立场，被政府列入"供应链风险"并失去了一部分政府合同。**AI 安全价值观在接触国家权力时，代价是真实的：你会失去合同，你会被从采购名单上移除。** 这不是理论风险，是已经发生的事情。

  对"AI 公司应该如何定位安全立场"这个问题，这件事提供了一个真实的数据点：选择坚守安全边界，会在特定场景下付出商业代价，但也可能是唯一能让公司长期存活的选项——如果你的客户群（企业和开发者）把你的安全立场视为信任基础而非营销话术的话。

  中文媒体会报"Anthropic 拒绝和美国军方合作"，不会分析：**最强硬地要求 Anthropic 去除安全护栏的那位官员，同期是 Anthropic 竞争对手的股东——监管权力和竞争利益在同一个人身上重叠，这才是这件事真正的问题所在。**

- **Resonance hook**: 7月2日，法院文件解封：向 Anthropic 施压、要求允许全自主武器系统的五角大楼官员 Emil Michael，在谈判期间持有 Perplexity AI 数百万美元股票，并以 500-2500 万美元变现了 xAI 股票。Perplexity 和 xAI 都是 Anthropic 的直接竞争对手。一个"代表国家评估 AI 供应链安全"的人，同时是这家 AI 公司竞争对手的股东。Amodei 拒绝了，Anthropic 被列入供应链风险名单，失去了政府合同。AI 安全立场的代价，第一次以这么具体的方式被量化了。
- **Recommended priority**: high

---

## Candidate 3: xAI 用 SpaceX 价值 600 亿美元收购的 Cursor 数据训练 Grok 4.5，马斯克的封闭 AI 飞轮第一次完整成型（June 28）

- **Event**: 2026年6月28日，**Elon Musk** 在 X 上宣布：xAI 最新模型 **Grok 4.5** 已进入在 **SpaceX 和 Tesla** 的私有 Beta 测试。核心参数：基于 V9 基础模型，**1.5 万亿参数**（约为现有 Grok 生产版本 v8-small 的3倍），在补充训练（post-pretraining supplemental training）阶段加入了 **Cursor**（Anysphere）的开发者工作流数据。Musk 的性能声明：接近甚至可能超越 Anthropic Claude Opus——但无独立基准测试，无 system card，无第三方验证。私有 Beta 策略：**仅限 SpaceX 和 Tesla 内部**，不对外开放，无公开访问渠道。发布节奏承诺：**2026年底前每月发布一个全新从头训练的基础模型**（非 fine-tune，是完整重新训练）。背景关键事实：**SpaceX 于2026年6月签署协议以 600 亿美元全股票收购 Anysphere（Cursor 母公司）**，预计 Q3 完成交割——届时 xAI 将获得 Cursor 超过**100 万活跃开发者用户**的编程行为数据，以及 Cursor 的全部开发者工作流语料。Grok 4.5 的 V9 基础模型于2026年5月26日完成训练。来源：**TechTimes**（2026年6月29日，《Grok 4.5 Enters Private Beta at SpaceX and Tesla: No Public Access, No Independent Benchmark》）、**FreePressJournal**（《Grok 4.5 Enters Private Beta At SpaceX & Tesla As xAI Signals Faster AI Rollout Cycle With 1.5T Model》）、**DigitalApplied**（《Grok 4.5: SpaceX's 1.5T V9 Model Trained on Cursor》、《SpaceX Buys Cursor for $60B: What the Deal Means in 2026》）、**TradingKey**（《Grok 4.5 Undergoing Internal Testing at SpaceX and Tesla, Musk Says Performance May Exceed Claude Opus》）、**BigGo Finance**（《Musk's AI Blitz: Grok 4.5 Performance Matches Opus, Plans to Launch a Brand-New Model Every Month Through Year-End》）。
- **Source**: https://www.techtimes.com/articles/319314/20260629/grok-45-enters-private-beta-spacex-tesla-no-public-access-no-independent-benchmark.htm | https://www.freepressjournal.in/tech/grok-45-enters-private-beta-at-spacex-tesla-as-xai-signals-faster-ai-rollout-cycle-with-15t-model | https://www.digitalapplied.com/blog/grok-4-5-cursor-data-flywheel-spacex-private-beta-2026 | https://www.digitalapplied.com/blog/spacex-acquires-cursor-anysphere-60b-ai-coding-2026
- **Timeliness**: 7 天前（2026年6月28日，Musk X 公告）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 这件事真正重要的不是 Grok 4.5 有多强——Musk 的性能声明没有独立验证，暂时不能当真。真正值得分析的是**马斯克现在拥有的那个结构**。

  把几件事放在一起看：xAI（AI 模型）、SpaceX/Tesla（第一批企业客户）、X（社交媒体用户数据）、Cursor（100万+活跃开发者的编程工作流数据，600亿美元收购）。这四个资产组合在一起，创造了一个其他 AI 实验室无法复制的闭合飞轮：**SpaceX 和 Tesla 的工程师使用 Cursor 写代码 → 编程行为数据进入 Grok 训练语料 → Grok 变得更懂工程场景 → SpaceX/Tesla 工程效率提升 → 产生更多、更专业化的编程数据 → 循环**。

  这个飞轮的关键特性是：**每一次"销售"同时是一次数据采集**。传统 AI 实验室的商业模式是：训练模型→销售 API 访问→用收入继续训练。Musk 的结构是：训练模型→在自己的企业里部署→企业员工的使用行为成为下一轮训练数据。"客户"和"数据来源"是同一群人。更重要的是，SpaceX 和 Tesla 的工程场景（火箭、电动车、自动驾驶）具有极高的专业性和稀缺性——这类数据不是通过开放 API 能采集到的，必须在真实的、高难度的工程环境里生成。

  "每月从头训练一个全新基础模型"这个承诺，也是一个组织宣言：**xAI 把训练基础设施当成制造流水线，不是研究实验室**。传统 AI 实验室每次大规模训练都是 18 个月以上的项目，充满不确定性。每月重训意味着 xAI 已经把这个过程工业化了——或者在押注这件事可以工业化。

  对理解"哪种 AI 公司结构有持久竞争力"的人：**垂直整合数据飞轮 vs 开放 API 市场竞争，是现在 AI 行业两种截然不同的组织逻辑**。Musk 的赌注是前者——你不需要外部用户，你需要高质量的自有场景数据。这个结构的弱点是：封闭数据的多样性不如开放市场，如果 Grok 主要被 SpaceX/Tesla 使用，它在其他场景的泛化能力可能受限。

  中文媒体会报"马斯克 Grok 4.5 上了，声称超过 Claude Opus"，不会分析：**600 亿美元收购 Cursor 建立的是一个数据飞轮，不只是一个产品——SpaceX/Tesla 既是 Grok 的第一批用户，也是训练数据的来源，Musk 在用企业帝国结构替代开放市场竞争。**

- **Resonance hook**: 6月28日，马斯克宣布 Grok 4.5 私测——只在 SpaceX 和 Tesla 内部，1.5T 参数，用 Cursor 编程数据训练，性能声称接近 Claude Opus，无独立验证。同期背景：SpaceX 以 600 亿美元收购 Cursor，预计 Q3 交割。承诺：2026年底前每月从头训练一个全新模型。这不是模型发布新闻，是一个组织结构声明：Musk 现在同时拥有模型（xAI）、主要用户（SpaceX/Tesla）、训练数据来源（Cursor 的 100 万开发者行为数据）。其他 AI 实验室有的是算力竞争，他有的是闭合飞轮。
- **Recommended priority**: high

---

## Scan summary

**Sources scanned**:
- BuildFastWithAI（2026年7月4日，《AI News Today July 4 2026: 15 Biggest Stories》）
- VentureBeat（2026年6月30日，《Meituan open sources LongCat-2.0, the 1.6T, near-frontier agentic coding model that's been leading OpenRouter — trained entirely on Chinese chips》）
- Decrypt（2026年6月30日，《LongCat-2.0: The Stealth AI Model That Was Quietly Topping OpenRouter All Along》）
- KuCoin（《Owl Alpha on OpenRouter Revealed as Meituan's LongCat-2.0-Preview with 11T Monthly Token Throughput》）
- SiliconANGLE（2026年6月30日，Meituan LongCat-2.0 国产芯片报道）
- CryptoBriefing（《Meituan reveals LongCat-2.0, undercuts GPT-5.5 and Claude Sonnet 5 on pricing》）
- Yahoo Tech（《LongCat-2.0: The Stealth AI Model That Was Quietly Topping OpenRouter All Along》）
- GeoPolitechs（《LongCat-2.0: China's Most Unexpected AI Model》）
- TechTimes（2026年7月4日，《Pentagon Blacklisted Anthropic Over Autonomous Weapons Limits: Emails Reveal "Very Close" Talks》）
- TechCrunch（2026年3月20日首发，《New court filing reveals Pentagon told Anthropic the two sides were nearly aligned》）
- The Next Web（《Anthropic–Pentagon emails reveal the real fight》）
- CNBC（2026年4月8日，《Anthropic loses appeals court bid to temporarily block Pentagon blacklisting》）
- Anthropic 官方博客（《Where things stand with the Department of War》）
- Congress.gov（CRS 产品报告，Pentagon-Anthropic Dispute）
- EFF（《The Anthropic-DOD Conflict》）
- TechTimes（2026年6月29日，《Grok 4.5 Enters Private Beta at SpaceX and Tesla》）
- FreePressJournal（《Grok 4.5 Enters Private Beta At SpaceX & Tesla》）
- DigitalApplied（《Grok 4.5: SpaceX's 1.5T V9 Model Trained on Cursor》、《SpaceX Buys Cursor for $60B: What the Deal Means in 2026》）
- BanklessTimes（2026年7月3日，《Anthropic Moves to Block Chinese Firms Using Claude via Offshore Workarounds》）
- Investing.com（2026年7月3日，FT 报道转摘，Anthropic 新加坡漏洞封堵）
- Benzinga（2026年7月3日，《Meta's Upcoming 'Watermelon' AI Model Matches OpenAI's GPT-5.5 on Key Benchmarks》）
- TechTimes（2026年7月4日，《Meta Watermelon AI Claims GPT-5.5 Benchmark Catch-Up: Benchmarks Remain Unnamed and Unverified》）
- BusinessStandard（2026年6月26日，White House + GPT-5.6 限制发布）
- TechCrunch（2026年6月26日，《OpenAI limits GPT-5.6 rollout after government request》）
- ResultSense（2026年7月2日，《US nears voluntary standards for AI model releases》）
- X/Twitter: Karpathy @karpathy（Sequoia Ascent 2026 fireside chat 博客帖，约 April 30 发布，超出最优窗口，排除）
- llm-stats.com（《AI Updates Today July 2026》）
- LongCatAI 官方（longcatai.org/models/longcat-2）

**Total signals found**: 约 28 个信号评估

**Why these 3**:

- **Candidate 1（Meituan LongCat-2.0 / Owl Alpha，6月30日）**：**Agent经济柱**——此柱距上次覆盖（7月2日，Claude Sonnet 5 agentic 基线化）已3天；Owl Alpha 匿名拿 OpenRouter 两个月第一的叙事结构是本周最强的"发现式"钩子（读者可自行去 OpenRouter 验证调用量数据）；559亿 token/天的真实使用量比任何自我声明的性能基准更有说服力；"外卖公司的模型悄悄拿了 Agent 编程赛道第一"这一反常识事实在中文 AI 圈几乎零分析（中文报道停在"美团又搞 AI 了"）；国产全流程训练（5万张 ASIC，无 NVIDIA）与 Fable 5 出口管制（7月2日 063 已选）形成叙事镜像——美国在管控 AI 出口，中国在用国产芯片绕过依赖；定价（$0.30/M input 促销）的信息增量直接影响读者当下的工具选择；**HIGH 优先级**。

- **Candidate 2（五角大楼邮件：Emil Michael 持竞争对手股票施压 Anthropic，7月2日解封）**：**深层AI思考柱**——此柱昨日（7月4日）被 Altman IAEA/5%股权方案占据（治理架构），今日角度完全不同（监管利益冲突 + AI 安全护栏的真实代价）；法院文件7月2日解封，TechTimes 7月4日跟进报道，时效3天；"负责 AI 供应链安全的官员同时持有竞争对手股票"这一利益冲突在中文媒体完全缺失——中文报道停在"Anthropic 不给美军做自主武器"，完全没有分析 Emil Michael 的股权背景；"AI 安全立场代价第一次被具体量化（失去政府合同）"这一角度在中文 AI 思考圈也几乎缺席；此候选与7月4日 Candidate 1（Altman IAEA）构成完整叙事对仗：Altman 主动入局政府治理框架，Anthropic 被动对抗政府权力——两个截然不同的生存策略；**HIGH 优先级**。

- **Candidate 3（Grok 4.5 + SpaceX Cursor $600亿飞轮，6月28日）**：**组织形式变革柱**——此柱上次覆盖为7月3日（Newsom+Anthropic，2天前）；Grok 4.5 本身（无独立基准）信息质量有限，但"600亿美元收购 Cursor 建立封闭训练飞轮"这个组织结构分析在中文媒体完全缺失（中文报道停在"Grok 又升级了/马斯克又吹了"）；SpaceX/Tesla 作为第一批"既是用户也是训练数据来源"的企业客户这一结构创新，是"组织形式变革柱"的典型素材——这不是一家 AI 公司，是把 AI 嵌入帝国结构的组织实验；"每月从头训练一个新基础模型"的工业化训练承诺，本身就是一个值得分析的组织能力主张；时效为7天前（最优窗口边缘，但组织结构分析类内容有更长的有效期）；**HIGH 优先级**（时效略弱，但信息增量和柱空白补偿）。
