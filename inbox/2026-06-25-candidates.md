---
date: 2026-06-25
status: pending_selection
---

# Today's Candidates

## Candidate 1: Anthropic 发布 40 万次真实会话研究——「域知识」（非编程能力）才是 AI 协作效率的决定因素（June 16 发布 / June 23 TechTimes 深度报道）

- **Event**: 2026年6月16日，Anthropic 在官方研究页面发布论文《Agentic Coding and Persistent Returns to Expertise》，作者 Zoe Hitzig、Maxim Massenkoff 等五位研究人员，基于 **2025年10月至2026年4月 约40万次 Claude Code 真实会话、约23.5万用户**的隐私保护分析。核心发现：**① 域知识深度（而非编程背景）是预测 AI Coding Agent 使用效果的首要因素**；② 在典型会话中，人类负责大部分规划决策（「做什么」），Claude 负责大部分执行决策（「怎么做」）；③ **域知识越深，每条人类指令让 Claude 完成的工作量就越多**——即高域知识用户的单次指令杠杆率系统性更高；④ 没有编程背景的域专家（如生物学家、律师、产品经理）可以在编程任务上取得与有编程背景的普通用户相当甚至更好的效果，因为他们能更精确地评估输出是否正确。2026年6月23日，**TechTimes** 以「AI Coding Agents Reward Domain Expertise, Not Coding Skill: Anthropic Study of 400K Sessions」为题专题报道，成为该研究覆盖量最高的二次报道。
- **Source**: https://www.anthropic.com/research/claude-code-expertise | https://www.techtimes.com/articles/318955/20260623/ai-coding-agents-reward-domain-expertise-not-coding-skill-anthropic-study-400k-sessions.htm | https://www.explainx.ai/blog/anthropic-claude-code-expertise-research-agentic-coding-2026 | https://pathmode.io/blog/orchestration-era-needs-intent
- **Timeliness**: 2 天前二次深度报道（TechTimes，2026年6月23日）；原论文发布 9 天前（Anthropic 官方，2026年6月16日）
- **Topic pillar**: AI协作实践
- **Zico's angle**: 「AI 让所有人都能编程」这个叙事从来就不准确。40万次真实会话告诉我们的是：**AI 让域知识可以直接转化为执行能力——跳过了以前必须经过的技能瓶颈（写代码/做设计/写合同）。**

  这个发现有一个具体的推论：如果你深度理解一个问题，你能识别 AI 输出的对错；如果你不深度理解，AI 给你再多代码你也无法判断它是否正确。一个不懂蛋白质折叠的程序员用 Claude 写 AlphaFold 类的代码，产出不会比懂蛋白质折叠但不会编程的生物学家更好——因为后者能看出 AI 输出的错误在哪，前者不能。

  这和 Karpathy 说的「AI 是新物种」有一个联动：Agent 最终是否产出价值，取决于人类那一端能不能提供「正确性的锚」。域知识就是这个锚。没有锚的人不是被 Agent 增强了，是被 Agent 随机化了——输出看起来有模有样，但对不对只有真正懂的人才能判断。

  对做 AI 产品的人：产品策略、用户行为理解、空间智能应用判断——这些域知识在 Agent 协作中比「会用 prompt」更值钱。这个研究是第一个用真实数据验证了这一点的东西。对于那些在犹豫「我该不该学编程来适应 AI 时代」的人，数据给了不同的答案：**先把你已经在做的领域学深，比学一个新技能更有用。**

  中文职场社区对「AI 时代需要什么技能」有极高关注度，但讨论大多停在「要学提示词工程」层面。这个研究直接挑战这个假设，且有 40 万条真实数据背书。

- **Resonance hook**: 6月16日，Anthropic 公布了一份 40 万次 Claude Code 真实会话的研究：决定你用 AI 效率高低的，不是你会不会编程，是你对自己工作领域懂得有多深。域知识越深，Claude 每条指令干的活就越多。不会编程但深懂领域的人，效果和普通程序员差不多——因为他们知道怎么判断输出对不对。AI 不是让人人都能编程，是让深度领域知识直接变成执行能力。
- **Recommended priority**: high

---

## Candidate 2: Reflection AI 与 SpaceX 签 $63 亿算力合同——AlphaGo 工程师 + Gemini RLHF 负责人离开 DeepMind，NVIDIA 押注造开源超级智能（June 22）

