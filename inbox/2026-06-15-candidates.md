---
date: 2026-06-15
status: written
selected: candidate 1 → drafts/046-pricing-split-xhs.md
---

# Today's Candidates

## Candidate 1: Anthropic 今天起拆分计费——Claude Agent SDK 与对话额度正式分家，Pro 每月仅 $20 Agent 信用，用完即停（June 15）

- **Event**: 2026年6月15日（今天），Anthropic 正式执行 Claude 订阅计费结构调整，Agent SDK 程序化使用额度从 Pro/Max 订阅额度中完全分离，独立计为月度信用池。具体数字：Claude Pro $20/月 Agent SDK 信用、Claude Max 5x $100/月、Claude Max 20x $200/月。覆盖范围：Claude Agent SDK（`claude -p`）、Claude Code GitHub Actions、所有基于 Agent SDK 构建的第三方应用。计费方式：按标准 API token 费率计费，每月重置，无滚存；超出额度后自动化停止运行，除非启用溢出计费。TechTimes 于6月2日率先报道（标题：《Anthropic Ends Subscription Subsidy for Agents June 15: Credit Pool Replaces Flat-Rate Access》）；The New Stack、ChatForest、VantagePoint、CodersEra 等开发者媒体发布详细操作指南。
- **Source**: https://thenewstack.io/anthropic-agent-sdk-credits/ | https://www.techtimes.com/articles/317625/20260602/anthropic-ends-subscription-subsidy-agents-june-15-credit-pool-replaces-flat-rate-access.htm | https://chatforest.com/reviews/anthropic-claude-agent-sdk-billing-split-june-15-2026-credit-pool-developer-guide/ | https://vantagepoint.io/blog/ai/claude-agent-sdk-billing-change-june-15 | https://codersera.com/blog/anthropic-june-2026-billing-change-claude-code/
- **Timeliness**: 今天（2026年6月15日正式生效；TechTimes 2026年6月2日首报）
- **Topic pillar**: AI协作实践
- **Zico's angle**: Anthropic 今天做的事，和 GitHub 6月1日做的事是同一件事，只是在不同的层上。

  GitHub 把代码补全和 Copilot Workspace 分开计费——你让 AI 帮你打字，免费；你让 AI 替你干活，按量收费。Anthropic 把对话使用和 Agent SDK 分开计费——你用 Claude 聊天，消耗订阅额度；你用 Agent SDK 程序化调用 Claude，消耗独立信用池。

  两周之内，两个主流 AI 平台完成了同一个价格拆分，在工具层（GitHub）和模型层（Anthropic）各自画出了"AI 助手"和"AI 代理"的边界线。这不是巧合，是产品战略的收敛。

  $20/月 的 Agent SDK 信用是一个很具体的信号：这不是让你大量使用的额度，是让你感受到计费边界在哪里的设计。按 Claude Haiku 4.5 的 API 费率，$20 大约可以处理 2000 万个输入 tokens——听起来很多，但一个复杂的 multi-agent 工作流跑一次可能消耗数十万 tokens，认真做自动化的开发者几天就能耗尽一个月的信用。这个设计的逻辑是：严肃的 Agent 部署需要企业 API 合同，不是 $20/月订阅套餐。Anthropic 在用价格把两类用户分类：对话用户留在订阅里，Agent 开发者推向 API。

  对正在用 Claude Code 做开发或用 Agent SDK 构建自动化的人：今天开始你的成本结构不同了。这不是涨价，是结构重新定义。

- **Resonance hook**: 今天（June 15），如果你有 Claude Pro，你的 Agent SDK 使用额度从今天开始单独计算：每月 $20 信用，独立于你的对话额度，用完停止。2周前 GitHub 把 Copilot 代码补全（免费）和 Workspace 任务（按量收费）分开。今天 Anthropic 把订阅对话和 Agent SDK 程序化调用分开。模型层和工具层同步完成了同一个拆分：AI 助手和 AI 代理，从今天起是两种不同经济学的产品。
- **Recommended priority**: high

---

## Candidate 2: LiteLLM CVSS 10.0 被 CISA 列为在野利用漏洞——无需登录即可 RCE，CrewAI、DSPy 等 Agent 框架的模型路由层正被活跃攻击（June 8-9）

