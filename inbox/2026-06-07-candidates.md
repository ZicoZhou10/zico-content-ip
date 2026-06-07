---
date: 2026-06-07
status: pending_selection
---

# Today's Candidates

## Candidate 1: Apple WWDC 2026 明天开幕：iOS 27 "Extensions" 框架让用户自由切换 Claude/Gemini/Grok/Perplexity，Apple 正式从 AI 公司退出、成为 AI 操作系统（June 5–6）

- **Event**: 2026年6月5日，Bloomberg Mark Gurman 发布 WWDC 2026 完整预览报道；2026年6月6日，TechTimes 等多家媒体跟进确认。WWDC 2026 于明天（2026年6月8日）上午10点开幕——亦是 Tim Cook 作为 CEO 的最后一次 WWDC 主题演讲（他将于9月1日移交 CEO 职务给 John Ternus）。三个核心信号：① **Apple 与 Google 签署 $10亿/年协议**，采购定制版 **1.2万亿参数 Gemini 模型**作为重建后 Siri 的云端智能核心（协议合同条款：Google 不得使用 Apple 用户的 Siri 对话数据训练 Gemini）；② **iOS 27 "Extensions" 框架**：用户将可在设置中将 Siri、Writing Tools、Image Playground 的大脑替换为 ChatGPT、Claude、Gemini、Grok、Perplexity 或 Mistral Le Chat 中的任何一个——这终结了 ChatGPT 自2024年12月（iOS 18.2）起作为唯一第三方 AI 集成的独家地位；③ **"Extensions" 机制**：AI 厂商通过各自 App Store 应用接入，用户一键切换，路由系统范围内所有 AI 请求。该功能计划与 iOS 27 于2026年秋季随 iPhone 17 同步发布，届时将覆盖超过 **14亿台 iPhone**。
- **Source**: https://www.bloomberg.com/news/articles/2026-06-05/wwdc-2026-preview-ios-27-siri-ai-features-macos-27-more-apple-will-announce | https://www.techtimes.com/articles/317902/20260606/wwdc-2026-opens-monday-gemini-powers-rebuilt-siri-iphone-11-faces-ios-27-cut.htm | https://www.macrumors.com/guide/wwdc-2026-what-to-expect/ | https://letsdatascience.com/blog/apple-ios-27-extensions-claude-grok-third-party-ai | https://www.cnbc.com/2026/01/12/apple-google-ai-siri-gemini.html
- **Timeliness**: 1天前（Bloomberg June 5 预览 + TechTimes June 6 确认；WWDC 主题演讲明日开幕）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: ChatGPT 在 iOS 上的独家优势是2024年 AI 领域最被低估的分发护城河。用一个事实说明这件事的规模：iOS 18.2 让 ChatGPT 成为10亿+用户的"系统级 AI"——不是 App Store 里的一个 app，而是操作系统里的一个能力层。这比任何一次营销活动的效果都强。

  Apple 今天在做的事，是把这个分发护城河从 OpenAI 手里拿走，开放给所有人。iOS 27 Extensions 的本质不是"苹果更民主了"，而是"苹果决定把 AI 竞争变成自己的平台竞争"。从此，Anthropic 的 Claude、xAI 的 Grok、Perplexity 都要争一个东西：iPhone 用户在 Settings 里选择的那个"默认 AI 槽位"。谁赢得这个槽位，谁就拿到了一个比 App Store 排名更深入的分发位置。

  同时，Apple 做了一个比 Extensions 更聪明的事：用 $10亿/年把 Gemini 锁定为 Siri 云端核心。这两件事并存说明：Apple 清楚自己不打算在模型能力上竞争，但它要控制"谁能接入、按什么规则接入"的规则定义权。Stripe 不构建支付网络，它定义支付 API 规范。Apple 不构建 AI，它定义 AI 进入最私密个人设备的入口。

  对于 AI 产品团队来说：这是一个战略选择时刻——是把资源押注在自己的 App 分发，还是争夺 iOS 27 Extensions 的集成位置？后者的竞争对手少、但准入门槛（必须已有 iOS 应用）明确。

- **Resonance hook**: 明天 WWDC 2026 开幕，Tim Cook 最后一次以 CEO 身份登台。Apple 要公布的核心之一：iOS 27 Extensions——用户可以在 Settings 里把 Siri 的大脑换成 Claude、Gemini、Grok 或 Perplexity。ChatGPT 自2024年12月起作为 iPhone 唯一第三方 AI 的独家地位，明天正式终结。14亿台 iPhone，Apple 不做 AI 公司，它做 AI 操作系统——不在乎谁赢，只需要赢家经过它。
- **Recommended priority**: high