- **Event**: 2026年6月22日，**SpaceX** 与 **Reflection AI** 签署算力租赁协议：Reflection AI 从 **2026年7月1日**起，每月向 SpaceX 支付 **$1.5 亿**，使用 **Colossus 2**（田纳西州孟菲斯数据中心）的 **NVIDIA GB300 芯片**，合同周期至 **2029年底**，双方可在前三个月后以 90 天通知提前终止，总合同金额若跑满为 **$63 亿**（CNBC 首发，Data Center Dynamics 确认）。这是 SpaceX 商业算力业务第四个大客户（已有 Anthropic $450 亿合同、Google $300 亿合同、Cursor 金额未披露）。Reflection AI 由两位前 Google DeepMind 核心研究者联合创立：① **Ioannis Antonoglou**（DeepMind 创始工程师，AlphaGo 关键贡献者，后担任 Gemini 后训练负责人）；② **Misha Laskin**（Gemini RLHF 奖励模型负责人，UC Berkeley 博士后）。公司使命：构建**开源超级智能（open-source superintelligence）**，即前沿级别、权重完全公开、可任意下载运行的模型，直接对标 Meta Llama 但规模更大、研究更深。当前估值 **$250 亿**（2026年3月），**NVIDIA 是主要投资方**。截至合同签署时，Reflection AI 尚未公开发布任何模型。
- **Source**: https://www.cnbc.com/2026/06/22/spacex-ai-colossus-data-center-reflection.html | https://www.datacenterdynamics.com/en/news/spacex-secures-63bn-compute-capacity-deal-from-ai-startup-reflection/ | https://www.fool.com/investing/2026/06/23/spacex-just-inked-a-new-ai-deal-worth-up-to-63-billion/ | https://sequoiacap.com/article/reflection-ai-spotlight/
- **Timeliness**: 3 天前（CNBC 2026年6月22日首发；Motley Fool 2026年6月23日跟进）
- **Topic pillar**: Agent经济
- **Zico's angle**: Reflection AI 做了一件结构上不寻常的事：**在没有发布任何模型的情况下，用 $250 亿估值、NVIDIA 背书，锁定了 $63 亿算力合同。** 这不是一家产品公司在扩张，是一家 bet 正在下、结果尚未揭晓的公司在提前抢占计算资源。

  NVIDIA 投资 Reflection AI 的逻辑有战略含义：NVIDIA 卖芯片，开源模型会扩大全球部署量（任何公司都能下载运行 → 都需要 GPU），而闭源模型会把算力需求集中在少数超大 hyperscaler 手里。NVIDIA 押注 Reflection AI，不只是财务回报，是**「开源前沿模型扩大整体芯片市场」的生态系统押注**——比起 OpenAI 或 Anthropic，开源模型对 NVIDIA 的市场扩展价值更大。

  把这个故事放在 6 月 12 日 Fable 5 出口管制事件之后，有了新的语境：美国政府用 90 分钟关停了 Anthropic 的闭源旗舰模型，理由是「防止外国国籍人员访问」。但一个在 Hugging Face 上已经下载了数百万次的开源模型，没有任何政府能在 90 分钟内关停它。Reflection AI 押注的不只是「开源更好」，而是**「可以被下载的模型是一种不依赖任何单一主权的基础设施形态」**。这是 Fable 5 出口管制的市场层回应。

  DeepMind 人才流失的第三条叙事线：Shazeer（Transformer）→ OpenAI，Jumper（AlphaFold/Nobel）→ Anthropic，Antonoglou + Laskin（AlphaGo + Gemini RLHF）→ Reflection AI 自立创业。四个定义了过去 10 年 AI 最重要工作的人，无一留在 Google。

- **Resonance hook**: 6月22日，CNBC：Reflection AI（$250亿估值，NVIDIA 投资）与 SpaceX 签 $63 亿算力合同，从7月起每月付 $1.5 亿租 Colossus 2 的 NVIDIA GB300 芯片。创始人：AlphaGo 创始工程师 Ioannis Antonoglou + Gemini RLHF 负责人 Misha Laskin，两人均来自 Google DeepMind。目标：开源超级智能——权重完全公开，任何人可下载运行。目前尚未发布任何模型，但已是 SpaceX 算力的第四大商业客户，仅次于 Anthropic（$450亿）和 Google（$300亿）。政府关停闭源模型的那个月，他们在烧 $1.5 亿/月做不能被关停的模型。
- **Recommended priority**: high

---

## Candidate 3: Google Gemini 3.5 Pro 延期至 7 月——CEO 在 I/O 面向数千开发者承诺 6 月 GA，模型团队「对当前性能不满意」（June 23）

