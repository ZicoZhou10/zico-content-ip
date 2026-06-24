---
date: 2026-05-17
status: written
selected: candidate 2 → drafts/021-agent-metering-fork-xhs.md
---

# Today's Candidates

## Candidate 1: OpenAI Codex 进手机——异步 AI 编程监督模式正式到来，开发者变成"例外处理者"

- **Event**: 2026年5月14-15日，OpenAI 正式发布 **Codex Mobile**，将 Codex 编程 Agent 集成进 ChatGPT iOS 和 Android App，对所有 ChatGPT 计划（包括 Free 和 Go）全面开放 preview。工作原理：开发者在 Mac 端运行 Codex App → 手机扫 QR 码配对 → 此后 Codex 在 Mac 本地全速执行长任务，手机端实时查看进度、切换线程、审批 Agent 请求的关键动作（运行某命令、修改某文件、推进下一步）。敏感文件、凭证、本地权限全部保留在宿主机，不传手机。TechCrunch（5月14日）标题："OpenAI says Codex is coming to your phone"；MacRumors（5月15日）："OpenAI Brings Codex Coding Agent Controls to ChatGPT Mobile App"；CIOL（5月15日）、WinBuzzer（5月15日）同日覆盖。OpenAI 官方文档（openai.com/index/work-with-codex-from-anywhere）同步上线。竞争背景：Anthropic 早已在 Claude Code 中推出类似的 remote 功能，OpenAI 此次是正面跟进。
- **Source**: https://openai.com/index/work-with-codex-from-anywhere/ | https://techcrunch.com/2026/05/14/openai-says-codex-is-coming-to-your-phone/ | https://www.macrumors.com/2026/05/15/openai-brings-codex-chatgpt-mobile-app/ | https://www.ciol.com/generative-ai/openai-codex-mobile-remote-workflow-management-chatgpt-11837163
- **Timeliness**: 2-3 days ago（2026年5月14-15日）
- **Topic pillar**: AI 协作实践
- **Zico's angle**: 中文媒体会把这件事报道成"OpenAI 出了个新功能，以后可以在手机上写代码了"——这个叙事框架把方向搞反了。Codex Mobile 不是"手机写代码"，是**手机监督 AI 写代码**。开发者不需要盯着屏幕输入 prompt，而是在任何地方生活，等 Agent 跑几个小时后发消息说"我到了一个需要你判断的地方"，然后你掏出手机看一眼，点 Approve 或 Reject，继续生活。这是两种完全不同的人机关系：以前是人驱动、AI 执行；现在是 AI 默认运行、人负责例外路径。"异步监督"不是功能，是工作方式的结构变化。每当 AI Agent 需要执行一个它没被授权自主决定的动作，它就停下来等人。人的注意力成本从"持续输入"变成了"按需决策"。这个模式 OpenAI 在做，Anthropic 在做，Cursor 在做——它在整个行业同时出现，意味着它不是产品创新，是用户使用 AI 工具方式的结构性转移。对想认真用 AI 提效的人，这个转变有一个具体含义：你的工作流要从"我坐在那里和 AI 一来一往"，变成"我给 AI 一个任务，它跑，我只处理它处理不了的那几个决策点"。
- **Resonance hook**: OpenAI 5月14日把 Codex 编程 Agent 接进了 ChatGPT 手机 App。不是让你在手机上打代码——是让 Codex 在你的 Mac 上跑几个小时，遇到需要人判断的关键决策时，给你手机发通知，你点个 Approve，它继续跑。人不再是 AI 的驾驶员，人是 AI 的例外处理者。Anthropic Claude Code 先做，OpenAI 这周跟进——这个工作模式正在成为行业标准。
- **Recommended priority**: high

---

## Candidate 2: Anthropic 把 Agent SDK 单独计费——$20 Pro 订阅跑 Claude Agent 的时代，6月15日结束

