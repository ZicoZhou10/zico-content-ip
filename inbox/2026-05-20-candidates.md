---
date: 2026-05-20
status: pending_selection
---

# Today's Candidates

## Candidate 1: Karpathy 加入 Anthropic（May 19）：曾说当今 AI Agent 是"slop"的人，现在用 Claude 来构建下一个 Claude

- **Event**: 2026年5月19日（昨天），Andrej Karpathy 在 X 上宣布加入 Anthropic："I've joined Anthropic. I think the next few years at the frontier of LLMs will be especially formative."。具体职能：在 pre-training 团队 lead **Nick Joseph** 旗下工作，同时立刻组建一个新小组，使命是**用 Claude 加速 Claude 自身的预训练研究**（use Claude to speed up the research that produces the next Claude）。背景：Karpathy 是 OpenAI 联合创始人之一，之后去 Tesla 领导 FSD/Autopilot AI 团队（2017-2022），2022年回 OpenAI 一年，2024年离职创办 **Eureka Labs**（教育 AI 初创公司）。**他在2025年10月 Dwarkesh Patel 播客上明确说过：frontier 模型产出的大量 Agent 输出是"slop"，并主张应该想"十年 Agent"，而不是"一年 Agent"。** Karpathy 是 "vibe coding" 概念的提出者。来源覆盖：Karpathy 本人 X 帖（May 19, https://x.com/karpathy/status/2056753169888334312）、TechCrunch（May 19）、Bloomberg（May 19）、CNBC（May 19）、Axios（May 19）、Gizmodo（May 19）、Fortune（May 19）。
- **Source**: https://x.com/karpathy/status/2056753169888334312 | https://techcrunch.com/2026/05/19/openai-co-founder-andrej-karpathy-joins-anthropics-pre-training-team/ | https://www.axios.com/2026/05/19/anthropic-openai-karpathy-andrej-claude | https://www.cnbc.com/2026/05/19/anthropic-hires-openai-cofounder-andrej-karpathy-former-tesla-ai-lead.html
- **Timeliness**: 1 day ago（2026年5月19日）
- **Topic pillar**: 组织形式变革 / 深层思考
- **Zico's angle**: 中文 AI 圈会把这件事报道成"Karpathy 从 OpenAI 跳槽 Anthropic，薪酬一定很高"或"Anthropic 在抢人才"。这个框架遗漏了最值得注意的结构。Karpathy 在2024年离开 OpenAI，不是去另一家大厂——是去创业（Eureka Labs，教育 AI）。AI 顶级研究者的标准叙事是"大厂→创业→独立"。Karpathy 的路径是"大厂→创业→**大厂**"，反向了。他选择放下自己的公司回到实验室，意味着他判断：当前阶段，预训练前沿（pre-training frontier）才是最值得投入的工作，产品和创业可以等。更值得分析的是他在 Anthropic 的具体任务：**用 Claude 来加速产出下一代 Claude 的研究**。这是一个递归自改进的研究范式——AI Agent 在训练循环里干掉部分研究员的工作，提出代码修改、运行实验、只保留通过验证的改进。Karpathy 之前在 autoresearch 项目里测试过：AI agent 在两天内跑了约700次实验，找到约20个可堆叠的改进，产出11%训练加速。他加入 Anthropic 的赌注是：把这套东西正式化为 Anthropic 的研究工作流。一个曾经公开说当今 Agent 是"slop"的人，现在的工作是用 Agent 来构建更好的 Agent。这不是打脸，是他一直说的"十年 Agent"在他自己身上开始兑现。对 AI 协作实践来说，Karpathy 这个角色是一个清晰信号：顶级 AI 研究的生产环节里，人类 researcher 开始被 AI Agent 部分替代，这不是科幻——是 Anthropic 正在运行的生产架构。
- **Resonance hook**: 2026年5月19日，Karpathy 宣布加入 Anthropic。他的职责：用 Claude 加速产出下一代 Claude 的研究。在此之前，他公开说过当今 AI Agent 的大量输出是"slop"，并主张应该想"十年 Agent"而不是"一年 Agent"。他在2024年离开 OpenAI 去创业，现在把自己的公司放下，回到实验室。AI 顶级研究者的路径通常是"大厂→创业→独立"——Karpathy 的路径反过来了。
- **Recommended priority**: high