- **Event**: 2026年6月23日，**Business Insider** 独家报道（经 Investing.com Insider 同步）：**Google DeepMind 已取消 Gemini 3.5 Pro 的 6 月底发布计划**，内部团队**「对当前模型性能不满意（dissatisfied with current performance）」**，正在收集早期测试者反馈并做调整，正式 GA 推迟至 **2026年7月**。背景：**Google CEO Sundar Pichai** 在 2026年5月19日 **Google I/O 开发者大会**上公开宣布 Gemini 3.5 Pro 将 **6 月内 GA**——面向数千名开发者的明确承诺，现场报道称延期消息传出时开发者「发出明显叹息（audible groan）」。同期信号：**GPT-5.6** 在同一周被 Polymarket 预测市场降价，6月22-28发布概率从高峰 **83% 跌至 18%**，市场新共识指向 **7月底**（94% 概率）。两款前沿旗舰同周滑入 Q3。Gemini 3.5 Pro 已确认规格：**200 万 token 上下文窗口**（是 Flash 的两倍）、**Deep Think 推理模式**、多模态升级。CryptoBriefing（6月23日）、TipRanks（6月24日）多方跟进确认。
- **Source**: https://cryptobriefing.com/google-delays-gemini-35-pro-launch-to-july-2026/ | https://www.investing.com/news/stock-market-news/google-delays-gemini-35-pro-model-release-to-july--insider-93CH-4758816 | https://www.tipranks.com/news/alphabet-googl-delays-release-of-gemini-3-5-pro-ai-model | https://finance.yahoo.com/technology/ai/articles/traders-abandon-bets-gpt-5-093100441.html
- **Timeliness**: 2 天前（Business Insider 独家 2026年6月23日；CryptoBriefing / TipRanks 跟进 2026年6月23-24日）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 「对当前性能不满意」这六个字是这次延期最有信息量的部分。

  做模型发布不是做软件发布。传统软件可以「先发 v1，快速迭代」；AI 旗舰模型发布没有这个选项——因为每个版本一发布，benchmark 数字就全部公开，竞争对手、媒体、开发者在 48 小时内会出完整对比报告。如果 Gemini 3.5 Pro 在关键 benchmark 上比 GPT-5.5 低 3 个百分点，这 3 个百分点会被截图传播数月。**发布一个「不够好」的旗舰模型，比不发布的代价更大。** 这是 AI 产品 PM 面临的，传统软件 PM 从来没遇到过的结构性约束。

  这创造了一个具体的悖论：你在 I/O 上承诺时间线（面向开发者，公开可信度赌注），但你无法控制模型在内部测试中的实际表现。Sundar Pichai 的「6 月 GA」承诺，在他说出来的时候，基于的是一个「训练进度可以预测」的假设——但大模型训练的最后几个百分点往往是最难预测的。

  GPT-5.6 同周也滑期这一点让分析更有力：这不只是 Google 的执行问题，是**前沿模型训练时间线比任何产品路线图都更难预测**这一系统性现实的两个数据点同时出现。对于在闭源前沿模型之上构建产品的公司：**「供应商旗舰模型比承诺晚 4-8 周」应该是默认预算，不是意外情况。** 这是技术供应链风险，不是商务谈判可以规避的。

- **Resonance hook**: 6月23日，Business Insider 独家：Google 取消 Gemini 3.5 Pro 的 6 月发布计划，理由是「对当前性能不满意」。5月19日，Sundar Pichai 在 Google I/O 面向数千名开发者承诺了 6 月 GA，据报道延期消息传出时现场发出明显叹声。同一周，GPT-5.6 的 Polymarket 发布概率从 83% 跌至 18%。两款前沿旗舰同周滑入 7 月。不是技术失败，是 AI 产品 PM 独有的悖论：在开发者大会上承诺时间线，和大模型训练最后几个百分点的不可预测性，这两件事无法同时成真。
- **Recommended priority**: medium-high

---