- **Event**: 2026年5月13日，Anthropic 宣布重大计费结构调整，**2026年6月15日起生效**：Claude Agent SDK、`claude -p` 命令、Claude Code GitHub Actions、所有第三方 Agent 框架（OpenClaw、Conductor、Zed、Jean 等）将从现有订阅用量池**剥离**，移至独立的"Agent SDK Credit 池"，按 API 标准费率计费。各等级月度 Credit 额度：**Pro（$20/月）→ $20 credits；Max 5x（$100/月）→ $100 credits；Max 20x（$200/月）→ $200 credits**。Credits 不滚存，按 Anthropic API 标准费率扣减。**不受影响**：网页 Claude 对话、桌面/移动端交互、Claude Code 终端交互、Claude Cowork 继续沿用订阅用量限制。背景：2026年初，$20 Pro 订阅可通过 OpenClaw 等第三方 Agent 框架运行等价于数百美元 API 调用量的 Agent 工作负载（compute arbitrage）。Anthropic 先封锁第三方 Agent 访问，随后以此 Credit 方案重新开放。开发者社区实测：有效价格提升 **12x–175x**（取决于工作负载类型）。VentureBeat（5月13日）："Anthropic reinstates OpenClaw and third-party agent usage on Claude subscriptions — with a catch"；InfoWorld（5月13日）；The New Stack；MagnaCapax GitHub Gist（社区规范化参考，包含完整数学推导）。
- **Source**: https://venturebeat.com/technology/anthropic-reinstates-openclaw-and-third-party-agent-usage-on-claude-subscriptions-with-a-catch | https://www.infoworld.com/article/4171274/anthropic-puts-claude-agents-on-a-meter-across-its-subscriptions.html | https://thenewstack.io/anthropic-agent-sdk-credits/ | https://gist.github.com/MagnaCapax/d9177e35b355853f03c730dfcaa693ef | https://dikrana.dev/blog/anthropic-agent-sdk-credit-split/
- **Timeliness**: 4 days ago（2026年5月13日宣布，6月15日生效）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 中文开发者社区把这件事报道成"Claude 涨价了"——这个叙事框架只抓到了表象。Anthropic 在6月15日实际上在做一件更根本的事：**在产品层正式承认"人用 AI"和"机器用 AI"是两种不同的产品，需要两种不同的经济模型**。对话型用量（人→Claude）继续走订阅；Agent 型用量（程序→Claude）开始走计量。这个分界线的出现，意味着 Anthropic 内部已经确认：当前 Agent 使用量的规模和可变性，已经无法再用订阅这个工具来约束了。Compute arbitrage（用 $20 订阅套出数百美元 API 价值的 Agent 工作负载）的存在，说明 Agent 需求已经超过了订阅模型的定价空间。这不只是 Anthropic 的问题——所有 AI 平台最终都会遇到同一个边界：当 AI-to-AI 调用量超过 human-to-AI 调用量，订阅模型就撑不住了。OpenAI 和 Google 面对的是同一个数学问题，只是时间先后不同。对正在用 Claude 构建 Agent 产品的人，6月15日之后有一个非常具体的事：你需要重新核算成本结构。Pro 的 $20 credits 在高强度 Agent 工作负载下可能几天就耗尽，然后你的工具就断了。这是 AI 工具从"订阅消费品"向"工业计量基础设施"转型的第一个可见时间节点。
- **Resonance hook**: 2026年6月15日之后，用 $20 Claude Pro 订阅跑 Agent 工作负载的时代结束了。Anthropic 5月13日宣布：Claude Agent SDK、OpenClaw 等第三方 Agent 框架，从订阅用量池剥离，移到独立计费的 Credit 池，按 API 费率扣减。Pro 每月 $20 credits，Max 5x 每月 $100。社区实测：有效价格提升 12x 到 175x，取决于你的工作负载。但这不只是涨价——是 Anthropic 在产品层第一次正式承认"人用 AI"和"机器用 AI"是两件不同的事。
- **Recommended priority**: high

---

## Candidate 3: Anthropic 和 PwC 扩大同盟——30,000 名顾问培训上 Claude Code，目标是 $2 万亿企业技术债

