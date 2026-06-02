---
date: 2026-06-02
status: written
selected: candidate 1 → drafts/035-model-parasitism-xhs.md
---

# Today's Candidates

## Candidate 1: Microsoft 在 Build 2026 发布自研 AI 编程模型 Project Polaris，从 8 月起替换 GitHub Copilot 里的 GPT-4 Turbo，并点名 Claude Code 是它要干掉的对手

- **Event**: 2026年6月2日（今天），Microsoft Build 2026 开幕，Satya Nadella 在旧金山 Fort Mason Center 发表主旨演讲，宣布 **Project Polaris**——微软自研 AI 编程模型——从 **2026年8月** 起替代 **GPT-4 Turbo**，成为 GitHub Copilot 的默认推理引擎（提供3个月 GPT-4 回退期供企业团队过渡）。技术细节：混合专家架构（Mixture-of-Experts），针对不同编程语言和框架定制专项子模块；在 **HumanEval 和 MBPP benchmark** 上优于 GPT-4 Turbo，低资源语言（Rust、Haskell）提升尤为显著；运行在 Azure 自研 **Maia AI 加速器**上，降低推理延迟和单次成本；Pro 用户获得 **10 万行多文件上下文**和自主测试生成能力。战略信号：**Microsoft 在发布会上公开命名 Claude Code 为 Polaris 要取代的竞争对手**——这是主流 AI 工具厂商首次在产品发布会上明确承认，在开发者 AI 编程工具这一品类中，Anthropic 已取得可量化的市场份额。同场宣布：**Windows Agent Store**（开发者提交 Agent 获 **85% 分成**，对比 App Store 的 30%；Adobe 和 Zoom 已签约早期合作）；**Windows Agent Framework** 开源；**Azure Agent Mesh**（联邦 Agent 执行控制平面，按延迟和 GPU 可用性跨三个部署目标路由任务）；**Copilot Workspace** 全面 GA；**Foundry Local** GA（Windows/macOS Apple Silicon/Linux x64 离线 AI 推理）。来源：ChatForest Build 2026 Recap（June 2）、AI Weekly（Microsoft Targets Claude Code with Project Polaris）、WindowsNews.ai（Build 2026: Homegrown AI Models to Power GitHub Copilot）、WindowsForum（Build 2026: Microsoft Makes Windows an Agent Platform）。
- **Source**: https://chatforest.com/builders-log/microsoft-build-2026-recap-windows-agent-platform-project-polaris-copilot-workspace/ | https://aiweekly.co/alerts/microsoft-targets-claude-code-with-project-polaris | https://windowsnews.ai/article/microsoft-build-2026-homegrown-ai-models-to-power-github-copilot.420887 | https://windowsforum.com/threads/microsoft-build-2026-ai-agents-copilot-azure-ai-foundry-and-windows-local-ai.420861/
- **Timeliness**: 今天（0 天）；Build 2026 开幕日
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 最重要的信息不是 Polaris 的 benchmark 数字，是微软在发布会上点名了 Claude Code。

  公司在产品发布会上点名竞争对手，通常意味着：市场份额数据已经足够难看，没必要装了。微软在 GitHub Copilot 上的问题在今年5月已经有据可查——微软 Experiences & Devices 部门（Windows、Office、Teams、Surface）因为工程师用量超标，主动取消了大量 Claude Code 许可证。意思是：微软的内部工程师，在公司付费的 Copilot 旁边，用 Anthropic 的产品完成工作。

  现在微软同时做了两件事：① 把 OpenAI 的模型从 Copilot 里换掉，用自研模型替代（降低对 OpenAI 的依赖和推理成本）；② 宣布这个自研模型专门为对抗 Claude Code 而建。

  这两件事合在一起说明：**微软意识到"把 OpenAI 的模型塞进 VS Code 插件"不是一个可持续的产品策略**。Claude Code 赢开发者，不是因为 GPT-4 Turbo 不好，是因为 Anthropic 在整个开发者体验上做得更深——工作流集成、context window、多文件编辑。Polaris 是技术层面的响应。Windows Agent Store 的 85% 分成是生态层面的战略赌注。

  有一个更深层的结构性判断值得单独说：**当你在 AI 产品里依赖第三方模型，你永远是一个产品决策之外的风险**。GitHub Copilot 在 OpenAI 模型上构建了四年。今天，这个"替换"决定是微软主动做的。但如果是 OpenAI 先动——调价、改接口、收回授权——微软的处境会很难看。Polaris 首先解决的是这个架构风险，对抗 Claude Code 是第二位的。

