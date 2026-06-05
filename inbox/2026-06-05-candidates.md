---
date: 2026-06-05
status: written
selected: candidate 2 → drafts/038-chatgpt-ads-fork-xhs.md
---

# Today's Candidates

## Candidate 1: OpenAI GPT-Rosalind June 3 重大更新——专项模型首次在所有评估维度超越 GPT-5.5，基因组学分析少用 31% token，向全球机构开放（June 3）

- **Event**: 2026年6月3日，OpenAI 在官网发布 GPT-Rosalind 重大能力更新（"Introducing new capabilities to GPT-Rosalind"）。关键数字：更新后模型在所有测试生命科学领域均超越 GPT-5.5（OpenAI 当前通用旗舰），且 token 效率优势在基因组学最显著——完成长周期定量生物学分析比 GPT-5.5 **少用 31% token**。新能力：① **Life Sciences Research Plugin** 和 **Life Sciences NGS Analysis Plugin**，接入 50+ 科学数据库，将证据检索、生物学解读、生物信息学执行整合在同一工作区；② **研究预览版首次向全球机构开放**（此前限于美国部分机构），采用受信赖访问结构（要求合法科研目的 + 强治理安全监督 + 企业级控制访问）。合作伙伴扩展：**Novo Nordisk**（4月与 OpenAI 签署战略合作，覆盖药物发现、制造、供应链和商业运营）正式接入 GPT-Rosalind，用于跨文献/基因组学/转录组学/结构生物学整合证据、测试假设。时间背景：GPT-Rosalind 初版于2026年4月发布（定位"面向生命科学研究的 AI"）；6月3日更新是首个重大能力更新，标志从"局限于少数合作机构"扩展至"全球受信赖访问"。
- **Source**: https://openai.com/index/introducing-new-capabilities-to-gpt-rosalind/ | https://www.techtimes.com/articles/317754/20260604/gpt-rosalind-drug-discovery-update-openai-cuts-genomics-compute-expands-global-access.htm | https://www.ciol.com/generative-ai/openai-pushes-deeper-into-drug-discovery-with-gpt-rosalind-upgrade-12000797 | https://www.digit.in/news/general/openai-expands-access-to-gpt-rosalind-its-most-advanced-ai-model-for-scientific-research-all-details.html
- **Timeliness**: 2天前（2026年6月3日，OpenAI 官方发布）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: GPT-5.5 是 OpenAI 的当前通用旗舰。GPT-Rosalind 在药物发现领域比 GPT-5.5 更好，还更便宜（少31% token）。这不是"垂直 AI 创业公司"的故事，而是同一家公司内部的产品结构分叉。

  OpenAI 正在同时运营两套逻辑：GPT-5.5 = 通用智能基础设施；GPT-Rosalind = 生命科学专项引擎。两者服务不同客户，优化不同目标，定价不同。这个分叉背后有一个结构性判断：**通用模型的规模扩展，已经到达"专项模型能以更低成本在特定领域超越它"的临界点**。

  这打破了两个常见假设。第一个假设："只要 scaling law 继续，旗舰模型会最终覆盖一切"——Rosalind 告诉你，药物发现这个领域已经不是这样了，用旗舰模型做基因组学分析不仅更贵，而且结果更差。第二个假设："垂直 AI 创业公司的护城河是领域数据"——但 Rosalind 接入了50+ 科学数据库，Novo Nordisk 的战略合作覆盖了供应链和商业运营。OpenAI 在说的是：**我不只是卖 API，我要直接承接你的 domain problem**。

  Novo Nordisk 的选择值得单独看：一家全球领先的制药公司，选择与 OpenAI 签战略合作（不是买垂直 AI 创业公司的产品），让 AI 旗舰实验室深入到药物发现的每个环节。这个客户决策的逻辑是：当基础模型公司本身开始解决你的 domain problem，中间层的垂直 SaaS 产品必须重新想清楚自己的定位——是在 OpenAI 体系里做集成商，还是在 OpenAI 没有覆盖的更窄场景里做专精者？

  做 AI 产品的人需要回答这个问题：你的产品是在帮用户更好地使用通用 AI，还是在提供通用 AI 提供不了的东西？GPT-Rosalind 在告诉你，后者的空间在被持续压缩。