---

## Candidate 2: OpenAI 把 ChatGPT 接进银行账户（May 15）：AI 进入个人金融，Plaid 成了 AI 与钱之间的管道

- **Event**: 2026年5月15日（5天前），OpenAI 正式发布 **ChatGPT 个人金融功能（Personal Finance）**，面向美国 **ChatGPT Pro** 订阅用户开放预览。核心功能：用户通过 **Plaid** 接口连接超过 **12,000 家金融机构**（包括 Schwab、Fidelity、Chase、Robinhood、American Express、Capital One），ChatGPT 可以读取账户余额、交易记录、投资持仓、债务和订阅费用。界面：侧边栏出现 "Finances" 选项，显示投资组合表现、消费分类、订阅清单、即将到期付款等 dashboard。ChatGPT **不能看到完整账户号码，不能转账、支付、下单、修改账户**——纯读取层。技术架构：OpenAI 与 Plaid 合作管理账户连接（Plaid 已是 Venmo、Coinbase、Robinhood 的金融数据基础设施）。断开连接后30天内 OpenAI 删除已同步数据。计划：近期支持 Intuit 集成（支持税务影响分析、信用卡批准概率预测）。背景：OpenAI 在2026年4月收购了个人理财初创公司 **Hiro** 的团队（Ribbit、General Catalyst、Restive 支持）。TechCrunch（5月15日）、OpenAI 官方博客（5月15日）、MacRumors（5月15日）、American Banker（5月17日）、Plaid 官方博客（5月17日）多方覆盖。
- **Source**: https://openai.com/index/personal-finance-chatgpt/ | https://techcrunch.com/2026/05/15/openai-launches-chatgpt-for-personal-finance-will-let-you-connect-bank-accounts/ | https://www.macrumors.com/2026/05/15/chatgpt-personal-finance/ | https://plaid.com/blog/chatgpt-personal-finance-plaid/
- **Timeliness**: 5 days ago（2026年5月15日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 中文 AI 媒体会报道 "ChatGPT 现在可以帮你管钱了"。这个叙事跳过了一个更值得分析的产品战略问题：**谁拿到了个人金融的聚合器位置？** 个人金融聚合器的历史：Mint 做了16年被 Intuit 收购后在2024年3月关闭；Personal Capital 被 Empower 收购；YNAB 至今是利基产品。2024年到2026年之间这个品类实际上是一片空白。现在 OpenAI 用 Plaid 的数据管道，把 ChatGPT 的 800M+ 用户基础接进了这个空白里。重要的不是"ChatGPT 能帮你分析消费"，而是 **OpenAI 选择用"读取但不执行"的产品架构来切入高监管的金融领域**。ChatGPT 现在只能看，不能动。这是 AI 进入强监管高风险垂直行业的标准进入策略：先做信息层，再做决策层，最后做执行层。每一层都比上一层需要更多监管信任和用户信任。下一步显然是：AI 开始主动提建议（"你这笔订阅3年没用，建议取消"）→再下一步是：AI 主动执行（"我已经帮你取消了，退款已处理"）。Plaid 在这个结构里的位置也值得注意：Plaid 不是 OpenAI 的竞争对手，是它的分发管道——就像 Dell 是 Codex 进入企业数据中心的管道一样。在高监管行业，数据基础设施商（Plaid）和 AI 层（OpenAI）的关系会越来越像云计算时代的 AWS 和 SaaS 应用层——前者提供接口和合规，后者提供智能。OpenAI 收购 Hiro 团队后一个月内就发布产品，这个速度也值得记住：**AI 原生产品的开发周期已经不是18个月，是4-8周**。
- **Resonance hook**: 2026年5月15日，OpenAI 推出 ChatGPT 个人金融功能，通过 Plaid 接入超过12,000家金融机构。ChatGPT 可以看你的账户余额、交易记录、投资持仓，但不能动一分钱。Mint 2024年关闭后，个人金融聚合器的位置空了两年——OpenAI 用800M+用户基础和Plaid的数据管道填进来了。"读取但不执行"是 AI 进入强监管行业的标准第一步。下一步已经很清楚。
- **Recommended priority**: high