- **Resonance hook**: 2026年6月2日，Microsoft Build 开幕。微软发布 Project Polaris，自研 AI 编程模型，从8月起替换 GitHub Copilot 里的 GPT-4 Turbo。发布会上，微软点名了 Claude Code 是它要干掉的竞争对手。同一周，微软内部工程师因为 Claude Code 用量超标，被公司取消了 Copilot 许可证。一家公司在发布会上点名竞争对手，通常是因为数据已经不好看了，没必要装了。
- **Recommended priority**: high

---

## Candidate 2: Anthropic June 15 计费分拆——AI 平台第一次在账单里正式区分"人类使用"和"Agent 使用"（背景：OpenClaw 封禁风波）

- **Event**: **2026年5月13日**，Anthropic 官方宣布，从 **2026年6月15日** 起（距今13天），通过订阅计划的程序化使用——**Claude Agent SDK、claude -p、Claude Code GitHub Actions、基于 Agent SDK 的第三方应用**——将从订阅原有限额池分离，移入独立的"**Agent SDK 信用额度**"：Pro $20/月，Max 5x $100/月，Max 20x $200/月，按标准 API 定价计量，不滚存。背景时间线：**4月4日**，Anthropic 禁止第三方 Agent 和 Harness（含 **OpenClaw**）通过订阅使用 Claude——原因：未优化的第三方工具重复处理大量数据，单个 Agent 用户实际消耗数百至数千倍于普通交互用户的资源，威胁系统稳定；**4月10日**，OpenClaw 创始人被 Anthropic 临时封禁访问 Claude（TechCrunch 报道）；**5月13日**：禁令解除"但有条件"——上述计费新架构。开发者反应：**T3.gg 创始人 Theo Browne** 计算，使用 claude -p、Conductor、Zed 等工具的开发者实际程序化使用成本上涨 **25 倍**；深度工作负载（Agentic CI/CD pipeline）的等效价格涨幅达 **12x–175x**；Anthropic Claude Code 团队工程师 **Lydia Hallie** 的说明推文在数小时内遭 **Community Note**。来源：The New Stack（Anthropic splits billing again: Agent SDK gets separate credit pools）；VentureBeat（Anthropic reinstates OpenClaw and third-party agent usage on Claude subscriptions — with a catch）；GitHub Gist canonical reference（MagnaCapax，May 13 Agent SDK policy change 完整数学分析）。
- **Source**: https://thenewstack.io/anthropic-agent-sdk-credits/ | https://venturebeat.com/technology/anthropic-reinstates-openclaw-and-third-party-agent-usage-on-claude-subscriptions-with-a-catch | https://gist.github.com/MagnaCapax/d9177e35b355853f03c730dfcaa693ef | https://techcrunch.com/2026/04/10/anthropic-temporarily-banned-openclaws-creator-from-accessing-claude/
- **Timeliness**: 公告 20 天前（5月13日）；生效日距今 13 天（6月15日）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 这不是 GitHub Copilot 计费混乱的重复（6月1日已写）。那篇是用户侧的"pricing surprise"。今天是平台侧的"governance decision"。

  OpenClaw 被封禁的根本原因：Anthropic 的订阅定价假设"人类以人类的速度使用 Claude"。订阅限额是按一个人一个月能发多少交互请求来估算的。OpenClaw 是一个开源 Agent 框架，在后台自动循环运行，不优化缓存，不停下来等人确认。同一份订阅，人类用户月底还没用完，一个 Agent 在一天内就能烧完。

  **封禁 OpenClaw 是 Anthropic 在说："我们的定价模型无法承担 Agent 的真实成本。"**

  5月13日的计费分拆是 Anthropic 在说："你可以在我们的模型上运行 Agent，但必须按 Agent 的成本付费，不是按人类的成本。"

  这是 **AI 平台第一次在账单层面正式区分"人类使用"和"Agent 使用"**。这个区分的影响是系统性的：任何 AI 工具的产品定价，从现在起必须显式地为两种使用模式设计不同的经济模型——"月费封顶"逻辑不能同时覆盖人类和 Agent，因为两者的消耗量差了一到三个数量级。

  Theo Browne 说这是对开源生态的攻击。另一种读法是：Anthropic 在做一个艰难但必须做的修正——把 Agent 的真实成本从订阅补贴里抽离出来。OpenClaw saga 的完整弧线是：套利 → 封禁 → 反弹 → 有条件解禁 → 正式建制。AI 平台的 Agent 治理，正在从"打补丁"进入"立规矩"的阶段。

- **Resonance hook**: 2026年6月15日，距今13天，Anthropic 要把 Claude 的程序化使用（Agent SDK、claude -p、第三方 Agent 工具）从订阅里拆出来，放进独立额度——Pro 用户 $20，按完整 API 价格计量。这是 OpenClaw 风波的最终结局：4月封禁，5月有条件解禁，6月15日建制。Anthropic 在账单层面第一次正式回答了一个问题：你是人在用，还是 Agent 在用？答案是：两者按不同价格计算。开发者算了下，原来无限额的程序化使用，等效价格涨了 12 到 175 倍。
- **Recommended priority**: medium