- **Resonance hook**: 2026年6月3日，OpenAI 更新了 GPT-Rosalind，在所有生命科学领域全面超越 GPT-5.5，基因组学分析少用 31% token。GPT-5.5 是 OpenAI 的当前通用旗舰。同一家公司，专项模型打败自家旗舰。这不是例外，是结构信号：通用模型做基础设施，专项模型做应用层，OpenAI 已经在自己的产品矩阵里印证了这个分叉。Novo Nordisk 没有选一个垂直 AI 创业公司——它直接和 OpenAI 签了战略合作。垂直 AI 的护城河正在被重新定义。
- **Recommended priority**: high

---

## Candidate 2: ChatGPT 今日正式开放转化优化广告——OpenAI 进入 Performance Marketing，8亿月活用户成为广告资产（June 5）

- **Event**: 2026年6月5日（今天），OpenAI 在 ChatGPT Ads Manager 中正式开放**转化优化广告活动（Conversion-Optimized Campaigns）**早期访问，仅限6月1日前已配置 JavaScript Pixel 或 Conversions API 的广告主。这是 ChatGPT 广告平台从"曝光/流量"跨越至"效果（Performance Marketing）"的关键里程碑——进入 Google Ads 和 Meta 的核心战场。完整时间轴：**2026年1月16日**，OpenAI 宣布面向美国免费和 Go 层用户测试广告；**2月9日**，广告正式上线（Free + Go，$8/月）；**3月26日**，广告 ARR 突破**$1亿**（距上线不足2个月，Reuters 确认）；**5月**，扩展至英国、墨西哥、巴西、日本、韩国；**6月5日**，转化优化功能开放早期访问；用户层级结构：**Pro/Business/Enterprise 订阅用户不看广告**，免费和 Go 用户看广告，或可选择减少每日免费消息换取无广告体验。收入目标：2026年广告收入目标 **$25亿**，2028年 **$250亿**，2030年 **$1000亿**（内部文件）。市场影响：DataBeat 5月报告（35亿+ 月均 impressions 样本）显示，美国 programmatic CPM 4月同比上涨 **33.9%**，移动端 CPM 同比上涨 **51.6%**；广告不影响 ChatGPT 回答内容，OpenAI 声明不向广告主出售用户对话数据。
- **Source**: https://openai.com/index/testing-ads-in-chatgpt/ | https://openai.com/index/new-ways-to-buy-chatgpt-ads/ | https://ppc.land/chatgpt-launches-conversion-ads-june-5-us-programmatic-cpms-up-34/ | https://digiday.com/marketing/openai-opens-up-chatgpt-ads-manager-to-the-u-s-while-promising-third-party-measurement-cpa-bidding/ | https://searchengineland.com/openai-confirms-conversion-focused-ads-are-coming-to-chatgpt-478843
- **Timeliness**: 今天（2026年6月5日，转化优化广告早期访问开放日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: OpenAI 今天在产品结构上做了一个不可逆的选择：**同一家公司，同时运营两套激励逻辑**。

  企业端（Pro/Business/Enterprise）：订阅收费。AI 回答越直接有效，用户感知价值越高，续费率越高。优化目标 = 用户效用最大化。

  消费者端（Free/Go）：广告收费。广告转化率越高，advertiser 愿意付的 CPM 越高，OpenAI 收入越高。优化目标 = 用户注意力停留 × 意图匹配精度。

  问题在于：**这两个优化目标在某些场景下是矛盾的**。一个能用两句话直接解决问题的 AI，在广告模式下实际上是反激励的——用户不用深入探索，广告展示机会就少了。Google 用了20年在这个张力里找平衡，代价是搜索结果里广告占比越来越高、用户对搜索推荐的信任度持续下降。OpenAI 说"广告不影响答案内容"——这在技术上可能是真的，但在系统激励层面，这个分裂迟早会产生摩擦。

  对比 Anthropic 的选择：Claude.ai 完全订阅制，没有广告。两家公司的商业模式正在从"都是 AI 公司"分化为"完全不同的经济结构"。这个结构不只影响收入，它会影响产品团队的 OKR、模型训练的目标函数、和用户关系的长期性质。

  对于做 AI 产品的人，这里有一个关键判断要做：你在构建的是面向 OpenAI 消费者生态的东西，还是面向 Anthropic 企业生态的东西？两者接下来的演化方向，由它们各自的商业模式激励决定，而不是由技术能力决定。

