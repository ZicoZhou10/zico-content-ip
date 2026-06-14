---
date: 2026-06-14
status: pending_selection
---

# Today's Candidates

## Candidate 1: 美国政府命令 Anthropic 关闭 Fable 5 和 Mythos 5——发布第3天被叫停，触发条件是竞争者的一份声明，不是真实攻击（June 12）

- **Event**: 2026年6月12日17:21 ET，美国商务部长 **Howard Lutnick** 致函 **Anthropic CEO Dario Amodei**，援引出口管制法规，以"国家安全"为由，要求暂停 **Fable 5** 和 **Mythos 5** 对所有外国人的访问——包括 Anthropic 在美国境内的外籍雇员。因无法实时区分外籍用户，Anthropic 选择对**全球所有用户**关闭两款模型（其他 Claude 模型不受影响）。Fable 5 于2026年6月9日发布，关闭发生在发布仅 **3天后**。触发原因：另一家公司声称已能越狱 Mythos 5，可绕过安全限制，让模型发现软件漏洞。Anthropic 审查了演示，认定只是"**少量已知的次要软件漏洞**"，其他公开可用模型可以发现同样的漏洞。Anthropic 官方声明明确反驳：如果这一标准被推广，"**实际上将阻止所有前沿模型供应商的新模型发布**"，并称此次指令为"误解"，正在争取恢复访问。**Axios** 标题：《Trump admin blocks foreign access to Anthropic's most powerful AI》；**TheNextWeb** 标题：《US gov orders Anthropic to pull Fable 5 and Mythos 5 in unprecedented AI model recall》；**Fortune**（June 13）独立报道确认。
- **Source**: https://www.axios.com/2026/06/12/anthropic-trump-mythos-fable-national-security | https://www.cnbc.com/2026/06/12/anthropic-disables-access-to-fable-5-and-mythos-5-to-comply-with-government-directive.html | https://thenextweb.com/news/anthropic-fable-mythos-us-government-suspension | https://www.anthropic.com/news/fable-mythos-access | https://fortune.com/2026/06/13/anthropic-disables-fable-mythos-export-controls-national-security-threat/
- **Timeliness**: 2天前（2026年6月12日17:21 ET 政府指令；6月12-13日 Axios + CNBC + Fortune + TheNextWeb 报道）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: 这是 AI 历史上第一次有一个商业前沿模型在发布3天后被政府命令关闭。关闭 Fable 5 的触发条件是"另一家公司声称找到了越狱方法"——不是一次真实攻击，不是数据泄露，是竞争者的一份声明。商务部长 Howard Lutnick 基于这份演示签发出口管制令。

  Anthropic 审查之后的结论：只是"少量已知的次要漏洞"，其他公开模型同样可以发现。但这个结论没有阻止关闭指令执行。

  这暴露了一个被低估的风险结构：如果标准是"任何竞争者可以声称越狱"，这个标准对所有前沿模型都有效。Anthropic 在官方声明里已经说穿了：如果这个标准被推广，"实际上将阻止所有前沿模型供应商发布新模型"。那不是在保护安全，是在让监管程序成为竞争武器。

  还有一个反讽值得说：Anthropic 是业内最积极倡导 AI 安全监管的公司——Project Glasswing（政府专属解锁通道）、静默降级机制、Constitutional AI、RSP 框架，都是 Anthropic 主动建立的。他们为政府监管铺好了配合路径，结果成为第一个被监管命令强制下线的公司。安全架构能设计如何处理能力风险，但无法设计如何应对竞争者触发的政治性干预。

  对做 AI 产品的人：上线前的安全测试 + 政府关系管理，这两件事此前是独立的。Fable 5 的案例说明它们已经合并成同一个风险点。发布一个模型，需要同时在技术层和政治层都通过"足够安全"的判定，而政治层的判定者不一定会听技术层的结论。