## Scan summary
- **Sources scanned**:
  - Anthropic 官方研究（《Agentic coding and persistent returns to expertise》，2026年6月16日）
  - TechTimes（《AI Coding Agents Reward Domain Expertise, Not Coding Skill: Anthropic Study of 400K Sessions》，2026年6月23日）
  - ExplainX.ai（《Anthropic Research: Domain Expertise Beats Coding Background in Agentic Programming》）
  - Pathmode.io（《2026 Agentic Coding Trends Report: Summary & Key Findings》）
  - DigitalApplied.com（《You Don't Need to Code to Ship With AI, Says the Data》）
  - CNBC（《SpaceX signs computing power deal with open-source AI startup Reflection worth up to $6.3 billion》，2026年6月22日）
  - Data Center Dynamics（《SpaceX secures $6.3bn compute capacity deal from AI startup Reflection》，2026年6月22日）
  - The Motley Fool（《SpaceX Just Inked a New AI Deal Worth Up to $6.3 Billion》，2026年6月23日）
  - Sequoia Capital（《Reflection AI: The Race to Unlock Superintelligence》）
  - Turing Post（《Inside Reflection AI: The $20B Open-Model Startup That Has Yet to Ship》）
  - CryptoBriefing（《Google delays Gemini 3.5 Pro launch to July 2026》，2026年6月23日）
  - Investing.com Insider（《Google delays Gemini 3.5 Pro model release to July》，2026年6月23日）
  - TipRanks（《Alphabet (GOOGL) Delays Release of Gemini 3.5 Pro AI Model》，2026年6月24日）
  - Yahoo Finance / Polymarket（《Traders abandon bets on a GPT-5.6 launch this week》）
  - BuildFastWithAI（《AI News Today June 24, 2026: 15 Biggest Stories》）
  - BuildFastWithAI（《AI News Today June 23, 2026: 15 Biggest Stories》）
  - Crescendo.ai（《Latest AI News and Breakthroughs That Matter Most》）
  - LLM-stats.com（June 2026 LLM更新全局扫描）
  - Gartner（《Gartner Forecasts Worldwide AI Spending to Grow 47% in 2026》，2026年5月19日——5周前，排除）
  - White House NSPM-11（《AI in the National Security Enterprise》，2026年6月5日——20天前，排除）
  - TechCrunch（《ChatGPT's market share slips below 50% for first time》，2026年6月16日——9天前，疑已被 June 17-20 选题文件覆盖，排除）
  - Latent.Space/swyx（June 2026 — 无独立时效事件锚点，排除）
  - arXiv June 2026 AI/agents/world models——无高传播性独立事件锚点，排除）
  - GitHub Trending OSSInsight June 2026——常青趋势，无独立时效事件，排除）
  - Karpathy blog《Sequoia Ascent 2026》——4-5月演讲录，非本周新事件，排除）

- **Total signals found**: 约 25 个信号评估

- **Why these 3**:
  - **Candidate 1（Anthropic 域知识研究，6月16/23日）**：AI协作实践柱过去3天完全未用（June 22/23/24均未选此柱）——今日首选；Anthropic官方原始数据（400K会话、235K用户）强度极高；TechTimes June 23二次报道提供时效锚点；「AI时代什么技能更有价值」在中文职场/AI社区是高持续共鸣话题，但「域知识比编程背景更重要」这一具体结论几乎未被中文媒体系统分析；直接映照Zico co-thinking 实践框架（Zico的产品/策略域知识就是驱动 Claude 输出质量的核心变量）；HIGH优先级
  - **Candidate 2（Reflection AI SpaceX $63亿，6月22日）**：Agent经济柱；CNBC + DCD + Motley Fool三方6月22-23日确认；AlphaGo+Gemini双核研究者联合创办、NVIDIA战略背书、$250亿估值的开源前沿实验室签下仅次于Anthropic和Google的SpaceX算力合同；「开源前沿实验室作为算力囤积+不可关停的主权AI替代方案」这一角度在中文AI媒体几乎无覆盖（会停在"另一家AI独角兽融资"层面）；与Fable 5出口管制（June 22 covered）的「可下载模型不可关停」叙事形成对话但角度完全独立；NVIDIA生态系统押注动机是可分析的战略层逻辑；HIGH优先级
  - **Candidate 3（Gemini 3.5 Pro延期，6月23日）**：AI产品战略柱（虽过去3天均用，今日角度独立——「AI产品PM特有的公开承诺 vs. 训练不可预测性」悖论分析）；Business Insider独家 + CryptoBriefing + TipRanks June 23-24确认；GPT-5.6同周也滑期（Polymarket 83%→18%）使这成为系统性信号而非单一公司失误；「前沿模型时间线作为产品供应链风险」这一实用框架在中文AI媒体缺席；与June 24 DeepMind人才流失叙事形成叙事延续但角度完全不同（「执行失败」vs「人才流失」是两个独立问题）；MEDIUM-HIGH优先级