---

## Candidate 3: Satya Nadella 在 Build 2026 宣告：Windows 不再只是人类的平台，Agent 是操作系统的一等公民

- **Event**: 2026年6月2日（今天），Microsoft Build 2026 开幕主旨演讲，Satya Nadella 宣告："**Windows is no longer a platform for human users only. Agents are now first-class citizens in the runtime, the tooling, and the distribution model.**" 当天同步宣布 Agent 基础设施全栈：① **Windows Agent Framework** 开源（系统级 Agent 运行框架）；② **Azure Agent Mesh**（联邦化 Agent 执行控制平面，跨三个部署目标按延迟和 GPU 可用性路由任务）；③ **Windows Agent Store**（Agent 分发市场，开发者分成 **85%**；**Adobe** 和 **Zoom** 已签约成为早期合作伙伴）；④ **Copilot Agent Mode**（跨 Microsoft 365 生态系统规划并执行多步骤任务的新运行层级，含 IT 管控护栏）；⑤ **Foundry Local** 全面 GA（Windows/macOS Apple Silicon/Linux x64 离线 AI 推理和 Agent 执行）。来源：WindowsForum（Build 2026: Windows becomes the platform for AI agents）、ChatForest Build 2026 Recap（June 2）、WindowsNews.ai（Build 2026: Microsoft makes Windows an agent platform for AI developers）。
- **Source**: https://windowsforum.com/threads/microsoft-build-2026-windows-becomes-the-platform-for-ai-agents.420503/ | https://chatforest.com/builders-log/microsoft-build-2026-recap-windows-agent-platform-project-polaris-copilot-workspace/ | https://windowsnews.ai/article/build-2026-microsoft-makes-windows-an-agent-platform-for-ai-developers.420496
- **Timeliness**: 今天（0 天）；Build 2026 开幕主旨演讲
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 操作系统是软件行业最大的平台权力。它定义什么是"应用"、什么是"用户"、什么是"交互单元"。

  Windows 在过去40年里的基本假设是：有一个人类，坐在屏幕前，用鼠标和键盘操作。GUI、窗口、任务栏、文件系统、权限模型——所有这些设计的起点都是一个人类用户。

  Satya Nadella 今天说的，字面上很平静。实际上包含一个很大的宣告：**微软在重新定义"用户"是什么**。操作系统不再只为人类设计，也要为 Agent 设计。这不是功能更新，是运行时（runtime）、工具链（tooling）、分发模型（distribution model）的系统性重构。

  Windows Agent Store 的 85% 分成不是出于慷慨，是卡位战略。App Store 以 30% 分成成为不可绕开的基础设施，花了15年。微软在 Agent 生态的最早窗口里，用远高于行业标准的分成比例快速吸引开发者。谁先建立 Agent 的分发渠道，谁就在接下来五年掌握 Agent 生态的流量入口。

  这里有一个组织形式变革的核心问题值得单独想：**如果 Agent 是操作系统的"用户"，那么"组织"的定义是什么？** 一个有 1000 名员工的公司，如果同时有 10 万个 Agent 在 Windows 上运行，组织的规模怎么算？软件采购的逻辑（按席位、按人头）怎么算？IT 治理的单位（"谁批准了这个权限"）怎么算？Satya Nadella 今天开了一个口子，但这些问题会在接下来几年里反复被问到。

- **Resonance hook**: 2026年6月2日，Satya Nadella 在 Build 2026 开幕演讲里说了一句话："Windows is no longer a platform for human users only. Agents are now first-class citizens in the runtime, the tooling, and the distribution model." 同一天，微软宣布 Windows Agent Store，开发者提交 Agent 可以拿到 85% 的分成。App Store 的分成是 30%，花了15年成为不可绕开的基础设施。微软今天在 Agent 生态最早的窗口里，用85%的分成卡住分发入口。操作系统正在重新定义它的"用户"是谁。
- **Recommended priority**: medium

---

## Scan summary