- **Resonance hook**: 6月12日17:21 ET，美国商务部长 Howard Lutnick 给 Dario Amodei 发了一封信：关闭 Fable 5 和 Mythos 5。发布3天后。原因是另一家公司声称能越狱 Mythos 5。Anthropic 说他们看了演示，只是"少量已知的次要漏洞"。但模型还是关掉了。Anthropic 自己在官方声明里说：如果这个标准被推广，"实际上将阻止所有前沿模型供应商发布新模型"。历史上第一次有政府命令商业 AI 模型下线。触发条件不是攻击，是声明。
- **Recommended priority**: high

---

## Candidate 2: OpenAI 收购 Ona（前 Gitpod）——Codex 从同步工具变成异步 Agent，你关掉电脑它继续工作数小时（June 11）

- **Event**: 2026年6月11日，**OpenAI** 宣布收购德国云基础设施创业公司 **Ona**（即 **Gitpod GmbH**，2019年以 Gitpod 成立，后更名 Ona）。财务条款未披露。战略目的：允许 **Codex**（OpenAI 的 AI 编码 Agent）在用户关闭笔记本电脑后继续独立运行数小时至数天，完成完整的 Agent 任务。Ona 的技术架构：① **云端沙箱**（cloud-based sandboxes）——隔离、可处置的执行环境，AI Agent 在其中安全运行；② **访问控制 + 审计日志**——满足受监管行业合规要求；③ **客户自有云执行**（customer-controlled execution）——Agent 在客户自己的云环境中运行，OpenAI 提供模型和编排层，客户控制数据边界。**Codex 当前规模**：超过 **500万** 周活用户（较今年初增长 **400%+**）；知识工作者（分析师、设计师、投资人、银行家）占用户 **20%**，增速是开发者的 **3倍**；最快增长任务：数据分析（周增 +110%）、研究（+37%）、报告/表格（+36%）。同步背景：6月2日 OpenAI 已推出面向知识工作者的 **6款角色专属插件**，以及 **Codex Sites**（让 Codex 构建并托管交互式 Web 应用）。来源：**Bloomberg**（June 11，《OpenAI to Acquire Cloud Platform Ona to Support AI Agents》）、**CNBC**（June 11）、TheNextWeb、**OpenAI 官方**（June 11）。
- **Source**: https://openai.com/index/openai-to-acquire-ona/ | https://www.bloomberg.com/news/articles/2026-06-11/openai-to-acquire-cloud-platform-ona-to-support-ai-agents | https://www.cnbc.com/2026/06/11/open-ai-ona-acquisition-codex.html | https://thenextweb.com/news/openai-acquires-ona-codex | https://blog.getbind.co/openai-codex-reaches-5-million-weekly-users-and-launches-role-specific-plugins-for-every-knowledge-worker/
- **Timeliness**: 3天前（2026年6月11日 Bloomberg + CNBC + OpenAI 官方首发）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 收购 Ona 改变了一个根本属性：Codex 从同步工具变成了异步 Agent。

  同步 Codex：你打开电脑，输入问题，等 AI 给答案，关电脑，Agent 停止。生命周期和用户在线时间绑定。Ona 的技术做的事是切断这个绑定：你描述一个任务，Codex 进入 Ona 的云沙箱，开始独立工作——读代码库、写代码、运行测试、修 bug、提 PR——你的电脑可以关掉，几小时后任务完成，你再去看结果。这是 Agent 时态的根本转换。

  知识工作者增速是开发者3倍，这个数字直接说明了 Codex 正在越过代码领域，进入报告、数据分析、投资研究这类可以异步完成的工作。分析师不需要等 Codex，他们让 Codex 跑，自己去做别的事。Ona 的收购是在基础设施层确认这个方向：OpenAI 在为"人不在场、AI 完成任务"建设后端。

  Ona 的企业级特性（审计日志、访问控制、客户自有云）是这个转变的前提条件，不是加分项。企业不会把 Agent 接入生产系统，除非能看到 Agent 在做什么，以及 Agent 只能访问被授权的内容。Ona 解决了合规问题，OpenAI 的 Codex 才能进入受监管行业。

  从基础设施视角：Ona 是 Agent 时代的"应用服务器"。同步 AI 工具需要客户端，异步 Agent 需要后端。OpenAI 通过这次收购，从 AI 模型公司开始变成 AI Agent 基础设施公司。下一个问题：其他 Agent 平台（Anthropic、Google）会用什么后端？