- **Event**: 2026年5月14日，Anthropic 和 PricewaterhouseCoopers（PwC）宣布扩大战略同盟。核心内容：**① 30,000 名 PwC 美国专业人员**接受 Claude Code 和 Claude Cowork 系统培训认证，随后向 PwC 全球 **364,000 人、136 国**推广；**② 建立联合卓越中心（Center of Excellence）**，三个最高杠杆点：Agentic 技术构建（为客户实施 AI 生产系统）、AI-Native 并购尽职调查、企业职能重组（CFO、供应链、HR）；**③ 新设 Claude-Native 财务业务团队**，嵌入 PwC 的 Office of the CFO 实践；**④ 此次合作属于 Anthropic Claude Partner Network 的最深度承诺**，Anthropic 在 2026 年投入 $1 亿支持服务机构帮助企业真正部署 AI（而非只做 pilot）。**已公开生产部署结果**：保险承销周期从 **10 周压缩到 10 天**，网络安全事件响应从**数小时压缩到数分钟**，客户交付改善最高达 **70%**，一个停滞的 HR 项目在一周内以可用原型重启，一个 COBOL 主机迁移项目在超出预期工作量的情况下仍按时推进、低于预算。战略目标：应对全球超过 **$2 万亿企业技术债**（遗留系统、数据孤岛、手工流程）。SiliconANGLE（5月14日）、PR Newswire（5月15日）、Cryptopolitan（5月15日）覆盖；PwC 和 Anthropic 官方同日发布新闻稿。
- **Source**: https://www.anthropic.com/news/pwc-expanded-partnership | https://www.pwc.com/us/en/about-us/newsroom/press-releases/anthropic-pwc-expand-alliance-agentic-enterprise.html | https://siliconangle.com/2026/05/14/pwc-expands-anthropic-alliance-will-train-30000-staff-claude/ | https://www.prnewswire.com/news-releases/anthropic-and-pwc-expand-alliance-driving-impact-across-client-work-and-the-firm-302772321.html | https://www.cryptopolitan.com/pwc-to-train-30000-staff-on-claude-code/
- **Timeliness**: 3 days ago（2026年5月14日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 中文媒体的报道框架：Anthropic 又签了一家大咨询公司。5月11日的 OpenAI DeployCo（McKinsey 和 Bain 同时是投资者和竞争对手）已经在5月14日 candidates 里覆盖了一侧。PwC 是另一侧，但 Zico 的角度完全不同：**PwC 不是 DeployCo 的竞争对手，PwC 是在主动把自己变成 AI 部署基础设施**。DeployCo 的策略是"AI 公司自己进企业"；PwC 的策略是"传统咨询公司让自己成为 AI 的执行通道"。COBOL 主机迁移在超出预期工作量的情况下按时、低预算完成——这句话意味着什么？意味着 PwC 用 AI 吸收了本该增加人头的范围变更，没有扩充团队，直接交付。**这是 AI 在专业服务领域第一批有数字的"以不变应万变"案例**：不雇更多人，不延期，成本不超——用 Claude Code 消化 scope creep。对组织设计来说，这是"弹性劳动力的第一个工业案例"：当你的知识工作者都用 Claude Code，面对工作负载波峰时你不需要招聘，直接让 AI 多跑几个并行任务。$2 万亿技术债框架也很重要：Anthropic 在定位自己不是"效率工具"，而是"可测量的债务偿还基础设施"。这对卖给企业的 AI 产品是一个值得借鉴的策略框架。
- **Resonance hook**: 2026年5月14日，Anthropic 和 PwC 扩大同盟：30,000 名顾问要被培训上 Claude Code，目标是全球 $2 万亿企业技术债。一个 COBOL 主机迁移项目，工作量超预期，但按时完工、低于预算——他们用 AI 吸收了本该加人加钱的 scope creep。保险承销从10周压缩到10天。这不是效率提升的宣传材料——这是专业服务行业第一批有具体数字的"人头不变、产出弹性"案例。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**: OpenAI 官方博客（5月14-15日 Codex Mobile；5月13日 GPT-Realtime-Whisper 三个 Realtime Audio 模型）、TechCrunch（5月14日 Codex Mobile；5月14日 Anthropic Gates Foundation）、MacRumors（5月15日 Codex Mobile）、CIOL / WinBuzzer / Kingy AI（5月15日 Codex Mobile）、VentureBeat（5月13日 Anthropic Agent SDK 计费重组 + OpenClaw 复活）、InfoWorld（5月13日 Agent SDK metering）、The New Stack（5月13日 Agent SDK billing split）、MagnaCapax GitHub Gist（社区规范化 Agent SDK 价格影响分析，12x-175x 实测）、dikrana.dev / devtoolpicks（Agent SDK June 15 影响分析）、Anthropic 官方（5月14日 PwC expanded partnership；5月14日 Gates Foundation $200M）、PwC 官方新闻稿（5月14日 PwC-Anthropic alliance）、SiliconANGLE（5月14日 PwC + Claude 30,000 staff）、PR Newswire（5月15日 PwC-Anthropic PRN）、Cryptopolitan（5月15日 PwC Claude Code $2T tech debt）、Slashdot / PYMNTS / QZ / Benzinga（5月14日 Gates Foundation $200M 覆盖）、Gates Foundation 官方（5月13日 press release）、X/Twitter（Jim Fan：AI Ascent 2026 上 Physical Turing Test talk 发布于4月20日，27天前，在30天窗口内但次优；Karpathy：5月内无独立新信号；Altman：5月14-17日无独立可用锚点；Swyx/Nat Friedman：无新独立信号）、GitHub Trending（OpenHuman v0.53.43 于5月13日发布，776 stars，早期动力不足以与 3 个主要候选竞争；anthropics/financial-services 仓库冲上12K+ stars，但属 Claude for Small Business 生态，昨日 candidates 已覆盖）、HN（Agent SDK 计费变更上榜讨论中；Gates Foundation 上榜）、arXiv cs.AI（SciResearcher 论文5月2日，15天前；无5月14日后新突破性论文超过现有 candidates）
- **Total signals found**: 27 evaluated
- **Why these 3**:
  - **Candidate 1（OpenAI Codex Mobile）**：时效最强（2-3天，5月14-15日），TechCrunch + MacRumors + OpenAI 官方多媒体确认；**AI 协作实践**柱在过去3天 candidates 中完全空缺（5月13-15日覆盖的是 Agent 经济、AI 产品战略、深层思考、组织形式）；"Codex 在 Mac 上全速跑，手机 Approve/Reject 例外决策点"的异步监督模式是一个新的工作范式，不是新功能；Claude Code Remote 和 OpenAI Codex Mobile 同期出现说明这是行业结构性转移而非单点创新；中文媒体停留在"手机编程"叙事，完全没有"人从驱动者变成例外处理者"的角度。
  - **Candidate 2（Anthropic Agent SDK Metering）**：时效4天（5月13日宣布）；**Agent 经济**柱的经济结构角度在过去3天 candidates 中空缺（5月13-15日 Agent 经济覆盖的是 Claude for Legal、Claude for Small Business 的部署策略，不是定价模型）；"人用 AI vs 机器用 AI 在产品层正式分叉"是 Agent 经济的核心分水岭事件；12x-175x 有效价格提升有可独立验证的社区数学推导（MagnaCapax Gist）；中文开发者社区对 June 15 影响的理解大部分停留在"涨价了"，对结构含义的覆盖接近零；这个边界迟早会出现在所有 AI 平台，Anthropic 是第一家公开划定它的。
  - **Candidate 3（Anthropic PwC）**：时效3天（5月14日）；**组织形式变革**柱：5月14日 candidates 覆盖 OpenAI DeployCo（AI 公司进入咨询市场），今日候选角度是"传统咨询公司主动变成 AI 部署通道"，两者是同一趋势的两个方向，无重叠；"COBOL 迁移工作量超预期但按时低预算交付"是可独立验证的"AI 吸收范围变更而不加人"案例，是专业服务领域弹性劳动力的第一批公开数字；$2T 技术债框架对 B2B AI 产品的定位策略有直接参考价值；30,000 人培训规模是目前专业服务业最大的 AI 工具强制部署案例，中文媒体完全停留在"大合同"叙事。