- **Resonance hook**: 今天，ChatGPT 广告后台正式开放转化优化功能。从2月上线到3月 ARR 破亿，只用了不到2个月。OpenAI 的8亿月活用户，现在是两种不同的资产：付费用户是 SaaS 收入，免费用户是广告库存。同一家公司，同时卖"效率工具"给企业，卖"注意力"给广告主。Anthropic 只卖前者。这不是竞争策略的差异，是关于 AI 应该优化什么的根本性分叉——订阅制 AI 优化用户效用，广告制 AI 优化用户停留。
- **Recommended priority**: high

---

## Candidate 3: Apple 在 CVPR 2026 发布 SFI-Bench——当前所有主流多模态模型都无法理解"这个物体能用来干什么"（June 3–7）

- **Event**: 2026年6月3日至7日，CVPR 2026 在科罗拉多丹佛举行。Apple 在会上提交14篇研究论文，其中最值得关注的是 **《From Where Things Are to What They're For: Benchmarking Spatial-Functional Intelligence for Multimodal LLMs》**（从"东西在哪里"到"东西能做什么"：为多模态大模型标定空间功能智能基准）。该研究提出 **SFI-Bench** 基准测试，包含来自 **134 个室内视频扫描**的 **1,555 道专家标注问题**，评估两个维度：① **结构化空间推理**（理解复杂布局、形成连贯空间表征）；② **功能推理**（推断物体的 affordance，即在特定上下文中"能用来做什么"）。评估任务包括条件计数、多跳关系推理、功能配对（哪两件物品应该总是一起出现）和知识指导的故障排除（这个摆放方式有什么问题）。**核心发现：当前主流多模态大模型（MLLMs）在将空间记忆与功能性知识整合方面持续表现不足**——模型能说出物体在哪里，但无法推断这个物体在此上下文中"有什么用"。时间背景：Apple 在 CVPR 论文方向与即将发布的 iOS/visionOS 功能存在明确对应（空间感知无障碍功能、图像编辑工作流）；WWDC 2026 通常在6月举行，Apple 本次 CVPR 亮相被多家媒体解读为 WWDC 前的 AI 研究预览。
- **Source**: https://machinelearning.apple.com/research/spatial | https://machinelearning.apple.com/updates/apple-at-cvpr-2026 | https://theroboticsmedia.com/article/apple-cvpr-2026-14-papers-vision-research-denver | https://appleinsider.com/articles/26/05/28/apples-ai-research-will-be-in-a-computer-vision-conference-before-wwdc
- **Timeliness**: 3天前（CVPR 2026 开幕日为2026年6月3日，论文正式呈现于会议现场，大会持续至6月7日）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: 这篇论文直接点名了我在做 3DGS 产品时反复遇到的一个壁垒：**空间感知和空间功能理解是两件事，但几乎所有的空间 AI 基准都只测前者**。

  传统的空间理解测试问的是："桌子在哪里？""椅子距离墙壁多远？"SFI-Bench 问的是："在这个厨房布局里，这两件物品应该总是放在一起吗？""这张沙发的摆放方式有什么功能性问题？"前者是几何感知，后者是上下文功能推理——需要把空间位置、物体属性知识和场景使用规则同时整合起来。

  Apple 的基准测试发现：当前所有主流 MLLM 都做不好这件事。这不是 benchmark engineering 问题，是真实的能力壁垒。

  在室内设计 AI 的场景里，这个壁垒就是用户反馈里最常出现的那类问题：AI 知道沙发在哪里，但不知道沙发是否应该对着电视；AI 能识别餐桌，但不知道这个空间里是否适合放餐桌。这是 3D 产品从"能看见"到"能判断"的本质跨越。我们在酷家乐做 3DGS 产品的时候，这个跨越一直是最难量化的部分——因为没有一个基准能告诉你"你现在在哪里，还差多远"。Apple 今天给了一个答案：SFI-Bench，1,555道题，你可以测自己的模型在哪里。

  另一个值得关注的信号：**Apple 在 CVPR 上定义这个基准，意味着他们在 Vision Pro / visionOS 的产品路线图里，已经把"功能推理"当作核心能力来建设**。谁定义了基准，谁就在说"什么才算做好了"。这不是学术贡献，是标准制定——在 spatial AI 的产品竞争里，这和专利一样重要。

  空间 AI 的下一个真实瓶颈已经被明确：不是重建精度，不是渲染质量，而是**从"看见"到"理解用途"的推理跨越**。