---

## Candidate 3: Isomorphic Labs 融资 $21 亿（May 12）：DeepMind 的药物设计 AI 要在2026年底把第一个分子送进临床试验

- **Event**: 2026年5月12日（8天前），Isomorphic Labs 宣布完成 **B 轮融资 $21 亿**，由 Thrive Capital 领投，跟投方包括 Alphabet、Google Ventures、CapitalG、新加坡淡马锡（Temasek）、英国国家主权 AI 基金（UK Sovereign AI Fund）。Isomorphic Labs CEO 是 **Demis Hassabis**，Google DeepMind 联席 CEO，AlphaFold 主导者，2024年诺贝尔化学奖得主（与 John Jumper 共同获奖）。公司背景：2021年从 Google DeepMind 拆分出来的独立 AI 药物设计公司，目标是用 AI 从头（de novo）设计全新药物分子——不只是预测蛋白质结构（AlphaFold 做的），而是针对已知的蛋白质靶点设计全新的可成药分子。核心产品：**IsoDDE（Isomorphic Drug Design Engine）**，AI 药物设计引擎。资金用途：加速 IsoDDE 开发，扩大伦敦、剑桥（马萨诸塞）、洛桑三地研究运营，**争取在2026年底将 AI 设计的药物推进人类临床试验**。Hassabis 公开表态："这是全球顶级投资人对我们 AI 优先药物设计方法的巨大信任投票。"来源：Tech.eu（5月13日）、PR Newswire（5月12日官方公告）、Yahoo Finance（5月13日）、The AI Insider（5月13日）。
- **Source**: https://tech.eu/2026/05/13/isomorphic-labs-lands-2-1bn-investment/ | https://www.prnewswire.com/news-releases/isomorphic-labs-secures-2-1-billion-funding-to-scale-its-ai-drug-design-engine-302769674.html | https://finance.yahoo.com/sectors/healthcare/articles/isomorphic-labs-raises-2-1-164235060.html | https://theaiinsider.tech/2026/05/13/isomorphic-labs-announces-2-1b-funding-to-scale-its-ai-drug-design-engine/
- **Timeliness**: 8 days ago（2026年5月12日，窗口边缘）
- **Topic pillar**: 深层思考 / AI 产品战略
- **Zico's angle**: 中文媒体会报道 "Demis Hassabis 的新公司融了21亿美元，AI 制药又热了"。这个叙事框架把这件事处理成了融资新闻，跳过了一个更根本的范式问题：**AlphaFold 做的是预测，IsoDDE 做的是设计——这是两种完全不同的 AI 能力**。AlphaFold 是给定蛋白质序列，预测它的3D结构。这是一个"理解"任务——读入，输出解释。IsoDDE 是给定一个蛋白质靶点（想要抑制或激活的结构），让 AI 设计一个能结合这个靶点的全新化学分子，这个分子之前从未在自然界存在过，也没有在任何药物数据库里出现过。这是一个"生成+推理"任务——给定约束，输出从未存在过的答案。从 AI 能力的角度，这是第一次在药物发现领域真正意义上的"AI 作为科学家"而非"AI 作为科研工具"。Isomorphic Labs 在2026年底把 AI 设计的分子送进临床试验，意味着从 AI 输出到人类可以测试的治疗候选物的整个周期，将首次被证明是可行的。这个里程碑如果实现，对 AI 在高风险高专业领域的信任建立有直接溢出效应——不只是生物制药，而是"AI Agent 在专业领域的判断值得信赖"这个命题。$21 亿的资本结构里有一个细节值得注意：**英国国家主权 AI 基金（UK Sovereign AI Fund）是新投资人之一**。主权基金进入 AI 药物设计，说明各国政府已经开始把 AI+生物科学的投资视为国家战略资产，而不只是私人资本的玩具。中文 AI 圈几乎没有人从"主权 AI 基金布局 Physical AI 前沿"的视角来分析这笔融资。
- **Resonance hook**: 2026年5月12日，Isomorphic Labs（Google DeepMind 拆分出的 AI 药物公司，CEO 是 AlphaFold 创造者、2024年诺贝尔化学奖得主 Demis Hassabis）完成 B 轮 $21 亿融资，目标：2026年底把 AI 设计的全新药物分子送进人类临床试验。AlphaFold 预测蛋白质结构——IsoDDE 设计从未存在过的药物分子。从"AI 理解生物学"到"AI 自主发现药物"，这一步很大。如果年底前实现，这是 AI Agent 在高风险专业领域独立决策的第一个临床验证。
- **Recommended priority**: medium