---

## Candidate 2: arXiv 新论文《软件工程的终结》——代码从"决策逻辑的载体"变成"LLM 推理循环的即用即抛工具"，Software → SaaS → AaaS 第三次范式跃迁（June 4）

- **Event**: 2026年6月4日，Zhenfeng Cao（来自灵犀智投 Lingxi Intelligent Investment）在 arXiv 提交论文《The End of Software Engineering: How AI Agents Are Fundamentally Restructuring the Software Paradigm》（arXiv:2606.05608）。核心论点：过去半个世纪，软件工程的基本前提是"人类工程师将决策逻辑编码进静态代码"。AI Agent 系统的出现（以 LLM 为主推理引擎、动态生成并丢弃代码）从根本上重构了这一范式——在 Agentic 系统里，**代码不再是决策逻辑的载体，而是 LLM 驱动的推理循环中即用即抛的工具**。论文形式化地区分了两个世界：传统软件（code = decision logic carrier）vs. Agentic 系统（code = ephemeral tooling for LLM reasoning loop）。历史弧线：**授权软件 → SaaS → AaaS（Agent-as-a-Service）**——每次迁移都将复杂度从用户身上移走。AaaS 的核心定义：agent 通过标准化 API 暴露，客户端系统动态发现并调用；agent 不提供静态功能，而是提供**自主推理能力**——解释目标、规划行动、适应上下文。
- **Source**: https://arxiv.org/abs/2606.05608 | https://arxiv.org/html/2606.05608
- **Timeliness**: 3天前（2026年6月4日，arXiv 提交日）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 这篇论文的重要性不在于标题有多耸动，而在于它精确命名了一个正在发生但还没有人说清楚的结构性转变。

  在 SaaS 时代，软件的竞争护城河是**功能累积**：你的产品功能越多，用户学习成本越高，切换成本越大。这就是为什么 Notion 、Figma 能持续扩张功能边界——功能就是资产。

  在 AaaS 时代，这个逻辑断了。如果代码是即用即抛的，那"有多少功能"就不再是护城河。Agent 能随时生成需要的函数、调用需要的 API、组装需要的工作流。AaaS 的竞争护城河变成了另外两件事：**推理质量**（agent 在特定 domain 的判断准确性）和**上下文深度**（agent 对这个客户累积的理解程度）。你可以复制功能；你无法复制六个月积累的客户上下文。

  这对 B2B AI 产品有直接的战略含义：传统 SaaS 的"功能 roadmap"框架在 AaaS 时代是错误的问题框架。正确的问题不是"下个季度要加什么功能"，而是"我的 agent 在什么维度上比竞争对手更懂这个客户"。数据飞轮、上下文积累、推理专业化——这些才是 AaaS 公司的护城河建造方式。

  授权软件 → SaaS 的跃迁花了20年。SaaS → AaaS 的跃迁正在发生，但中文 AI 圈对 AaaS 作为独立商业模式范畴的讨论几乎缺席。这篇论文提供了一个可以直接引用的框架。

- **Resonance hook**: 6月4日，arXiv 上一篇论文的标题是《软件工程的终结》。它的核心论点不是"AI 会取代程序员"，而是一个更精确的结构性声明：在 Agent 系统里，代码从"决策逻辑的载体"变成了"LLM 推理循环的即用即抛工具"。软件工程从此不再是把决策逻辑编进代码——而是把目标和上下文交给 agent，让 agent 自己生成并丢弃代码。这是第三次范式跃迁：授权软件 → SaaS → AaaS。每次跃迁都把复杂度从用户身上移走了。这次，把"学软件"这件事本身移走了。
- **Recommended priority**: high

---

## Candidate 3: Anthropic 将 Claude Mythos 扩展至全球15国150家关键基础设施机构——一个 Anthropic 不卖给你的最强模型，自4月起已找到10,000+高危漏洞（June 2）

