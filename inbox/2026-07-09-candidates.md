---
date: 2026-07-09
status: written
selected: candidate 1 → drafts/070-cost-routing-moat-xhs.md
---

# Today's Candidates

## Candidate 1: 美国 AI 初创公司正在悄悄把流量切给中国模型——CNBC 确认中国模型已占 US 企业 API token 的 30–46%，Lindy 100% 从 Claude 切 DeepSeek 省数百万美元（July 7）

- **Event**: 2026年7月7日，**CNBC** 发布深度调查报道：过去12个月，美国企业通过 **OpenRouter** 路由的 API token 中，中国模型份额的周均值已从 **11%** 上升至稳定在 **30% 以上**，峰值高达 **46%**——相比 2025 年上半年的 **4.5%** 增长近10倍。调查揭示的关键单一案例：约25人规模的 AI Agent 创业公司 **Lindy**（CEO Flo Crivello）将 **100% 的 AI Agent 推理流量**从 **Anthropic Claude** 全量切换至 **DeepSeek V4 Flash**（通过 Atlas Cloud 部署），推理成本降低约 **90%**，预计数月内节省"数百万美元"。切换前，AI 成本已超过薪资支出。Crivello 原话："这是生存问题。" Lindy 切换后未通知用户，用户无感知，服务不中断。同一调查覆盖另一个核心信号：**Zhipu（智谱）GLM 5.2** 于6月发布后，在 **Vercel** 平台创下 2026 年迄今最快模型采用速度，第一周 token 日使用量增长 **27 倍**，客户数量增长 **80 倍**。成本差距：中国开源模型比 Anthropic/OpenAI 领先模型便宜 **60–90%**。The Decoder 同日报道：《AI startup Lindy ditched Claude entirely for Deepseek, saving millions as cost pressure mounts on Anthropic》
- **Source**: https://www.cnbc.com/2026/07/07/chinese-ai-models-costs-us-openai-anthropic.html | https://the-decoder.com/ai-startup-lindy-ditched-claude-entirely-for-deepseek-saving-millions-as-cost-pressure-mounts-on-anthropic/ | https://www.lindy.ai/blog/migrating-from-claude-to-deepseek | https://letsdatascience.com/blog/startup-moved-100-percent-traffic-claude-to-deepseek
- **Timeliness**: 2 天前（2026年7月7日，CNBC 调查报道）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 这件事真正值得分析的不是"中国 AI 赢了"，而是它揭示了一个 AI 产品策略结构性变化：**当 Agent 推理成本高到超过薪资，"用最好的模型"不再是产品决策，"用刚好够好的模型"才是**。

  先把 Lindy 的决策逻辑还原出来。他们不是因为 Claude 不好才切——而是 Claude 贵到 AI 成本超过人力成本，继续用就是在烧钱维持情绪。DeepSeek V4 Flash 90% 更便宜，测试后任务完成率达标，切换。整个迁移过程用户无感知。Crivello 说：如果 Claude 降价，我会考虑切回去。这句话把事情说清楚了：**这不是对某个模型的信仰，是一个纯粹的成本路由决策**。

  CNBC 的数据把 Lindy 变成了一个行业信号：30-46% 的 US 企业 API token 已经流向中国模型。这个数字的背后不是"反美情绪"，是**任务路由经济学**：当 Agent 需要处理大量高频低复杂度任务（分类、摘要、格式转换），"好到 95 分但贵 10 倍"的模型不如"好到 85 分但便宜 90%"的模型。用 Claude 处理所有 Agent 任务，和用 Claude 处理所有 Excel 行，是同一个错误。

  对做 AI 产品或 AI Agent 基础设施的人，这件事有一个直接的产品架构含义：**未来 AI 应用层的护城河，可能不是"我用了最强的模型"，而是"我有最好的路由层"**——知道什么任务用什么模型，在质量和成本之间做动态分配。OpenRouter 周份额数据成为这个路由层的晴雨表。

  Anthropic 的问题不是 Lindy 切走了。是：当 Fable 5 因为"算力不足"退出订阅（昨天刚生效），同时 DeepSeek V4 Flash 切入了原本属于 Claude Sonnet 的中端推理市场——Anthropic 的用量定价模型在中端市场正在被两端挤压：上边 Fable 5 贵到不可持续，下边 Claude Sonnet 输给 DeepSeek V4 成本。

  中文媒体会报"DeepSeek 在美国大受欢迎"，不会分析：**Lindy 的 100% 迁移揭示的是 AI 产品层的成本路由革命——"任务路由经济学"正在成为 AI 产品决策的底层逻辑，而谁控制路由层，谁就控制了 Agent 时代的分发入口。**