---

**Excluded signals**:
- OpenAI GPT-Realtime-Whisper + GPT-Realtime-2 + GPT-Realtime-Translate（5月7-8日，10天前）：超7天理想窗口；中文科技媒体已覆盖"实时语音翻译 API"层面，信息增量有限；与 Zico 受众直接相关性弱于上述三个候选
- Anthropic Gates Foundation $200M（5月13-14日）：时效强（3-4天），但全球卫生/教育 AI 与 Zico 的 AI 产品战略 + Agent 经济 + 组织形式核心受众契合度低于上述三个候选；中文科技媒体已有覆盖（虽然浅），信息差相对较小
- Jim Fan AI Ascent 2026 Robotics Endgame + Physical Turing Test（实际发布4月20日，27天前）：已接近30天窗口边界；世界模型 + 机器人学习 survey 在5月14日 candidates 已覆盖，同一主题柱再次出现会造成5日内重复
- OpenHuman GitHub Trending（5月13日 v0.53.43，776 stars）：来源质量 Tier 2-3（AIToolly、TechTimes 覆盖为主），stars 量级远低于社区规模临界点，不满足"事件锚点需具体且可追溯"标准
- Anthropic Code with Claude 2026 开发者大会回顾（5月6日，11天前）：超7天理想窗口，主体事件在5月8日 candidates 已覆盖
- Cursor 3.3（5月发布，并行 Agent + PR review）：发布日期无法确认在5月10日后，来源 Tier 2-3，信息不够清晰，排除