- **Resonance hook**: 6月11日，OpenAI 宣布收购 Ona——就是以前的 Gitpod。收购理由很具体：让 Codex 在你关掉笔记本电脑之后继续工作数小时。以前 Codex 必须和你一起在线；现在 Codex 进入 Ona 的云沙箱，独立读代码、写代码、提 PR——审计日志、访问控制、客户自有云都备好了。Codex 现在500万周活用户，其中知识工作者（分析师、投资人、银行家）的增速是开发者的3倍。OpenAI 在为"AI 自己完成任务、人不需要在场"这件事建设后端基础设施。
- **Recommended priority**: high

---

## Candidate 3: Ramp AI Index 2026年6月——Anthropic 以41%首次超越 OpenAI 成为美国企业第一 AI 供应商，"从未用过 AI 的企业"直接选 Claude（June 2026）

- **Event**: **Ramp**（覆盖超过 **5万家** 美国企业实际支付数据的企业支出追踪平台）发布 **2026年6月 AI Index**：**Anthropic** 以 **41%** 的美国企业付费 AI 订阅占比，首次超越 **OpenAI**（39.5%），成为美国企业最广泛采用的 AI 供应商，6月环比增长 **2.5个百分点**。关键细节：① **"never-adopters"**（此前从未购买过任何付费 AI 产品的企业）现在直接选择 Claude，跳过 OpenAI；② 企业 AI 服务首次采购对决中，Anthropic 赢得约 **70%** 的新客户；③ 增速轨迹：Anthropic 从2023年6月 **0.03%**，到2025年4月 **7.94%**，到2026年4月 **34.44%**，到2026年6月 **41%**——2026年 Q2 增速出现指数加速（两个月 +6.5个百分点）。重要方法论说明：Ramp 数据来自实际信用卡和账单记录，**不是调查问卷**，代表真实付款行为。来源：Ramp AI Index（2026年6月）、**VentureBeat**（《Anthropic finally beat OpenAI in business AI adoption》）、FourWeekMBA、MindStudio 分析。时间背景：这份数据发布的同一周，Anthropic 的 Fable 5 和 Mythos 5 因政府指令被关闭。
- **Source**: https://ramp.com/leading-indicators/ai-index-june-2026 | https://venturebeat.com/technology/anthropic-finally-beat-openai-in-business-ai-adoption-but-3-big-threats-could-erase-its-lead/ | https://fourweekmba.com/anthropic-overtakes-openai-enterprise-adoption-ramp-ai-index/ | https://www.mindstudio.ai/blog/anthropic-vs-openai-business-adoption-2026-ramp-data-2
- **Timeliness**: 本周（2026年6月 Ramp AI Index，月度发布）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: Ramp 的数据不是问卷，是实际付款记录。这让这份数据的质量比大多数"AI 采用率"调研高出一个数量级。

  41% vs 39.5% 看起来边际很小，但有两个更关键的信号：① "never-adopters"直接选 Claude——那些此前从不购买 AI 产品的企业，现在的第一次 AI 采购去了 Anthropic，不是 OpenAI。这不是存量用户转移，是 Anthropic 在开拓 OpenAI 没有触达的增量市场。② 增速在加速：2026年 Q2，Anthropic 两个月增加了6.5个百分点，相当于全年增量的一半在最近8周完成。

  这个增长背后有两个驱动力是可以具体说的。第一个是产品力：Fable 5 发布（6月9日）之前几个月，Claude 在代码、长文档处理、工具调用上持续积累企业用户偏好。第二个是安全叙事转化为采购决策：企业 IT 部门在 AI 采购决策里越来越重视"合规记录"，Anthropic 的 Constitutional AI + 政府合作（Project Glasswing）成了差异化。企业合规官更容易给 Anthropic 通过内部审批。

  最值得追问的时间节点：这份数据发布的同一周，Anthropic 旗舰模型被政府叫停。Anthropic 刚刚成为美国企业第一 AI 供应商，Fable 5 三天后离线。市场领导地位和监管合规不是同一件事，甚至可能是两个独立维度的博弈——Anthropic 赢了市场维度，在监管维度被打了一记。这两件事同时发生，是本周最值得同时看的两个数据点。