- **Event**: 2026年6月2日，Anthropic 宣布将 **Project Glasswing** 扩展至全球超过 **15个国家的150家新机构**，新增覆盖电力、水务、医疗、通信和硬件等此前第一批次未覆盖的行业。Project Glasswing 的核心工具是 **Claude Mythos Preview**——Anthropic 尚未发布、也明确表示**不会面向公众发布**的最强旗舰模型。关键能力描述（Anthropic 原话）："Claude Mythos 在发现和利用软件漏洞方面，能够超越除最顶级人类黑客之外的所有人"（"surpass all but the most skilled humans at finding and exploiting software vulnerabilities"）。量化进展：自2026年4月 Glasswing 正式启动以来，Claude Mythos Preview 已找到超过 **10,000个高危或严重级别的软件漏洞**——约100个/天。战略声明：Anthropic 预计在6至12个月内，其他前沿 AI 实验室将拥有 Mythos 级别的模型能力，"但可能在没有足够防止滥用的安全护栏的情况下发布"。TechCrunch（June 2）、CNBC（June 2）、CyberScoop、Help Net Security（June 3）均独立确认。
- **Source**: https://www.anthropic.com/news/expanding-project-glasswing | https://techcrunch.com/2026/06/02/anthropic-scales-claude-mythos-to-critical-infrastructure-in-15-countries/ | https://www.cnbc.com/2026/06/02/anthropic-mythos-ai-project-glasswing.html | https://cyberscoop.com/anthropic-project-glasswing-expansion-critical-infrastructure-claude-mythos/ | https://www.helpnetsecurity.com/2026/06/03/anthropic-project-glasswing-expansion/
- **Timeliness**: 5天前（2026年6月2日，Anthropic 官方扩展公告；多方来源6月2-3日确认）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: Anthropic 正在运营一家隐形安全公司，而这家公司的核心"员工"是一个不卖给任何人的 AI。

  Claude Mythos 创造了一个在 AI 行业里几乎不存在的品类：**能力最强、但不对外销售的 AI**。它不是 API，不是订阅产品，不是 Claude 4 的延伸——它是一个只被用于特定任务、受到严格接入控制的"能力储备"。Anthropic 的判断是：这个级别的能力如果商业化，风险不可控；但如果封存不用，竞争对手会做出同等能力的模型然后无控制地发布。

  这是一种新型商业模式逻辑：**用最强能力做最不赚钱的事，来定义最高标准**。10,000个漏洞不是收入，是证据——证明这个模型级别确实存在，证明 Anthropic 是唯一一个有能力做这件事同时有节制不全面发布的实验室。这在"6到12个月后其他实验室会有同等能力"的叙事框架下，创造了一个窗口期：在别人赶上来之前，Anthropic 用这个优势建立关键基础设施的信任关系。

  对于做 AI 产品的人，这里有一个结构性启示：不是所有能力都适合被商业化。最强的能力往往比次强的能力有更窄的合适部署场景。Glasswing 的模型是：能力 × 严格接入控制 × 可量化安全贡献 = 一种新形态的企业 AI 合同。这不是 SaaS 定价，不是 API token 计费，是"我们帮你找漏洞，每个高危漏洞的社会价值远超每月订阅费"。

- **Resonance hook**: 2026年6月2日，Anthropic 把 Project Glasswing 扩到全球15个国家的150家机构。使用的模型是 Claude Mythos——Anthropic 最强的模型，你买不到也用不了。它从4月开始扫描电网、医院和水务系统，已找到10,000+高危漏洞。约100个/天。Anthropic 说，Mythos 级别的能力在发现和利用软件漏洞上"超越除最顶级人类黑客之外的所有人"——然后明确说：这个模型不会公开发布。不是不够强，是太强了。
- **Recommended priority**: medium

---

## Scan summary

