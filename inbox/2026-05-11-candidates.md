---
date: 2026-05-11
status: pending_selection
---

# Today's Candidates

## Candidate 1: ChatGPT 开始自动读取你的 Gmail——OpenAI 的产品战略从"聊天工具"变成了"个人记忆层"

- **Event**: 2026年5月9日，OpenAI 向 Plus 和 Pro 用户推出记忆增强功能，ChatGPT 现在可以在对话中主动引用用户过去的聊天记录、保存的记忆、个人文件，以及——最关键的——**已连接 Gmail 账户中的邮件内容**。用户可通过新的 "Memory Sources" 功能查看每条回答调用了哪些来源（哪次历史对话、哪封邮件）并可编辑。该功能先在 Web 端上线 Plus/Pro，Free/Go/Business/Enterprise 将于数周后跟进。这是 OpenAI 官方 ChatGPT release notes 记录的 5月9日更新，releasebot.io 同步追踪确认。同期背景：OpenAI 在 5月5日将 GPT-5.5 Instant 设为默认模型（幻觉减少 52.5%，回复字数减少 30.2%），5月9日 Codex 同步更新（plugin sharing、线程分页）；Anthropic 在 5月6日与 xAI/SpaceX 签下 Colossus 1 全量算力合同（Candidate 2）。
- **Source**: https://help.openai.com/en/articles/6825453-chatgpt-release-notes | https://releasebot.io/updates/openai/chatgpt | https://www.knightli.com/en/2026/05/07/chatgpt-release-notes-memory-gpt-5-5-sheets/
- **Timeliness**: 2 days ago（2026年5月9日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: ChatGPT 从来不是最强的模型——Gemini 在多模态有优势，Claude 在代码和长文有优势，GPT-5.5 Instant 在速度上领先。OpenAI 的真实竞争策略，一直不是在单轮对话里赢，而是在**时间维度上积累**。Gmail 连接是这个策略的最新执行：每一封你收到的邮件、每一次你用 ChatGPT 回复的对话，都在加深它对你个人上下文的理解。这创造了一种比 API 接入更难打破的护城河：**用的越久，上下文越深，切换成本越高**。做过数据飞轮分析的人都知道，这种积累是指数型的——第一个月的 Gmail 上下文和第十二个月的 Gmail 上下文不是线性差距。对 Claude、Gemini 来说，这意味着竞争维度正在从"哪个模型更智能"迁移到"哪个模型知道你更多"。Anthropic 在企业端用 Microsoft 365 整合（Word/Excel/Outlook/PowerPoint）做了类似的布局，但企业端护城河建立在合同周期上；消费端护城河建立在个人习惯上，前者可以谈判，后者几乎无法改变。更深一层的产品架构问题：OpenAI 正在把 ChatGPT 从"你打开的一个 App"变成"跟随你的一个层"。这不是功能迭代，是产品形态的重新定义。当 ChatGPT 能读你的 Gmail，你和它的关系就不再是"用户-工具"，而是接近"用户-秘书"。秘书是不容易换的。
- **Resonance hook**: ChatGPT 现在可以读你的 Gmail，回答问题时会主动引用你的邮件内容。这不是记忆功能升级——这是 OpenAI 把 ChatGPT 从聊天工具变成个人上下文层的关键一步。越用越难换，这才是 OpenAI 真正的护城河。
- **Recommended priority**: high

---

## Candidate 2: Anthropic 租下了马斯克的整个 GPU 集群——TechCrunch 说这让 xAI 变成了一个 neocloud