- **Resonance hook**: Ramp 追踪5万家美国企业的实际 AI 付款记录（不是问卷），2026年6月数据：Anthropic 41%，OpenAI 39.5%。Anthropic 首次超越 OpenAI，成为美国企业最广泛付费的 AI 供应商。更关键的一个细节：从未购买过 AI 产品的企业，现在第一次采购直接选了 Claude，跳过了 OpenAI。两年前 Anthropic 的企业采用率是0.03%。这份数据发布的同一周，Fable 5 被政府命令下线。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**:
  - OpenAI Newsroom 官方（June 2026 company announcements，产品发布扫描）
  - Releasebot OpenAI（June 2026 release notes，版本更新扫描）
  - Bloomberg（June 11，《OpenAI to Acquire Cloud Platform Ona to Support AI Agents》，原始报道）
  - CNBC（June 11，《OpenAI to acquire Ona to support its AI coding assistant, Codex》）
  - TheNextWeb（《OpenAI acquires Ona to run Codex agents inside the customer's own cloud》）
  - OpenAI 官方（June 11，《OpenAI to acquire Ona》公告原文；June 2，《Codex for knowledge work》5M用户数据）
  - TechTimes（June 13，《OpenAI Acquires Ona to Run Codex Coding Agents for Hours Without Your Computer On》）
  - MLQ.ai（《OpenAI Acquires German Cloud Startup Ona》，技术细节）
  - Bind AI Blog（《OpenAI Codex Reaches 5 Million Weekly Users》，知识工作者数据）
  - TechCrunch（June 2，《OpenAI launches new Codex tools for white-collar work》）
  - Axios（June 12，《Trump admin blocks foreign access to Anthropic's most powerful AI》，Fable 5 关闭原始报道）
  - CNBC（June 12，《Anthropic disables access to Fable 5 and Mythos 5》，第二方确认）
  - TheNextWeb（《US gov orders Anthropic to pull Fable 5 and Mythos 5 in unprecedented AI model recall》）
  - TechRadar（《After a 'potential jailbreak', Anthropic is shutting off access to its Mythos 5 and Fable 5 models》）
  - Fortune（June 13，《Anthropic disables Fable and Mythos AI models following U.S. government export ban》）
  - The New Stack（《Federal government orders Anthropic to pull Fable 5 and Mythos 5, three days after launch》）
  - NBC News（《Anthropic suspends new AI models after government directive》）
  - MarkTechPost（《Anthropic Disables Claude Fable 5 and Mythos 5 After US Government Order》）
  - heise online（《US government forces shutdown of Anthropic's AI Fable 5 and Mythos 5》，德国视角）
  - Anthropic 官方声明（《Statement on the US government directive to suspend access to Fable 5 and Mythos 5》）
  - Ramp AI Index June 2026（ramp.com/leading-indicators/ai-index-june-2026，实际支付数据）
  - VentureBeat（《Anthropic finally beat OpenAI in business AI adoption》，Ramp 数据分析）
  - FourWeekMBA（《Anthropic Just Overtook OpenAI in Enterprise Adoption》）
  - MindStudio（《Anthropic vs OpenAI Business Adoption in 2026: What the RAMP Data Shows》）
  - Axios（May 13，《Anthropic overtakes OpenAI in workplace AI adoption》，Ramp 首发报道）
  - BuildFastWithAI（June 13，《AI News Today: 16 Biggest Stories》，全局信号扫描）
  - LLM-stats.com（June 2026 AI Updates，全局模型发布扫描）
  - Karpathy（June 2026 近期活动，Sequoia Ascent 演讲；无独立 June 12-14 事件锚点，排除）
  - Demis Hassabis（Google I/O May 2026，AGI 2030预测；超7天，排除）
  - Jim Fan / NVIDIA GEAR（"Dream Zero"世界模型；无精确 June 2026 独立发布事件锚点，排除）
  - GPT-5.6（预期发布，无已确认日期锚点，排除）
  - Qwen 3.7 Plus（June 2，12天前；时效可接受，但 Agent 经济柱与 Ona/Codex 高度主题重叠，排除）
  - NVIDIA RTX Spark + Microsoft AI PC（Computex June 1，13天前；时效偏旧，排除）
  - SpaceX IPO（June 11-12，非 AI 内容，排除）
  - GitHub Trending AI repos（OpenClaw 210K星、OpenCode 172K星为长期趋势，无独立 June 12-14 爆发事件，排除）
  - arXiv June 2026 空间智能论文（HY-World 2.0 April、SpaceDG May、MetaEarth3D April，均超7天，排除）
  - Google Gemini CLI shutdown（June 18 EOL 倒计时，已在 June 11 candidates 全面覆盖，排除重复）
  - G7 summit AI CEOs（June 15-17 即将开幕，已在 June 13 candidates 全面覆盖，排除重复）
  - GitLab Agentic Era restructuring（已在 June 13 candidates 覆盖，排除重复）
  - Bioweapon DNA letter（已在 June 13 candidates 覆盖，排除重复）
  - NEURA Robotics / Tether（已在 June 12 candidates 覆盖，排除重复）
  - Microsoft MAI（已在 June 12 candidates 覆盖，排除重复）
  - GitHub Copilot token billing（已在 June 12 candidates 覆盖，排除重复）
  - Anthropic Fable 5 静默降级（已在 June 11 candidates 覆盖；今日 Candidate 1 是政府强制关闭，为不同事件）