- **Event**: 2026年6月8日，美国 CISA 将 CVE-2026-42271 加入已知被利用漏洞（KEV）目录，确认该漏洞已在野外被真实攻击者积极利用。CVE-2026-42271 存在于 BerriAI 的开源 AI 网关 LiteLLM（被 CrewAI、DSPy、AutoGen 等主流多智能体框架用作默认模型路由层），CVSS 评分 8.7（命令注入）。2026年6月9日，Horizon3.ai 安全团队披露完整漏洞利用链：CVE-2026-42271 与 CVE-2026-48710（Starlette HTTP 框架"BadHost" host header 验证绕过，CVSS 6.5）组合，最终达成 **CVSS 10.0 满分、无认证远程代码执行（RCE）**——攻击者无需任何 API key 或事先访问权限。攻击面：LiteLLM 的 `/mcp-rest/test/connection` 端点接受 `command`/`args`/`env` 字段并作为子进程直接执行，BadHost 绕过所有身份验证。成功利用后果：主机任意命令执行、窃取 LiteLLM 代理的所有 LLM 供应商 API 密钥（OpenAI、Anthropic、Google 等）、横向移动进入全部下游 Agent 工作流。修复：CVE-2026-48710 修复于 Starlette v1.0.1；CVE-2026-42271 修复于 LiteLLM **v1.83.7+**。The Hacker News（June 9）、HelpNet Security（June 9）、SOCRadar、Vulert、CybelAngel、Rescana 多方技术分析确认。
- **Source**: https://thehackernews.com/2026/06/litellm-flaw-cve-2026-42271-exploited.html | https://www.helpnetsecurity.com/2026/06/09/litellm-vulnerability-under-active-attack-cisa-warns-cve-2026-42271/ | https://www.rescana.com/post/active-exploitation-alert-cve-2026-42271-and-cve-2026-48710-unauthenticated-rce-in-litellm-ai-gateway-via-starlette-host | https://socradar.io/blog/cisa-kev-litellm-cve-2026-42271-check-point-cve-2026-50751/ | https://vulert.com/blog/litellm-cve-2026-42271-rce/ | https://cybelangel.com/blog/itellm-vulnerability-cve-2026-42271/
- **Timeliness**: 7天前（2026年6月8日 CISA KEV 加入；6月9日 The Hacker News + HelpNet Security + Horizon3.ai 详细披露）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: AI Agent 系统的基础设施层刚刚有了第一个 CISA KEV 级别的在野利用漏洞。这是一个架构信号，不只是一个安全告警。

  LiteLLM 是 Agent 框架里不起眼的那一层：它坐在 Agent 逻辑和 LLM API 之间，负责路由（把 CrewAI 的模型调用发给 OpenAI 还是 Anthropic）、负载均衡、重试、速率限制、成本追踪。因为它做的事情"透明"，大多数 Agent 开发者对它的安全姿态关注度极低——默认配置、默认端口、默认暴露。

  这次漏洞的攻击链设计揭示了 Agent 基础设施的一个结构性脆弱点：LiteLLM 的 MCP 配置端点（用于配置 MCP Server 的接入）接受 `command` 字段并执行——这本来是给管理员在内网测试 MCP 连接用的，但在互联网暴露的生产部署上，任何人都可以发送这个请求，加上 BadHost 绕过认证，等于把一个 `system("anything")` 接口开放到了公网。

  受损的不只是 LiteLLM 主机本身。LiteLLM 进程在内存里持有所有配置进来的 LLM 供应商 API 密钥——OpenAI、Anthropic、Azure、Google 的 key 都在那里。攻击者拿到 shell 之后，首先提取这些密钥，然后利用 LiteLLM 已建立的连接横向进入所有下游 Agent 工作流：客服 Agent、代码生成 Agent、数据处理 Agent——任何调用过 LiteLLM 的系统都在横向移动的射程内。

  AI 基础设施和传统软件基础设施的安全规律是一样的：你的系统有多少个对外暴露的有状态接口，就有多少个攻击入口。Agent 开发者在快速构建时把 LiteLLM 暴露在互联网上是常见操作，现在这个操作的代价变成了 CVSS 10.0 在野 RCE。这不是"AI 太危险了"的叙事，是"任何基础设施都需要在进入生产前做威胁建模"的工程常识，在 AI 系统上被重新验证了一次。