---

## Scan summary

- **Sources scanned**: Karpathy X 本人帖子（May 19）、TechCrunch（May 19 Karpathy+Anthropic）、Bloomberg（May 19）、CNBC（May 19）、Axios（May 19）、Gizmodo（May 19）、Fortune（May 19）、The New Stack（May 19）、TechTimes（May 19 Karpathy slop quote）、The Algorithmic Bridge（May 19 Karpathy深度分析）；OpenAI 官方博客（May 15 ChatGPT Personal Finance）、TechCrunch（May 15 ChatGPT finance bank accounts）、MacRumors（May 15）、Plaid 官方博客（May 17 ChatGPT+Plaid合作分析）、American Banker（May 17）、gHacks（May 18）、Dataconomy（May 18）、how2shout（May 15）；Isomorphic Labs 官方公告 PR Newswire（May 12）、Tech.eu（May 13）、Yahoo Finance（May 13）、The AI Insider（May 13）、Analytics Drift（May 13）、Greek City Times（May 15）；Google I/O 2026 Day 2 Developer Keynote（May 19-20）—Google Antigravity 2.0（CLI+SDK+Managed Agents+Enterprise）— 排除（Google I/O 已在5月19日 candidates Candidate 1 覆盖，同一事件不同侧面）；Google Search Information Agents（background monitoring + push notifications）— 同属 Google I/O 2026，排除；Karpathy autoresearch GitHub（March 2026，700实验/2天，11%训练加速）作为背景支撑；Jim Fan May 2026 X/LinkedIn：最新独立信号为 April 2026 AI Ascent Sequoia talk（April 20，已在5月17日 candidates 排除名单内，超20天窗口）；Demis Hassabis X/Twitter：无独立5月15日后新帖；OpenAI DOE collaboration（February 2026 MOU，超30天窗口）；StanChart CEO "lower-value human capital" 替换声明（May 19, Staffing Industry Analysts）— 企业人力资源角度有一定组织形式变革契合度，但叙事过于宏观、无具体可追溯数据锚点，弱于已选3候选；GitHub Trending（OpenHuman、Hermes Agent 153k stars、OpenClaw 372k stars、awesome-ai-agents-2026 汇编仓库）— 无独立时效性事件锚点超越已选候选；arXiv（2506.00320 Dyna-Think：Synergizing Reasoning, Acting, and World Model Simulation — June 2026 提交，超出搜索窗口；2604.22748 Agentic World Modeling — April 2026，25+天，超7天窗口；5月15-20日无新突破性论文超越已选候选）