- **Total signals found**: 约45个评估

- **Why these 3**:

  - **Candidate 1（Anthropic Fable 5 政府关闭令，June 12）**：时效2天，Axios + CNBC + TheNextWeb + Fortune + NBC News + Anthropic 官方6方来源确认；深层AI思考柱：过去3天此柱在 June 11 Fable 5 静默降级（Karpathy "too trigger happy" + Project Glasswing 分析）中被覆盖，今天角度根本不同——这不是产品设计选择，是**政府强制命令下线**，且触发条件是竞争者声明而非真实攻击，这是 AI 治理进入新阶段的具体事件；"unprecedented AI model recall"在中文 AI 圈几乎无深度分析（大多数报道停留在"模型被关掉"层面，无人拆解政治性干预与技术性安全标准之间的裂缝）；HIGH 优先级。

  - **Candidate 2（OpenAI + Ona Codex 异步化，June 11）**：时效3天，Bloomberg + CNBC + OpenAI 官方3方来源确认；Agent 经济柱：过去3天 Agent 经济柱在 June 12 NEURA Robotics（机器人经济主体）中被覆盖，今天角度不重叠——这是软件层 Agent 基础设施的关键缺口被补上（async execution = 人不在场的 Agent），知识工作者增速3倍于开发者这个数字是 Codex 已经越过纯代码工具定位的具体信号；中文 AI 圈普遍把此事报为"OpenAI 收购云公司"，完全未讨论"同步→异步"的 Agent 范式转换；HIGH 优先级。

  - **Candidate 3（Ramp AI Index June 2026，Anthropic 首超 OpenAI）**：时效本周（月度 Ramp 报告），Ramp 官方 + VentureBeat + FourWeekMBA 多方确认；AI 产品战略柱：过去3天此柱在 June 13 G7 AI 主权（AI 产品战略）和 June 12 Microsoft MAI（AI 产品战略）中被覆盖——今天角度不重叠：这是基于实际付款记录的市场份额翻转，41% vs 39.5% 的背后是"never-adopters 直接选 Claude"的市场开拓结构，而非存量转移；与 Candidate 1（同周 Fable 5 政府关闭）并置能产生"市场第一 + 旗舰模型下线同周发生"的强反差叙事，提升两篇选题的共振效应；HIGH 优先级。