- **Resonance hook**: 6月8日，CISA 把 LiteLLM 的一个漏洞列入"已知被利用"目录。LiteLLM 是 CrewAI、DSPy、AutoGen 背后的模型路由层——你的 Agent 调用 GPT 或 Claude，大概率经过它。攻击链：BadHost 绕过认证 + MCP 配置端点命令注入 = 无登录、无 API key，拿到主机 shell，顺走所有 LLM 供应商的 API 密钥，横向进入所有 Agent 工作流。CVSS 10.0 满分。修复版本：LiteLLM v1.83.7+，Starlette v1.0.1+。AI Agent 中间件刚刚有了它的第一个 CISA KEV 在野利用漏洞。
- **Recommended priority**: high

---

## Candidate 3: EngineAI 深圳工厂每 15 分钟下线一台 T800 人形机器人——成立不到 3 年，开始万台级交付，全栈自研不依赖 NVIDIA 或 Boston Dynamics（May 29）

- **Event**: 2026年5月29日，深圳公司 **EngineAI Robotics**（工程师人工智能，2023年10月成立）正式开放深圳宏华岭 EngineAI 智能制造基地，首批 **T800 全尺寸人形机器人**（面向工业应用场景）从产线下线，开始批量交付。工厂规模：约 **12,000 平方米**，覆盖来料检测、组件装配测试、最终总装、出厂测试、批量发货、售后维护的完整闭环制造流程。生产速率：**每 15 分钟下线一台 T800**。交付目标：2026年实现"**万台级**"（10,000 单位规模）交付能力，全年计划交付 **4,000 至 5,000 台**。技术栈：核心机器人组件、运动控制算法、具身 AI 技术均为**全栈自主开发**，不依赖第三方机器人平台或授权技术（无 NVIDIA GR00T、无 Boston Dynamics 技术依赖）。消息来源：PR Newswire（May 29，官方新闻稿）、Interesting Engineering（"One T800 humanoid robot every 15 mins, ENGINEAI's new factory claims"）、Humanoids Daily（"EngineAI Joins the Manufacturing Race: One Humanoid Every 15 Minutes at New Shenzhen Base"）、New Atlas、RoboticsTomorrow。
- **Source**: https://www.prnewswire.com/news-releases/engineai-launches-shenzhen-intelligent-manufacturing-base-as-first-batch-of-t800-humanoid-robots-roll-off-the-production-line-to-begin-mass-delivery-302785384.html | https://interestingengineering.com/ai-robotics/china-engineai-humanoid-robot-factory | https://www.humanoidsdaily.com/news/engineai-joins-the-manufacturing-race-one-humanoid-every-15-minutes-at-new-shenzhen-base | https://newatlas.com/ai-humanoids/engineai-t800-humanoid/ | https://www.roboticstomorrow.com/news/2026/05/29/engineai-launches-shenzhen-intelligent-manufacturing-base-as-first-batch-of-t800-humanoid-robots-roll-off-the-production-line-to-begin-mass-delivery/26644/
- **Timeliness**: 17天前（2026年5月29日 PR Newswire + Interesting Engineering + Humanoids Daily 多方报道；在30天窗口内）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 过去几周物理 AI 的新闻大多数是资本事件——NEURA 拿 $14亿、Boston Dynamics 获 Google DeepMind 集成。EngineAI 的深圳工厂是不同类型的信号：出货事件。

  "15分钟一台"这个数字不是 benchmark，是产线节拍（takt time）——是制造业语言，不是 AI 研究语言。它意味着 EngineAI 已经解决了物理 AI 进入规模生产的第一道门：零部件标准化、装配工序可重复、出厂质量检验自动化。这三件事比"我们的机器人能做什么"难得多，因为它们必须在真实约束（成本、供应链、工人技能）下达成，不是在实验室里。

  全栈自研是这个故事里更深的一层含义。EngineAI 的运动控制和具身 AI 算法不依赖 NVIDIA GR00T 授权或 Boston Dynamics 的技术转让。在当前地缘政治环境下，这意味着：中国工业场景的人形机器人采购可以不经过西方 AI 芯片和机器人技术的供应链。4,000 台 T800 进入工业场景，等于向 4,000 个工业节点输出了一套独立于西方技术栈的具身 AI 运行实例。

  2026年的物理 AI 竞争格局不只是"谁的机器人更聪明"，还有"谁的机器人能按时出货"。Tesla Optimus 目标是2026年数万台；Figure AI、1X 等美国公司还在 pre-production 阶段；EngineAI 的工厂5月29日已经在出货了。在物理 AI 这条赛道上，制造能力是和模型能力同等重要的护城河。