- **Event**: 2026年5月6日，Anthropic 与 xAI/SpaceX 正式签署协议，Anthropic 将使用 Colossus 1 数据中心的**全部算力**——300 兆瓦、超过 22 万张 NVIDIA GPU——预计一个月内上线。Anthropic 官方博客（anthropic.com/news/higher-limits-spacex）同日发布，同步宣布 Claude Pro/Max 用率限制翻倍、取消高峰时段用量上限、大幅提升 Claude Opus API 配额。CNBC（5月6日）、Bloomberg（5月6日）、Axios（5月6日）三家同日报道。背景：Dario Amodei 在 5月5日华尔街活动上披露 Q1 年化营收增长 **80 倍**，当前年化营收跑率达 **300 亿美元**；VentureBeat（5月8日）报道估值讨论已触及 **9000 亿美元**。2026年5月10日，TechCrunch 发布分析文章《We're feeling cynical about xAI's big deal with Anthropic》，同日另有分析《Is xAI a neocloud now?》——核心判断：Grok 的用户规模从未增长到 Colossus 1 所设计的算力需求，xAI 被迫将核心基础设施租给竞争对手，标志着 xAI 从"前沿模型公司"向"GPU 租赁服务商"的隐性转型。CoinDesk 补充：该协议时间节点在 SpaceX IPO 预期前夕（6月）。
- **Source**: https://www.anthropic.com/news/higher-limits-spacex | https://www.cnbc.com/2026/05/06/anthropic-spacex-data-center-capacity.html | https://techcrunch.com/2026/05/10/were-feeling-cynical-about-xais-big-deal-with-anthropic/ | https://techcrunch.com/2026/05/06/is-xai-a-neocloud-now/ | https://simonwillison.net/2026/May/7/xai-anthropic/
- **Timeliness**: 5 days ago（协议签署：2026年5月6日）；TechCrunch cynical 分析：1 day ago（2026年5月10日）
- **Topic pillar**: 深层思考
- **Zico's angle**: TechCrunch 说这让 xAI 变成了 neocloud，听起来是批评。但更准确的读法是：**这是 xAI 模型战略正在承压的第一个可量化信号**。Colossus 1 是为 Grok 建的。Grok 3、Grok 4 没有把用户规模带到 300 兆瓦的量级。现在 Anthropic 的 Q1 增长 80 倍、年化 300 亿——他们需要 GPU，今天就要。这个交易的成立条件，恰好是 xAI 模型端的不及预期和 Anthropic 模型端的超预期同时发生。更奇特的是意识形态维度：马斯克正在起诉 OpenAI 背叛安全使命；Dario Amodei 曾把 AI 描述为人类制造过的最危险的东西；Anthropic 因拒绝五角大楼"所有合法目的"条款而被列为供应链风险（5月1日）；同一周，Dario 签下了马斯克的 GPU 集群。在 AI 行业，意识形态定位和商业交易的关系，正在变得难以用简单的"谁安全谁不安全"框架来描述。AI 公司的价值链是：训练数据 → 算力 → 模型 → 分发 → 用户信任。xAI 在算力环节很强，在分发和用户信任环节弱于 Claude。Anthropic 在模型、分发、用户信任都在快速领先，唯独算力不够。这个交易是两家公司价值链的局部互换——不是因为他们彼此认同，而是因为市场压力迫使他们互相需要。这个模式将会重复：在 AI 军备竞赛里，算力稀缺时，竞争对手会成为临时合作方。
- **Resonance hook**: Anthropic 租下了马斯克 Colossus 1 的全部 22 万张 GPU。背后的逻辑：xAI 的 Grok 用户没有增长到填满这些 GPU 的规模，而 Anthropic 的 Q1 营收增长了 80 倍、急需算力。TechCrunch 昨天说：这正在让 xAI 从 AI 模型公司变成 GPU 出租方。两家意识形态截然不同的公司，被市场压力撮合成了临时合作方。
- **Recommended priority**: high

---

## Candidate 3: Addy Osmani 发布 agent-skills——19 条规则让 AI 编程 Agent 像资深工程师一样工作