- **Resonance hook**: 7月7日，CNBC 确认：美国企业 30–46% 的 AI API token，正在流向中国模型。1年前这个数字是 4.5%。Lindy（25 人 AI Agent 初创）把 100% 的推理流量从 Claude 切给了 DeepSeek V4 Flash，成本降 90%，省了数百万——用户没有任何感知。CEO Flo Crivello 的原话："这是生存问题。" 不是中国 AI 赢了情感战，是 Agent 推理成本高到超过薪资时，任何理性的产品团队都会做同样的决策。
- **Recommended priority**: high

---

## Candidate 2: NVIDIA GEAR Lab 开源 ASPIRE：机器人 skill library 让机器人有了持久记忆——Jim Fan 说 embodied AI 训练范式已经变了（July 1–2）

- **Event**: 2026年7月1日，**NVIDIA GEAR Lab**（由 **Jim Fan** 担任共同负责人）在 GitHub 开源了 **ASPIRE**（Agentic Skill Programming through Iterative Robot Exploration），同日发布 arXiv 论文 2607.00272（2026年7月2日）。ASPIRE 是一套用于具身机器人的**持续学习系统**，核心创新：机器人不再每次从头学习，而是把每次执行经验——无论成功还是失败——提炼成可复用的 **skill library**（技能库），下次遇到相同或相似任务直接调用并在此基础上迭代。技术架构：Code-as-Policy 范式，机器人自主写控制代码 → 执行 → 分析失败原因 → 修复程序 → 提炼为可复用 skill → 存入持久库。实测结果：**双臂物体传递任务**（dual-arm handover）成功率从 **20% → 92%**，长程任务泛化测试中，随着技能库规模扩大，成功率**持续提升**（而不是触及天花板）。Jim Fan 在 X 上的评价（[@DrJimFan](https://x.com/DrJimFan/status/2072004192294830583)）：这代表训练范式的根本转变——训练输出从**模型权重**变成了**持续扩展的技能库**；训练过程从**梯度下降**变成了**技能精炼**。Jim Fan 将这个架构的终点称为 **Physical API**：机器人操控原子的方式，就像软件操控比特一样。TechTimes（7月1日）：《Robot Skill Library ASPIRE Gives Robots Memory: Handover Climbs to 92%》
- **Source**: https://arxiv.org/abs/2607.00272 | https://research.nvidia.com/labs/gear/aspire/ | https://finance.biggo.com/news/b6c73fe9-9d01-41ed-a24f-be027f8a0645 | https://www.techtimes.com/articles/319443/20260701/robot-skill-library-aspire-gives-robots-memory-handover-climbs-92.htm | https://x.com/DrJimFan/status/2072004192294830583
- **Timeliness**: 7–8 天前（GitHub 开源 7月1日，arXiv 论文 7月2日，Jim Fan X 帖子同日）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: ASPIRE 真正值得单独分析的，不是"机器人又更聪明了"，而是它改变了 **AI 能力积累的单位**。

  现在的 LLM 训练：输入大量数据 → 梯度下降 → 输出一套固定权重。当权重被冻结，模型的知识就被锁住了，能力的上限在训练结束的那一刻就定了。ASPIRE 改变的是这件事：训练的输出不是一套固定权重，而是一个**持续增长的技能库**。机器人每次完成任务（哪怕失败），都在往技能库里写入东西。下次遇到相似任务，不用重新学，直接调用并在已有技能基础上扩展。

  Jim Fan 说这是从"梯度下降"到"技能精炼"的转变——这不只是技术架构的差异，是 AI 能力积累逻辑的根本分叉：**一种是训练结束能力就封顶，另一种是使用越多能力越强**。后者才是持续演化的系统。

  从 Zico 工作的领域看这件事：3DGS（3D Gaussian Splatting）和空间智能的核心问题之一，一直是"如何让模型在真实三维世界里持续学习"。ASPIRE 的技能库架构，给了一个具体的答案——不是让模型记住三维世界的所有状态，而是让它把"如何操作这个世界的经验"提炼成可调用的 skill，每次交互都在扩展这个库。20% → 92% 的双臂传递成功率，是一个具体数字，但背后说的是：**一个有技能库的 Agent，和一个没有技能库的 Agent，在同一个任务上的能力差距是指数级的**。

  对理解 physical AI 和 embodied AI 的人，这个结构有一个直接的类比：ASPIRE 对于机器人，就像 RAG 对于 LLM——区别在于 RAG 检索的是外部知识，ASPIRE 检索的是自己积累的操作经验。两者都在做同一件事：让模型的有效能力边界，超过它的静态训练权重。

  中文媒体会报"NVIDIA 开源新机器人技术"，不会分析：**ASPIRE 的技能库架构代表了 embodied AI 能力积累逻辑的范式转变——从"训练封顶"到"使用越多能力越强"，这是物理世界 AI 从静态权重迈向持续演化系统的第一个可量化的里程碑（20%→92%）。**

- **Resonance hook**: 7月1日，NVIDIA GEAR Lab 开源 ASPIRE。机器人双臂传递任务成功率：20% → 92%。但数字不是重点，重点是训练范式的变化：训练的输出不再是固定的模型权重，而是一个持续扩展的技能库。机器人每次执行任务（成功或失败），都在往技能库里写东西。使用越多，能力越强。Jim Fan（NVIDIA Director of AI）称这是从"梯度下降"到"技能精炼"的根本转变——以及他设想的终点：Physical API，机器人操控原子，就像软件操控比特。
- **Recommended priority**: high

---

## Candidate 3: GPT-5.6 Sol/Terra/Luna 今天全球上线——这是史上第一个经过美国政府 CAISI 正式评估并放行的前沿 AI 模型（July 9 TODAY）

- **Event**: 2026年7月9日（今天），**OpenAI** 正式向全球公开发布 **GPT-5.6** 三模型家族：**Sol**（前沿推理 + 长链 agentic 工作，$5/$30 per M token）、**Terra**（日常任务，性能接近 GPT-5.5 但成本减半，$2.50/$15）、**Luna**（最快最便宜，$1/$6）。新增 **Ultra Mode**：调用多个子 Agent 并行加速复杂任务。距离模型首次预览发布（6月26日）已过去13天。**关键背景**：6月25日，特朗普政府以安全顾虑为由，要求 OpenAI 将 GPT-5.6 的发布限制为约20家"受信任合作伙伴"，暂停面向公众发布。OpenAI 同意，并安排工程师赴华盛顿 D.C. 回答美国商务部下属机构 **CAISI**（Center for AI Standards and Innovation，AI 标准与创新中心）的技术审核问题。7月8日，特朗普政府宣布解除限制，GPT-5.6 获准今日公开发布。此次审核的法律依据：特朗普6月初签署的 AI 网络安全行政令，要求 AI 公司在发布最强大模型前，**自愿**提前30天向政府提交评估（商务部须在60天内建立评估流程）。这是 CAISI 首次对一个商业前沿 AI 模型发出正式放行信号。来源：**Axios**（2026年6月25日，《Trump administration asks OpenAI to limit release of GPT-5.6》）、**Axios**（2026年7月8日，《Scoop: Trump administration lifts restrictions on OpenAI's GPT 5.6》）、**CNBC**（2026年7月8日，《OpenAI to publicly release GPT-5.6, rolls out conversational AI models》）、**Neowin**（2026年7月9日，《OpenAI to release GPT-5.6 Sol, Terra and Luna on July 9》）
- **Source**: https://www.axios.com/2026/06/25/trump-administration-openai-gpt-model-release | https://www.axios.com/2026/07/08/openai-gpt-trump-ban-lifted | https://www.cnbc.com/2026/07/08/openai-expanding-gpt-5point6-ai-model-release-ending-government-limits.html | https://www.neowin.net/news/openai-to-release-gpt-56-sol-terra-and-luna-on-july-9/ | https://techmymoney.com/2026/07/08/openai-gpt-56-public-rollout-july-9-sol-terra-luna/
- **Timeliness**: 今天（2026年7月9日正式全球上线）；政府审核 6月25日—7月8日（13天）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 这件事真正值得分析的不是 GPT-5.6 的能力（这个昨天和上周都有报道），而是**它揭示了 AI 发布链条里出现了一个新的制度节点：CAISI 首次扮演了前沿 AI 模型的"发布许可机构"**。

  先把这件事的结构说清楚。特朗普6月签署 AI 网络安全行政令，要求 AI 公司在发布最强模型前自愿提前30天让政府评估。OpenAI 遵守了。GPT-5.6 从 6月26日预览到 7月9日公开上线，中间13天不是工程准备期，是 CAISI 的审核窗口。最终放行信号不是 OpenAI 自己决定的——是美国政府宣布"解除限制"之后，今天才上线。

  "自愿"这个词很重要，也很脆弱。Anthropic 是否会为 Fable 5 的下一个版本走同样流程？Google 的 Gemini 3.5 Pro 正在赶7月17日，它需要经过 CAISI 吗？目前答案不清楚，但先例已经建立：**美国历史上第一次，一个前沿 AI 模型在公开发布前经过了一个政府机构的正式技术审查并获得放行**。这个先例的重量，和行政令是否明文要求无关——先例一旦形成，"为什么 GPT-5.6 走了审查但你的模型没走"这个问题，是任何下一家公司都要面对的政治压力。

  对做 AI 产品战略和组织决策的人，这件事有一个直接的结构性含义：**AI 的发布链条正在从"公司内部决定"迁移到"公司 + 政府双重节点"**。FDA 审批药物，FAA 认证飞机——CAISI 也许会成为前沿 AI 的那个机构。区别在于：FDA 的审批是强制的，CAISI 的评估目前是"自愿的"。但自愿和强制之间的距离，往往只有一次事故。

  中文媒体会报"GPT-5.6 今天上线"，不会分析：**美国商务部 CAISI 首次对前沿 AI 模型发出正式放行信号——"自愿政府审查"是 AI 发布链条的新制度节点，GPT-5.6 是第一个，但不会是最后一个。**

- **Resonance hook**: 今天（7月9日），GPT-5.6 Sol/Terra/Luna 全球上线。但今天真正发生的事，不是三个新模型。是：这是史上第一次，一个前沿 AI 模型经过美国商务部 CAISI 正式技术审查、并在政府宣布"解除限制"之后才公开上线。6月25日特朗普政府叫停了原定的公开发布，要求 OpenAI 先接受审查。OpenAI 工程师飞去华盛顿 D.C.，CAISI 评估了13天，7月8日宣布放行。自愿的，暂时的，但先例已经建立：AI 的发布链条，第一次出现了政府的放行节点。
- **Recommended priority**: high

---

## Scan summary
- **Sources scanned**:
  - CNBC（2026年7月7日，《Chinese AI models are gaining ground with U.S. companies as OpenAI, Anthropic costs surge》）
  - The Decoder（《AI startup Lindy ditched Claude entirely for Deepseek, saving millions》）
  - Lindy 官方博客（《Migrating from Claude to DeepSeek》）
  - resultsense.com（2026年7月7日，《Chinese AI models seize up to 46% of US developer use》）
  - letsdatascience.com（《Chinese AI Models Overtake US Rivals in Token Usage》）
  - cryptobriefing.com（《Chinese AI models now claim over 30% of US OpenRouter traffic》）
  - The Decoder（《Chinese AI models regularly pass 30 percent on OpenRouter as cost gap widens》）
  - arXiv 2607.00272（ASPIRE: Agentic Skill Discovery for Robotics，July 2）
  - NVIDIA GEAR Lab（ASPIRE 项目主页）
  - finance.biggo.com（《Nvidia Open-Sources ASPIRE Robot Skill Library; Jim Fan Says Embodied AI Training Paradigm Has Shifted》）
  - TechTimes（2026年7月1日，《Robot Skill Library ASPIRE Gives Robots Memory: Handover Climbs to 92%》）
  - Jim Fan @DrJimFan X posts（ASPIRE open-source announcement）
  - Axios（2026年6月25日，《Trump administration asks OpenAI to limit release of GPT-5.6》）
  - Axios（2026年7月8日，《Scoop: Trump administration lifts restrictions on OpenAI's GPT 5.6》）
  - CNBC（2026年7月8日，《OpenAI to publicly release GPT-5.6》）
  - Neowin（2026年7月9日，《OpenAI to release GPT-5.6 Sol, Terra and Luna on July 9》）
  - techmymoney.com（2026年7月8日，GPT-5.6 global rollout）
  - TechTimes（2026年7月8日，《Gemini 3.5 Pro Targets July 17 as DeepSeek's July 24 Deadline Hits Developers Now》）
  - HackerNoon（《Google Delays Gemini 3.5 Pro to July 17: The Strategic Play》）
  - unrot.co（2026年7月8日，《Top 10 AI News: July 8 2026》）
  - buildfastwithai.com（2026年7月8日，《AI News Today July 8 2026: 15 Biggest Stories》）
  - Karpathy bearblog（《Sequoia Ascent 2026 summary》——评估后排除：Sequoia AI Ascent 为 4月30日，Karpathy 推文约5月初，超出7天窗口）
  - TechCrunch（2026年6月20日，John Jumper leaving DeepMind for Anthropic——超出7天窗口，排除）
  - Anthropic官网（Claude Sonnet 5 定价细节——6月30日发布，9天前，borderline，已被7月6日 Candidate 3 Claude Science 覆盖同一公司同日事件）
  - OSSInsight GitHub Trending（July 2026，无单一突破性新项目超过7天窗口）
  - Latent Space / Swyx（无最新相关 AI 工程深度文章，7月5日文章为个人感想，排除）
  - DeepSeek V4 API migration（July 24截止日——开发者运维层面，Zico 受众匹配度低，排除）

- **Total signals found**: 约 25 个信号评估

- **Why these 3**:

  - **Candidate 1（Chinese AI 30–46% US enterprise tokens / Lindy 100% 切 DeepSeek，7月7日）**：**AI产品战略柱**——此柱最近一次覆盖为7月8日（Fable 5 退订 + 算力不足声明），今日角度完全不同：从"最强模型的定价瓶颈"转向"中端推理任务的成本路由革命"；CNBC 调查 + Lindy 官方博客双重一手来源，数据具体可查（30-46%、90% 成本降低、100% 流量迁移）；Lindy CEO Crivello 公开承认"AI 成本超过薪资"是"生存问题"——这句话是整个行业隐而不宣的现实；Zhipu GLM 5.2 第一周 Vercel 27x token 增长作为第二数据点加强信号；中文媒体报"DeepSeek 赢了！"，不分析任务路由经济学和"路由层控制权"的产品战略含义；**HIGH 优先级**。

  - **Candidate 2（NVIDIA ASPIRE open-source 技能库，7月1–2日）**：**深层AI思考柱**——此柱最近一次覆盖为7月8日（GPT-5.6 Sol METR 安全评测与能力可测性反向关系），今日角度完全不同：从"AI 能力的不可测性"转向"embodied AI 能力积累范式从权重冻结到技能库持续扩展"；时效7–8天（Tier 2 arXiv/开源源，7天窗口边缘可接受）；Jim Fan 是 X/Twitter 上的 KOL（满足 Tier 1 来源要求），open-source 事件和 arXiv 论文提供双重时效锚点；20%→92% 这组数字是可量化的里程碑，不是抽象进展；与 Zico 自身在酷家乐做 3DGS/空间智能的背景高度匹配，具有内行视角；中文媒体报"NVIDIA 机器人技术进步"，不分析"技能库架构"对 physical AI 能力积累逻辑的根本改变；**HIGH 优先级**。

  - **Candidate 3（GPT-5.6 全球今日上线 + CAISI 首次政府放行，今天）**：**组织形式变革柱**——此柱最近一次覆盖为7月6日（Tesla AI 工具支出封顶 + Grok 豁免），今日角度完全不同：从"企业 AI 成本治理"转向"政府机构成为 AI 发布链条的制度节点"；虽然 GPT-5.6 Sol 已在7月8日候选中覆盖（METR 安全测试失败角度），但今日角度是 CAISI 政府审查放行机制的历史首次——是"AI 发布制度基础设施"而非模型性能或安全评测；Axios 两篇独家报道（6月25日封锁 + 7月8日解封）提供一手来源；"自愿→强制"的先例建立逻辑，是任何 AI 公司产品发布战略必须理解的结构变量；发现式钩子：今天上线的表象下，是 CAISI 第一次行使"放行"权力的事实——这个细节在绝大多数中文报道中不会出现；**HIGH 优先级**。