- **Resonance hook**: 2026年5月29日，深圳，一家2023年10月成立的公司（EngineAI）开了一条产线，每15分钟下线一台T800全尺寸人形机器人。工厂12,000平方米，2026年计划交付4,000至5,000台，全栈自研——运动控制、关键组件、具身AI算法都是自己做的，不依赖NVIDIA或Boston Dynamics的技术授权。过去几周物理AI的新闻大多是融资（NEURA $14亿、Boston Dynamics接 Gemini）。深圳这条产线说的是另一件事：出货开始了。
- **Recommended priority**: medium

---

## Scan summary

- **Sources scanned**:
  - The New Stack（《Anthropic splits billing again: Agent SDK gets separate credit pools》，June 15 生效细节）
  - TechTimes（June 2，《Anthropic Ends Subscription Subsidy for Agents June 15》，首报）
  - ChatForest（《Anthropic's June 15 Billing Split: What Every Claude Agent Developer Needs to Know》，详细操作指南）
  - VantagePoint（《Claude Agent SDK Billing Splits June 15: What Teams Must Do》，企业影响分析）
  - CodersEra（《Anthropic's June 15 Billing Change: What Every Claude Code & Agent SDK User Must Do》）
  - Level Up Coding（《Anthropic Just Quietly Raised Claude Pro Bill》，用户影响分析）
  - DigitalApplied（《Claude Credit Overhaul 2026: What Changes on June 15》）
  - The Hacker News（June 9，《LiteLLM Flaw CVE-2026-42271 Exploited in the Wild, Chains to Unauthenticated RCE》，Horizon3.ai 完整利用链披露）
  - HelpNet Security（June 9，《LiteLLM vulnerability under active attack, CISA warns (CVE-2026-42271)》，CISA KEV 加入确认）
  - Rescana（《Active Exploitation Alert: CVE-2026-42271 and CVE-2026-48710》，双CVE攻击链技术细节）
  - SOCRadar（《CISA KEV Highlights LiteLLM RCE (CVE-2026-42271)》）
  - Vulert（《LiteLLM CVE-2026-42271 Exploited》，修复路径确认）
  - CybelAngel（《LiteLLM Vulnerability CVE-2026-42271: 7 Things to Know》）
  - KSEC Forum / DevLeap（The Hacker News 二次确认镜像）
  - PR Newswire（May 29，《EngineAI Launches Shenzhen Intelligent Manufacturing Base as First Batch of T800 Humanoid Robots Roll Off the Production Line to Begin Mass Delivery》，官方新闻稿）
  - Interesting Engineering（《One T800 humanoid robot every 15 mins, ENGINEAI's new factory claims》，产线速率独立核实）
  - Humanoids Daily（《EngineAI Joins the Manufacturing Race: One Humanoid Every 15 Minutes at New Shenzhen Base》）
  - New Atlas（《T800 humanoid robot mass production for industrial use》）
  - RoboticsTomorrow（EngineAI T800 技术规格 + 产能细节）
  - G7 Summit 2026 信号扫描（Euronews June 14 + TechPolicy.Press + Bloomberg June 12 确认 Altman/Amodei/Hassabis 出席；G7 June 15 首日开幕——暂无具体 AI 承诺产出，延迟至 June 16-17 后续扫描）
  - OpenAI S-1 SEC 机密提交（Yahoo Finance + Fortune June 8-9；已在 2026-06-09 candidates 全面覆盖，排除重复）
  - Apple Spatial Reframing WWDC（已在 2026-06-09 candidates 全面覆盖，排除重复）
  - Pentagon "Too Safe for War"（已在 2026-06-09 candidates 全面覆盖，排除重复）
  - Fable 5 静默降级（已在 2026-06-11 candidates 全面覆盖，排除重复）
  - Google Gemini CLI EOL（已在 2026-06-11 candidates 全面覆盖，排除重复）
  - Dario "Policy on the AI Exponential"（已在 2026-06-11 candidates 全面覆盖，排除重复）
  - NEURA Robotics + Tether $14亿（已在 2026-06-12 candidates 选定为 draft 043，排除重复）
  - Microsoft MAI + "Set Free"（已在 2026-06-12 candidates 覆盖，排除重复）
  - GitHub Copilot token billing（已在 2026-06-12 candidates 覆盖；今日 Candidate 1 Anthropic 同类计费拆分与之角度不重叠：一为工具层 June 1，一为模型提供商层 June 15，两者共同指向行业级的定价结构收敛，逻辑可并置但各有独立事件锚点）
  - G7 AI 三大 CEO 出席（已在 2026-06-13 candidates 选定为 draft 044，排除重复）
  - GitLab Agentic Era 重组（已在 2026-06-13 candidates 覆盖，排除重复）
  - AI CEO 联名致国会 DNA 筛查（已在 2026-06-13 candidates 覆盖，排除重复）
  - Fable 5 + Mythos 5 政府命令下线（已在 2026-06-14 candidates 选定为 draft 045，排除重复）
  - OpenAI 收购 Ona + Codex 异步化（已在 2026-06-14 candidates 覆盖，排除重复）
  - Ramp AI Index Anthropic 超 OpenAI（已在 2026-06-14 candidates 覆盖，排除重复）
  - MetaMask Agent Wallet（June 8，7天前；与 June 12 draft 043 NEURA+Tether 机器/代理钱包概念高度重叠，主题重复，排除）
  - NVIDIA DreamDojo（2026年2月20日发布，超30天，排除）
  - NVIDIA DreamZero（2026年初，超30天，排除）
  - Grok 5 预期发布（无确认 GA 日期锚点，排除）
  - Gemini 3.5 Pro（仍在 Vertex 限量预览，无已确认 GA 日期锚点，排除）
  - Boston Dynamics + Gemini Robotics ER 1.6（April 8，超30天，排除）
  - Nat Friedman "Entire" 平台（2026年2月/3月，超30天，排除）
  - ChatGPT "Dreaming" 记忆系统（June 4，已在 2026-06-06 candidates 覆盖，排除）
  - University of Toronto AI worm（June 2-4，已在 2026-06-11 HN 信号中注意到；Hacker News 时效窗口覆盖但深层 AI 思考柱 June 14 已选，且事件锚点 June 2-4 与今日窗口偏旧，排除）
  - Palo Alto Networks Prisma AIRS 3.0（RSAC 2026 March 23 发布，超30天，排除）