- **Total signals found**: 18 evaluated

- **Why these 3**:
  - **Candidate 1（Karpathy → Anthropic）**：时效最强（1天，May 19），Karpathy 本人 X 帖 + TechCrunch + Bloomberg + CNBC + Axios 五方确认，无任何近期 candidates 文件覆盖；组织形式变革柱：5月17-19日覆盖了 PwC 30,000人、OpenAI Codex Mobile 异步监督、Google I/O OS层，未覆盖"顶级 AI 研究者路径反向"这个组织形式信号；"曾说 Agent 是 slop 的人现在用 Agent 构建 Claude"是极强的反直觉叙事钩子；"Claude→builds→next Claude"递归研究范式在中文 AI 媒体没有分析；Zico 的 AI 协作实践视角（AI 在研究工作流中替代人类研究员）有直接内容产权关联。
  - **Candidate 2（ChatGPT Personal Finance）**：时效5天（May 15），OpenAI 官方博客 + TechCrunch + MacRumors + Plaid 博客多方确认；AI 产品战略柱在5月17-19日覆盖的是 Codex Mobile（异步监督）、Google I/O 平台战略、OpenAI+Dell 企业部署——个人金融垂直完全未覆盖；"Mint 关闭后空白2年→OpenAI 填入"这个聚合器位置叙事在中文媒体完全缺失；Plaid 作为 AI+金融的数据管道分析角度（类比 Dell 之于 Codex on-prem）信息增量高；"读取但不执行"的进入策略分析对 Zico 受众做 B2C AI 产品有直接参考价值；OpenAI 收购 Hiro 团队后一个月发布产品这个 velocity 数据点可独立验证。
  - **Candidate 3（Isomorphic Labs $2.1B）**：时效8天（May 12，窗口边缘但无近期覆盖），PR Newswire 官方公告 + Tech.eu + Yahoo Finance 确认；深层思考柱：5月18日覆盖 Anthropic "2028"政策报告，5月19日覆盖 WAMs paper，今日候选角度是"AI 从预测到设计"的范式跨越 + "主权 AI 基金进入 Physical AI 前沿"——不重叠；"AlphaFold 理解→IsoDDE 设计从未存在过的分子"是最清晰的"AI 作为科学家非工具"叙事，配合 Zico 的 AI 新物种框架；UK Sovereign AI Fund 参与投资是可独立验证的国家战略信号，中文媒体完全未分析；候选相对偏弱（时效8天，中文受众与生物制药距离偏远），但"2026年底 AI 设计药物进临床试验"是一个极具未来感的可验证里程碑，共鸣潜力超越垂直圈层。

---

**Excluded signals**:
- Google I/O 2026 Antigravity 2.0 / Search Information Agents / Gemini Spark（May 19）：同一事件（Google I/O 2026）已在5月19日 candidates Candidate 1 覆盖，避免同事件重复
- Jim Fan AI Ascent Sequoia talk（April 20, 2026）：已在5月17日 candidates 排除名单，超20天窗口
- OpenAI Department of Energy MOU（February 2026）：超30天窗口
- Karpathy autoresearch（March 2026）：超30天窗口，用作 Candidate 1 背景支撑而非独立选题
- StanChart CEO "lower-value human capital"（May 19）：组织形式变革契合，但无具体量化锚点，叙事过于宏观，弱于 Candidate 1
- GitHub Trending（OpenHuman、Hermes Agent 153k stars、OpenClaw 372k stars）：无独立时效性事件锚点超越已选候选；OpenHuman 已在5月18日排除
- arXiv 2506.00320 Dyna-Think（June 2026 提交，超窗口）；arXiv 2604.22748 Agentic World Modeling（April 2026，超7天）
- Anthropic Code with Claude London event（May 20-21，今明两天进行中）：行业活动而非产品/研究发布，缺乏独立事件锚点