- **Resonance hook**: CVPR 2026 本周在丹佛进行，Apple 带来了14篇研究论文。其中一篇直接测试了一件事：当前的多模态 AI 能理解"这把椅子在这个上下文里能用来干什么"吗？答案是不能。1,555 道专家标注问题，当前所有主流 MLLM 在"空间功能推理"上持续失败。它们能说出物体在哪里，但无法推断这个物体在此场景中有什么用。Apple 把这个能力缺口定义成了基准：SFI-Bench。空间 AI 的下一个技术壁垒不是重建精度，是理解"用途"。
- **Recommended priority**: medium

---

## Scan summary

**Sources scanned**:
- OpenAI 官方 newsroom（openai.com/index/introducing-new-capabilities-to-gpt-rosalind/，June 3 2026，GPT-Rosalind 重大更新；openai.com/index/testing-ads-in-chatgpt/ + openai.com/index/new-ways-to-buy-chatgpt-ads/，ChatGPT 广告转化优化官方来源）
- TechTimes（June 4，GPT-Rosalind drug discovery update，基因组学 token 效率数据确认）
- CIOL + digit.in（GPT-Rosalind upgrade 多源确认）
- pharmaphorum + Fierce Biotech（GPT-Rosalind 初版发布背景，April 2026）
- ppc.land（June 5 ChatGPT 转化广告上线 + US programmatic CPM +33.9% 数据）
- digiday（ChatGPT Ads Manager CPA bidding，June 5 开放范围确认）
- searchengineland（转化优化广告功能技术细节确认）
- Reuters / CNBC via multiple secondary（3月 ARR $1亿里程碑确认）
- Apple Machine Learning Research 官方（machinelearning.apple.com/research/spatial，SFI-Bench 论文正式来源；machinelearning.apple.com/updates/apple-at-cvpr-2026，CVPR 2026 参会确认）
- The Robotics Media（Apple 14篇论文 CVPR 2026 详情）
- AppleInsider + Let's Data Science（Apple CVPR 论文 WWDC 预热报道，5月28-29日发布）
- GitHub Trending / OSSInsight（AI repos June 2026：Hermes agent 140K stars 于5月13日，超7天窗口排除；Understand-Anything 当周爆发无精确事件锚点排除；awesome-ai-agents-2026 系列为汇总型清单无独立锚点排除）
- HN top AI posts（June 4-5：Anthropic surpasses OpenAI valuation 为主导话题，已在June 3 candidates 全面覆盖排除；其余为技术讨论类无独立事件锚点）
- YC Blog（无确认 June 1-5 新 AI 深度文章，排除）
- Karpathy（May 19 加入 Anthropic 已在近期 candidates 排除记录；无独立 June 3-5 新帖子）
- Jim Fan / Swyx（无确认 June 3-5 独立锚点，Sequoia AI Ascent April 超30天窗口排除）
- Google DeepMind DOE Genesis（January 8 2026 宣布，超30天窗口排除）
- A2A Protocol v1.0（April 2026 一周年里程碑，超30天窗口排除；Build 2026 Microsoft 集成 June 2 已在 June 2 candidates 全面覆盖排除）
- LlamaCon（2025年活动；April 2026 Meta AI releases 无精确 June 3-5 锚点）
- OpenAI AWS Bedrock（June 1-2，已在 June 3 scan 中以"微软/OpenAI关系叙事角度重叠"排除）
- arXiv June 2026（cs.AI current + cs.LG current：扫描未发现有精确 June 3-5 2026年发布且具备独立叙事强度的单篇突破论文）
- CVPR 2026 Demo（June 5 demos：GazeAnywhere/ARVRag/MIBURI 为技术演示类，无独立产品战略叙事锚点，排除）