- **Total signals found**: 约45个评估

- **Why these 3**:

  - **Candidate 1（Anthropic Agent SDK 计费拆分，June 15）**：时效"今天"（正式生效），The New Stack + TechTimes + ChatForest + VantagePoint 等多方开发者媒体确认；AI协作实践柱：过去3天此柱完全未被选中（最近选用为 June 8 或更早）；今日角度独特：这是模型提供商层（Anthropic）和工具层（June 1 GitHub Copilot）在两周内同步完成"AI 助手 vs AI 代理"计费分离的第二个事件，形成行业级定价结构收敛的明确模式；$20/月 Agent SDK 信用的具体数字是可验证的；对正在用 Claude Code 或构建 Agent SDK 自动化的开发者有今天即生效的直接影响；中文开发者社区对这一计费变化几乎没有深度讨论；HIGH 优先级。

  - **Candidate 2（LiteLLM CVE-2026-42271 CISA KEV，June 8-9）**：时效7天，The Hacker News + HelpNet Security + CISA 官方 + Horizon3.ai + SOCRadar + Vulert + CybelAngel 七方来源确认；深层AI思考柱：过去3天此柱在 June 14 Fable 5 政府关闭（监管政治角度）中被覆盖——今天角度根本不同：这是 AI Agent 基础设施的第一个 CISA KEV 级主动利用漏洞，聚焦的是"Agent 中间件 = 新类别基础设施攻击面"的架构洞察，而非监管政治；CVSS 10.0 满分 + 无认证 RCE + LiteLLM 路由 CrewAI/DSPy/AutoGen 的架构位置，在中文 AI 开发者社区几乎没有任何报道（国内使用 LiteLLM 的开发者极多但对 CISA KEV 告警几乎无感知）；HIGH 优先级。

  - **Candidate 3（EngineAI T800 深圳工厂，May 29）**：时效17天（在30天窗口内），PR Newswire 官方新闻稿 + Interesting Engineering + Humanoids Daily + New Atlas + RoboticsTomorrow 五方来源确认；Agent 经济柱：过去3天此柱在 June 12 NEURA+Tether（欧洲机器人 + 加密支付轨道，金融层）中被覆盖——今日角度不重叠：这是中国物理 AI 的制造层信号（不是融资不是合作，是"出货"），全栈自研 + 地缘政治独立性 + 每15分钟一台的 takt time 数字，与 Zico 在做 3DGS/Physical AI 的一线视角直接共鸣；中文媒体覆盖集中在新闻稿转发层面，"takt time 作为物理 AI 竞争力的新维度"角度几乎缺失；MEDIUM 优先级（时效17天，略旧，但物理 AI 制造事件的信息密度支撑独立叙事）。