**Sources scanned**:
- Microsoft Build 2026 multi-source（ChatForest Build 2026 Recap June 2；AI Weekly Project Polaris；WindowsNews.ai Build 2026 agent platform；WindowsForum Build 2026 keynote；Notebookcheck Build 2026 preview；Studioglobal Build 2026 themes；WindowsForum Copilot homegrown models）
- Anthropic billing split multi-source（The New Stack "Agent SDK gets separate credit pools"；VentureBeat "OpenClaw reinstated with a catch"；GitHub Gist MagnaCapax canonical math reference；TechCrunch April 10 OpenClaw creator ban；DevToolPicks billing split breakdown；Codersera June 2026 billing guide；ChatForest billing split developer guide；GenaI Unplugged billing workarounds；Zed blog subscription changes；DEV.to claude -p production cost；Level Up Coding repricing analysis）
- KOL X/Twitter 扫描（Karpathy: 最近无独立6月锚点；Sequoia Ascent 2026 博客约4月下旬，超7天窗口；Altman: May 26"很高兴我错了"已在June 1 C3覆盖；LeCun: May 4–7 "don't listen to CEOs"，超7天窗口；Jim Fan: Sequoia AI Ascent 4月20日，已在May 29 scan排除）
- GitHub Trending（AI Weekly June 2026 model releases；Hermes Agent 140K stars 但发布于5月13日，20天，超7天窗口；QwenPaw v1.1.10 June 1，无强叙事角度）
- HN front page（2026-05-31 front；NeuralBuddies May 29 recap；BuildFastWithAI May 31 news roundup）
- Anthropic/OpenAI/DeepMind blogs（Anthropic: June 15 billing announcement May 13；OpenAI: GPT-5.5 Instant May 5 超7天；Rosalind Biodefense May 29已在May 30 scan排除；Frontier Governance Framework May 29已在May 30 candidates覆盖；DeepMind: Boston Dynamics Gemini Robotics-ER April 8 超7天窗口）
- arXiv（Dyna-Think 2506.00320确认为2025年6月投稿非2026，排除；Embodied AI Agents Meta arXiv:2506.22355确认为2025年论文，排除）
- 空间智能前沿（Physical Intelligence π0.7：日期未精确确认为May 26–June 2窗口，排除；ShengShu Motubrain：April 29，超7天窗口，排除；NVIDIA Nemotron 3 Nano Omni：日期未确认；Inception Mercury 2：日期未确认）
- Air Street "State of AI: May 2026"（Nathan Benaich，May 31，月度回顾，作为背景context使用，无独立事件锚点）

**Total signals found**: 约30个评估

**Why these 3**:
- **Candidate 1（Microsoft Build 2026 / Project Polaris，June 2）**：时效最强（今天0天），ChatForest + AI Weekly + WindowsNews + WindowsForum 四方来源确认；AI 产品战略柱：过去3天 SELECTED 覆盖了 Groq/NVIDIA 授权架构（May 30）和 $500M Claude 账单（May 31），今天角度完全不重叠——"大厂自建模型替换第三方依赖 + 公开命名竞争对手"是全新叙事；微软命名 Claude Code 为对手是发布会层面极罕见的公开竞争信号；中文媒体会报道 Build 功能清单但不会分析"微软在 Copilot 上失去了多少开发者份额才做出这个决定"；与 Zico 的 AI 产品战略认知（"在别人模型上构建的架构风险"）高度匹配；HIGH 优先级。
- **Candidate 2（Anthropic Agent SDK billing / OpenClaw，May 13 + June 15）**：时效20天（公告），在30天可接受窗口内；生效日距今13天，developer reaction 当前进行中；Agent 经济柱：与 June 1 SELECTED（GitHub Copilot token billing）互补而非重叠——GitHub Copilot 是"用户侧pricing surprise"，OpenClaw 是"平台侧governance decision"，叙事层次不同；OpenClaw 的完整弧线（套利→封禁→反弹→有条件解禁→建制）是独立且完整的叙事单元；"AI 平台第一次在账单里正式区分人类使用和Agent使用"是一个结构性洞察，中文媒体报道会停在"涨价"这一层；12x–175x 数字可独立验证（GitHub Gist 完整数学推导）；MEDIUM 优先级（时效偏旧，但June 15截止带来当前紧迫性）。
- **Candidate 3（Satya Nadella / Windows Agent Platform，June 2）**：时效最强（今天），WindowsForum + ChatForest + WindowsNews 三方确认；组织形式变革柱：过去3天 SELECTED 候选均未覆盖此柱（May 30–June 1选中的是AI产品战略和Agent经济）；"操作系统重新定义用户是谁"是一个独立于 Project Polaris 竞争叙事的组织/平台形态变革信号；Windows Agent Store 85% 分成是分发层面战略卡位，视角是"谁控制Agent生态入口"而非"产品性能对比"；与 Zico 在酷家乐做 3DGS/Physical AI 产品的一线经验有直接认知连接（Agent 分发平台对 embodied AI 的影响）；MEDIUM 优先级（与 C1 同日同事件，但不同叙事层和主题柱，组织形式变革柱近期缺席是独立加分项）。