**Total signals found**: 约29个评估

**Why these 3**:

- **Candidate 1（OpenAI GPT-Rosalind June 3 更新）**：时效2天，OpenAI 官方 + TechTimes June 4 + CIOL + digit.in 四方来源确认；AI 产品战略柱：过去3天 SELECTED 覆盖了 Anthropic Partner Network（June 4，分发渠道锁定）和 Anthropic IPO（June 3，估值与安全定位）——今天角度完全不重叠："同一家公司内专项模型在所有评估维度超越自家通用旗舰"是模型层分叉的新结构信号；31% token 效率优势 + 全球受信赖访问开放是首次披露的独立可追溯数据点；Novo Nordisk 战略合作覆盖药物发现全链路是企业采购模式转变的具体案例；中文媒体会报道"OpenAI更新生物医学模型"但不会分析"专项模型超越旗舰模型意味着什么"；HIGH 优先级。

- **Candidate 2（ChatGPT 转化广告 June 5）**：时效最强（今天），OpenAI 官方 + ppc.land + digiday + searchengineland 四方来源确认；组织形式变革柱：过去3天 SELECTED 覆盖了 Trump EO（June 4，监管形态）和 Windows Agent Platform（June 2，OS用户重定义）——今天角度完全不重叠："AI 旗舰实验室同时建立订阅 + 广告双激励结构"是商业形态演变的分叉叙事；ARR $1亿（6周内）+ CPM +33.9%（DataBeat独立数据）是可验证的市场影响数字；"转化优化 = 进入 Performance Marketing"是比"ChatGPT显示广告"更深一层的里程碑信号；中文媒体会报道"ChatGPT开放转化广告"但不会分析"订阅激励 vs 广告激励对 AI 产品优化目标的结构性分叉"；HIGH 优先级。

- **Candidate 3（Apple SFI-Bench CVPR 2026，June 3-7）**：时效3天（CVPR 大会正在进行中），Apple ML Research 官方 + The Robotics Media + AppleInsider 三方来源确认；深层AI思考柱：上次 SELECTED 为 June 3 Tesla 神经世界模拟器（物理AI数据护城河），今天角度完全不重叠——"从空间感知到空间功能推理的能力缺口"是认知层面的新框架，不是基础设施层；1,555道专家标注问题基准是具体可验证的技术指标；与 Zico 在酷家乐做 3DGS 产品的一线认知有直接对照（"AI知道沙发在哪里，但不知道沙发是否应该对着电视"就是这个项目反复遇到的边界）；Apple WWDC 2026 连接增加产品落地可信度；中文媒体不会报道 Apple 的 CVPR 学术论文；MEDIUM 优先级（学术论文而非产品发布，但深层AI思考柱明确适合此类内容，且 Zico 对空间AI的一线背景让这个选题有特殊匹配度）。