- **Event**: 2026年5月8日，Addy Osmani（前 Google Chrome DevRel 负责人，现 Anthropic）在 GitHub 发布 **agent-skills**（github.com/addyosmani/agent-skills），并配套发表同名博客文章（addyosmani.com/blog/agent-skills）。项目定位：为 AI 编程 Agent 提供 **19 条生产级工程规范**，覆盖完整软件开发生命周期六阶段：**DEFINE → PLAN → BUILD → VERIFY → REVIEW → SHIP**。每条规范包括：Agent 会用来跳过这一步的常见借口（如 "I'll add tests later"）、要求提供的证据（测试通过截图、构建输出、运行时数据）。支持平台：Claude Code、Cursor、Gemini CLI、Windsurf、GitHub Copilot、Kiro，以及其他支持 AGENTS.md 的工具。发布后 3 天内积累 **8,600+ GitHub stars**，AIToolly（5月8日）确认其在 GitHub Trending AI 类目出现。背景：同期 GitHub Trending 周榜（Week 18）中还有 mattpocock/skills（55k stars，模板类）和 pi-mono（43.9k stars，Agent 工具包），但 agent-skills 是这批项目中唯一专注于"AI Agent 行为规范"而非"工具封装"的。
- **Source**: https://github.com/addyosmani/agent-skills | https://addyosmani.com/blog/agent-skills/ | https://aitoolly.com/ai-news/article/2026-05-08-addy-osmani-launches-agent-skills-a-framework-for-production-grade-engineering-in-ai-coding-agents
- **Timeliness**: 3 days ago（2026年5月8日）
- **Topic pillar**: AI 协作实践
- **Zico's angle**: Claude Opus 4.7 可以写出极好的代码。它写不出来的，是在没有人要求的情况下自己说"等等，我应该先写测试"。agent-skills 要解决的不是模型能力问题，而是**AI Agent 的行为规范缺失问题**。每一条规范对应的是一种 Agent 会在生产环境里犯的专业错误——不是智力错误，而是习惯错误。资深工程师不提交没跑过测试的代码，不是因为他更聪明，而是因为他被 code review 文化、CI/CD 流程、和职业代价训练出了这个习惯。AI Agent 没有这些训练。agent-skills 就是在用 AGENTS.md 文件，把这个习惯直接写进 Agent 的操作逻辑里。这个项目更深的意义在于：它把 CLAUDE.md / AGENTS.md 这类配置文件，从"给这个项目的特殊说明"升级成了"AI 员工入职标准手册的开源规范"。你雇了一个 AI 员工，不给它任何入职文档，然后惊讶它不知道公司的工程文化——这一直是 AI 编程工具在生产环境失败的真实原因。agent-skills 是第一个系统化尝试解决这个问题的开源项目，而且它来自 Anthropic 内部（Addy 现在在 Anthropic），这意味着 Claude Code 的设计团队在用实际行动表达他们对"AI-Native 工程师文化"应该长什么样子的判断。对正在用 Claude Code 或 Cursor 做真实工程的人，这是本周最值得直接拿来用的东西。
- **Resonance hook**: Addy Osmani（曾任 Google Chrome DevRel 负责人，现在 Anthropic）发布了一套 19 条规则，专门解决这个问题：AI 编程 Agent 够聪明，但没有资深工程师的习惯。比如它不会主动说"我应该先写测试"。这 19 条规则直接写进 AGENTS.md，就能让 Claude Code / Cursor / Gemini CLI 在你没要求时自己执行完整的 DEFINE → BUILD → VERIFY → SHIP 流程。3 天 8600 stars。
- **Recommended priority**: medium

---

## Scan summary