**Sources scanned**:
- Bloomberg（Mark Gurman June 5 WWDC 2026 完整预览；$1B Gemini deal 细节；Tim Cook last keynote confirmed）
- TechTimes（June 6，WWDC 2026 开幕确认；Gemini-powered Siri 细节）
- MacRumors（WWDC 2026 what-to-expect guide，Extensions framework 技术细节；iOS 27 third-party AI chatbots，May 5）
- Let's Data Science（iOS 27 Extensions：Claude, Grok integration confirmed）
- CNBC（January 12，Apple-Google Gemini deal 首次官方确认）
- arXiv（arXiv:2606.05608，June 4 提交，Zhenfeng Cao，The End of Software Engineering；HTML + abstract 原文直接读取）
- Anthropic 官方（anthropic.com/news/expanding-project-glasswing，June 2）
- TechCrunch（June 2，Anthropic scales Claude Mythos to 15+ countries，独立确认）
- CNBC（June 2，Anthropic Mythos Project Glasswing，关键数字确认）
- CyberScoop + Help Net Security（June 2-3，Glasswing expansion 150 organizations 细节）
- Sequoia AI Ascent 2026（April，Karpathy/Demis/Jim Fan，超30天窗口排除）
- Gemini Spark（May 19，Google I/O 2026，19天前，超7天窗口排除）
- BYD humanoid robots "Yao-Shun-Yu"（June 3-4，TechNode + Pandaily + CnEVPost；Zico 信息差评估：中文社交媒体已大面积覆盖，排除）
- Google Gemini 3.5 Flash（June 2026，DeepMind Contextual AI 招聘 $80-90M，无独立 June 1-7 精确事件锚点，排除）
- YC Blog（June 2026，无确认 June 1-7 新 AI 深度文章，排除）
- Swyx / Latent Space（January 2026 roadmap；AIE Europe Debrief 2026，无独立 June 1-7 事件锚点，排除）
- Anthropic "When AI Builds Itself"（June 4，已在 2026-06-06 candidates 中选定，排除）
- Microsoft MAI-Thinking-1（June 2，已在 2026-06-06 candidates 中完整覆盖，排除）
- ChatGPT Dreaming V3（June 4，已在 2026-06-06 candidates 中覆盖，排除）
- ChatGPT 转化广告（June 5，已在 2026-06-05 candidates 中选定，排除）
- GitHub Trending AI（OSSInsight + Agent of the Day June 2，无 June 4-7 独立爆发事件锚点，排除）

**Total signals found**: 约28个评估

**Why these 3**:

- **Candidate 1（Apple WWDC 2026 / iOS 27 Extensions，June 5-6）**：时效最强（1天前），Bloomberg Gurman + TechTimes June 6 + MacRumors + Let's Data Science 四方来源确认；AI 产品战略柱：过去3天 SELECTED 覆盖了 ChatGPT 广告双激励结构（June 5）、Anthropic Partner Network 分发锁定、MAI-Thinking-1 微软自主模型栈——今天角度完全不重叠："Apple 放弃成为 AI 公司、改为运营 AI 操作系统"是平台层战略的新结构信号；ChatGPT 失去 iOS 独家地位 + 14亿 iPhone 成为 AI 中立平台是可验证的市场影响；iOS 27 Extensions 技术机制（App Store 接入 + Settings 一键切换）是具体的竞争规则变化；中文媒体会报道"Apple 用 Google AI 改造 Siri"但不会分析"Apple 用 Extensions 框架把 AI 竞争内化为自己的平台竞争"；HIGH 优先级。

- **Candidate 2（arXiv 2606.05608 "End of Software Engineering"，June 4）**：时效3天，arXiv 原文直接可验证；Agent 经济柱：过去3天 SELECTED 未覆盖 Agent 经济主题（近期选题集中在监管/商业模式/安全）——今天是该柱首次入选；"代码从决策逻辑载体变为 LLM 推理循环的即用即抛工具"是 Agent 经济底层逻辑的精确重新表述，Zico 在 Confluence 里的 Agent Economy 框架（"Make something agents want"）有直接对照；AaaS（Agent-as-a-Service）作为独立范畴的命名在中文 AI 讨论中几乎缺席；SaaS → AaaS 护城河转变（功能积累 → 推理质量 + 上下文深度）是 B2B AI 产品经理的直接工具；HIGH 优先级（arXiv 论文类通常 medium，但 Agent 经济柱长期缺席且本文论点直接可转化为内容，提升至 high）。

- **Candidate 3（Anthropic Project Glasswing / Claude Mythos，June 2）**：时效5天（7天窗口内），Anthropic 官方 + TechCrunch + CNBC + CyberScoop 四方来源确认；深层AI思考柱：昨日选定主题为"When AI Builds Itself"（递归自我改进 / 代码自动化）——今天角度不重叠："能力最强的 AI 不商业化，仅用于关键基础设施防御"是 AI 能力分层和部署伦理的新结构问题；10,000个漏洞/每天~100个是可量化的部署结果；"能力 × 严格接入控制 × 可量化安全贡献"的新型 AI 商业模式框架中文媒体无覆盖；Anthropic 连续两天入选存在集中度风险，但本事件在产品战略和能力伦理两个维度上与昨日选题无重叠；MEDIUM 优先级。