- **Sources scanned**: X/Twitter（Karpathy 5月8-11日无独立新信号；Altman/OpenAI 官方博客：5月9日 ChatGPT memory/Gmail rollout；Jim Fan/NVIDIA 5月无新具体锚点；LeCun 5月无新信号；Demis Hassabis 无 5月8-11 新发言）、GitHub Trending AI（Week 18-19：addyosmani/agent-skills 5月8日；mattpocock/skills；pi-mono；jcode）、HN 2026-05-09 前页（ChatGPT Gmail memory；xAI/Anthropic cynical TechCrunch）、OpenAI 官方 release notes（5月9日 ChatGPT memory/Gmail；5月9日 Codex plugin sharing；5月5日 GPT-5.5 Instant 已在 5月6日 candidates 覆盖）、Anthropic 官方博客（5月6日 higher-limits-spacex；Code w/ Claude 2026 会议 5月6日）、xAI 官方（x.ai/news/anthropic-compute-partnership）、TechCrunch（5月10日 cynical xAI/Anthropic；5月6日 Is xAI a neocloud）、CNBC/Bloomberg/Axios/Fortune（5月6日 Anthropic-SpaceX deal）、VentureBeat（5月8日 Anthropic $30B run rate）、arXiv cs.AI 5月最新列表（无 5月8-11 强时效锚点新论文；现有论文提交时间多在 4月或更早）、Google I/O 2026 预告（5月19日，预告内容在泄露阶段，无具体可用事件锚点）
- **Total signals found**: 17 evaluated
- **Why these 3**:
  - **Candidate 1（ChatGPT Gmail memory）**：时效最强（2天），5月9日 OpenAI 官方 release notes 确认；Gmail 连接是 ChatGPT 产品形态从"会话工具"到"个人上下文层"的实质性转变，中文圈对这个功能的报道停留在功能层（"ChatGPT 能读 Gmail 了"），无人从"个人上下文积累作为竞争护城河"框架分析；AI 产品战略柱：5月8日 candidates 覆盖 GPT-Realtime-2 语音 Agent（垂直 Agent 部署通道），本篇是消费端个人记忆层（完全不同的产品战略维度）；"越用越难换"的上下文护城河对 Zico 受众（AI 产品经理、创业者）有直接的策略参照价值。
  - **Candidate 2（xAI Colossus neocloud）**：协议 5 天前（5月6日），TechCrunch 分析文章 1 天前（5月10日）提供新鲜叙事锚点；经逐一核查 5月6日、7日、8日 candidates 文件，该事件均未被选入候选；xAI 从模型公司向 GPU 出租方的隐性转型，是 AI 竞争格局中高价值的结构性信号；意识形态敌对方（Musk-Dario）被市场压力撮合这一细节，在中文圈几乎无分析；深层思考柱：5月8日 candidates 覆盖 Hassabis 50/50，本篇角度（AI 公司价值链局部互换）完全不同。
  - **Candidate 3（Addy Osmani agent-skills）**：时效 3 天（5月8日），8,600 GitHub stars 是强可验证锚点；AI 协作实践柱近期（5月6-8日 candidates）均未使用；agent-skills 不是"又一个 AI 工具"，是第一个将"资深工程师职业习惯"系统化编码进 AGENTS.md 规范的开源项目；Addy Osmani 现在在 Anthropic 的身份给这个项目额外的信号价值（Anthropic 内部对 Claude Code 应该怎么工作的判断）；可直接操作（用户可立即 fork 并在自己的 Claude Code 配置中使用），创造"召唤式产物收尾"的文章结构可能。

- **Excluded signals**:
  - Anthropic $30B revenue run rate（VentureBeat 5月8日报道）：数据来源是 5月5日 Anthropic 华尔街活动，已在 5月7日 candidates Candidate 2 完整覆盖，排除独立候选
  - Code w/ Claude 2026 会议（5月6日，Anthropic 开发者大会，无新模型发布）：未在之前 candidates 中直接覆盖，但事件本身缺乏强叙事锚点（"没有新模型"不是一个 Zico 角度能落到的具体细节），排除
  - OpenAI GPT-5.5 Instant 默认模型（5月5日）：已在 5月6日 candidates Candidate 2 完整覆盖，排除
  - OpenAI Codex plugin sharing 更新（5月9日）：技术细节有用，但无独立叙事价值；开发者工具更新类，Zico 角度不强，排除
  - Musk v. Altman 庭审进展（5月中旬责任认定预期）：庭审背景已在 5月6日 candidates Candidate 3（xAI 蒸馏承认）完整覆盖；责任认定尚未发生，无新事件锚点，排除
  - Google I/O 2026 预告 / Gemini Omni 视频模型泄露（5月19日大会前）：泄露内容（UI 字符串）缺乏足够具体的技术或战略细节作为 Zico 视角的锚点；"泄露" ≠ 可验证事实，8 天后大会本身会有更强锚点，排除
  - arXiv cs.AI 最新列表（5月11日）：无 5月8日之后提交的强 AI agent/reasoning 论文锚点；最新主要论文（Agentic Reasoning 综述）提交于1月，超出7天窗口，排除
  - PocketOS/Cursor 数据库删除事件（2026年4月25日）：事件发生在 16 天前；ServiceNow Knowledge 2026 引用（5月6日）虽是新角度，但核心事件应已在 4月27-30日 candidates 中覆盖，排除重复
