---
date: 2026-05-05
status: written
selected: candidate 1 → drafts/014-floor-line-fallacy-xhs.md
---

# Today's Candidates

## Candidate 1: Karpathy 在 Sequoia Ascent 发布"Agentic Engineering"框架——Vibe Coding 是地板，这才是天花板

- **Event**: 2026年4月29日，Andrej Karpathy 在 Sequoia Capital 主办的 AI Ascent 2026 大会上接受合伙人 Stephanie Zhan 的炉边对话采访。2026年4月30日，Karpathy 在个人博客（karpathy.bearblog.dev/sequoia-ascent-2026/）发布详细回顾，并在 X 发推（status/2049903821095354523）宣传，帖文写道"fireside chat at Sequoia Ascent 2026 from a ~week ago"。核心框架：Software 1.0（显式代码）→ 2.0（神经网络权重）→ 3.0（提示词编程 LLM 解释器，上下文窗口即程序）。关键区分——Vibe Coding vs. Agentic Engineering：Vibe Coding 是提高门槛，让任何人都能构建原型；Agentic Engineering 是拉高天花板，专业人员协调多个易错 AI Agent 的系统工程。Karpathy 定义的 Agentic Engineer：设计规格说明、监督执行计划、检视 diff、编写测试、创建评估循环、管理权限隔离，同时保留正确性、安全性、品味、可维护性。转折时间节点：2025年12月——在此之前 AI 编码 Agent "basically didn't work"，在此之后成为默认专业工作方式。核心金句："You can outsource your thinking, but you can't outsource your understanding." 未来招聘设想：让候选人现场用 AI Agent 构建完整项目、部署、安全加固，并抵御对抗性 Agent 的攻击测试。附例：Karpathy 自己做的 menugen（手机拍餐厅菜单→生成食物图片），上线数周后被 Gemini + Nanobanana 的原生多模态能力完全淘汰，不是更新了，是这类 App 整体被 Software 3.0 "吞噬"了。
- **Source**: https://karpathy.bearblog.dev/sequoia-ascent-2026/ | https://x.com/karpathy/status/2049903821095354523 | https://analyticsdrift.com/andrej-karpathy-agentic-engineering-software-3/ | https://www.franksworld.com/2026/05/01/andrej-karpathy-on-the-evolution-from-vibe-coding-to-agentic-engineering/
- **Timeliness**: 5 days ago（博客 + 推文：2026年4月30日；Sequoia 现场：4月29日）
- **Topic pillar**: AI 协作实践
- **Zico's angle**: 中文媒体的报道标题是"Karpathy 宣布 Vibe Coding 已死"，然后结束。整个框架的核心被截断了。Karpathy 说的不是"停止 vibe coding"，是"vibe coding 不够了，专业标准在这里"。这个"专业标准"的具体描述和 Zico 用 Claude Code 做 AI+3D 产品的工作方式高度吻合：写 CLAUDE.md 约束 AI 行为（管理权限）、设计评估循环（测试 diff 而非盲目接受生成代码）、在多个并行 Agent worktree 里做决策仲裁。Zico 的反直觉角度：Karpathy 说"2025年12月是转折点，之前 AI 编码 Agent 基本不能用"——这是他第一次给出一个明确的时间刻度。意味着：2025年12月之前用 AI 辅助编码的人，已经在不知不觉中落后于"可生产使用"的基线了。对于任何做 AI 产品的人，这个时间节点不应该只是技术史的注脚，而是 calibration 的锚点。Zico 对 menugen 例子的直接感受：做了一个 3D 家装设计功能，上线后三个月被另一家集成了多模态能力的工具"吃掉"了。这不是产品失败，这是 Software 3.0 的运行方式——它吞噬整个 App 类别，不会通知你。
- **Resonance hook**: Karpathy 说，他自己做的 App 在上线数周后被 Gemini 直接淘汰了——不是被竞争对手打败，而是这个 App 所在的整个类别被语言模型"吃掉"了。他管这叫 Software 3.0。他还说：vibe coding 提高了门槛，但 agentic engineering 才是专业标准，两者的距离比大多数人以为的要大得多。
- **Recommended priority**: high

---

## Candidate 2: Altman 说 AI 可以完全靠合成数据训练——他在说什么，他没说透什么

- **Event**: 2026年5月4日（昨日），MediaPost 发表深度分析文章《Sam Altman's Warning: AI Is Starting To Replace Reality》，引用 Altman 近期与记者 Nicholas Thompson（The Atlantic AI 编辑）的对话录像。Altman 明确表态："I believe you could get there entirely on synthetic data"（我认为完全靠合成数据就能训练出强大的模型）。Nicholas Thompson 在 Substack 跟帖写道："I was a little surprised by Sam Altman's answer here. But if he's right—and you can train a model completely on synthetic data—it would have all sorts of implications for how we develop and deploy this technology." 采访由 The Atlantic Re:think（The Atlantic 的品牌内容工作室）制作。MediaPost 的分析框架：如果 AI 不再需要人类经验作为训练地基，其输出将不再锚定于人类共享的现实——"We are building systems that generate reality, training them on increasingly synthetic inputs, and deploying them at global scale, without fully understanding how they arrive at their outputs or how those outputs will evolve over time." Altman 同时承认："We still don't have a great mechanistic understanding"（我们仍然不能很好地解释这些模型内部在发生什么）。
- **Source**: https://www.mediapost.com/publications/article/414802/sam-altmans-warning-ai-is-starting-to-replace-re.html | https://substack.com/@nxthompson/note/c-250987896
- **Timeliness**: 1 day ago（2026年5月4日）
- **Topic pillar**: 深层思考
- **Zico's angle**: 中文媒体会把这件事写成"OpenAI CEO 谈数据策略"，然后结束。但 Altman 这句话的潜台词更深：如果 AI 能完全从自己的输出中学习，它就不再是人类知识的镜像——它在建立自己的认知底座。Zico 的框架是"AI 是新物种，不是工具"——这个命题在 Altman 的话里找到了最直接的商业角度的表述。AI 作为工具的定义是：它处理人类产生的输入，返回人类能使用的输出；人类经验始终是地基。如果合成数据足够，地基变了——AI 产生的世界里，人类经验是可选项，而不是必要输入。这不是哲学虚构，它有直接的产品含义：内容生产（已经大量合成）、代码生成（AI 生成 → AI 测试 → AI 修复）、设计（AI 生成 → AI 评估 → AI 迭代）。每个环节都在循环收紧，人类的介入窗口在缩小。Nicholas Thompson 说"I was surprised"——他做 AI 报道多年，他知道这句话意味着什么。Altman 说了一句轻描淡写的话，把人类在 AI 训练链路里的地位从"必须的"变成了"此阶段的"。
- **Resonance hook**: Sam Altman 昨天说了一句话，Nicholas Thompson（The Atlantic AI 编辑）说自己"被惊到了"：AI 可以完全用合成数据训练，不需要人类产生的数据。如果这是真的，AI 不再从人类经验里学习——它开始从自己的输出里学习。人类在这个循环里的位置是什么？
- **Recommended priority**: high

---

## Candidate 3: AWS "What's Next 2026" 发布 Amazon Quick + 4 垂直 AI Agent 产品线——这是和 Microsoft、OpenAI 完全不同的胜法

- **Event**: 2026年4月28日，AWS 举办年度产品发布活动 "What's Next with AWS 2026"。核心公告三项：① **Amazon Quick 正式发布**：AI 工作助手，桌面 App（Preview）、免费/Plus 两档定价，无需 AWS 企业账号（用 Google/Apple/GitHub/Amazon 账号即可注册），接入 Google Workspace、Zoom、Airtable、Dropbox、Microsoft Teams、Google Drive，产品定位："connects to all of them, learns what matters to you, and takes action on your behalf"；② **Amazon Connect → 4 条垂直 AI Agent 产品线**：Amazon Connect Decisions（供应链决策 Agent）、Talent（招聘 Agent）、Customer（客户体验 Agent）、Health（医疗 Agent）——从单一联络中心平台拆分为四个领域专用自主 Agent；③ **AWS + OpenAI 合作扩展**：GPT-5.5 和 GPT-5.4 通过 Amazon Bedrock API 上线（Limited Preview）；Amazon Bedrock Managed Agents powered by OpenAI（Limited Preview）。AWS 发布年度回顾文章于2026年5月4日（昨日）。背景：OpenAI 于2026年4月27日正式终止与微软的7年独家授权协议，同日 AWS 即签约，4月28日在 "What's Next" 大会宣布产品细节。
- **Source**: https://aws.amazon.com/blogs/aws/aws-weekly-roundup-whats-next-with-aws-2026-amazon-quick-openai-partnership-and-more-may-4-2026/ | https://aws.amazon.com/blogs/aws/top-announcements-of-the-whats-next-with-aws-2026/ | https://futurumgroup.com/insights/aws-pushes-the-agent-stack-quick-connect-verticals-openai-on-amazon-bedrock/
- **Timeliness**: 7 days ago（事件：2026年4月28日）/ 1 day ago（AWS 周报：2026年5月4日）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 中文媒体的报道框架是"OpenAI 进驻 AWS，微软独家结束"，然后停在这里。真正的信号在 Amazon Connect 那部分：AWS 没有做通用 AI 助手，它把 Amazon Connect 拆成了四条垂直 Agent 产品线，每一条对应一个千亿美元市值的 SaaS 品类——供应链（SAP / Oracle 的地盘）、招聘（Workday 的地盘）、客户体验（Salesforce Service Cloud 的地盘）、医疗（Epic 的地盘）。这不是"给现有软件加 AI 功能"，这是"用自主 Agent 替代整个软件品类的核心功能"。微软走的是"控制平面"路线（Agent 365 = 管理所有 Agent 的基础设施）；OpenAI 走的是"通用智能"路线（Workspace Agents = 做任何工作的跨域助手）；AWS 走的是"垂直领域捕获"路线——我不需要是最聪明的 Agent，我只需要在你的具体行业里做得足够深，深到你的数据、流程、合规要求都跑在我上面，你没有理由切换。Amazon Quick（免费注册，不用企业账号）是 SMB 流量入口；Amazon Connect 四条垂直线是大客户护城河。两条线同时推进，是 AWS 在 Agent 经济里最清晰的战略表达。
- **Resonance hook**: AWS 上周发布会把 Amazon Connect 拆成了四个产品：供应链 Agent、招聘 Agent、客户体验 Agent、医疗 Agent。每一个对应一家市值千亿的 SaaS 公司的核心功能。AWS 不是在给这些公司做竞品，是在用 Agent 替换他们的主营业务。同时，Amazon Quick 用 Google/Apple 账号就能注册，不用买 AWS。这是两条同时推进的线。
- **Recommended priority**: medium（时效7天，略偏旧；但与4月30日 candidates Candidate 1 "微软-OpenAI 独家结束"是不同维度的故事，且 Amazon Connect 垂直 Agent 切入逻辑中文圈几乎零覆盖）

---

## Scan summary

**Sources scanned**:
- X/Twitter: Karpathy（Sequoia Ascent 2026 fireside chat + 博客4月30日，tweet status/2049903821095354523；Agentic Engineering 框架；vibe coding 一周年回顾）；Altman（synthetic data 采访片段 + MediaPost 分析5月4日）；Jim Fan（无7天内新锚点）；LeCun、Demis Hassabis（无7天内新锚点）；Swyx（Latent Space "Scaling without Slop" Jan 2026，超窗口）；Nat Friedman（5月4日 candidates 已纳入 Meta MSL）
- GitHub Trending: jcode（May 3，code agent toolkit，信息增量有限）；Superpowers agent framework（May 3，无明确事件锚点）；Craft Agents OSS（May 2，已在May3 candidates excluded）；caramaschiHG/awesome-ai-agents-2026（持续更新，无单点事件）
- Hacker News: 5月2-5日前页（Karpathy Agentic Engineering 讨论活跃；Altman synthetic data讨论；AWS What's Next 分析贴）
- Anthropic 官方博客: Claude 4 系列（Opus 4.7 April 16，19天前超窗口；Claude Design April 17，18天前超窗口）；Anthropic Release Notes May 2026（无7天内独立大事件未被前3天 candidates 覆盖）
- OpenAI 官方: Workspace Agents（April 22，13天前超7天窗口，且与April 30 candidates 微软-OpenAI 独家结束叙事链路相关，不重复）；Codex "for almost everything"（Major update，但无精确发布日期锚点确认为7天内）
- DeepMind / Google: Deep Research Max（April 21-22，13天前，已在April 30 candidates excluded）；Gemini 3.1 Ultra（更早，超窗口）
- AWS 官方博客: "What's Next with AWS 2026" top announcements（April 28 事件，May 4 发布周报）；Amazon Quick，Amazon Connect verticals，OpenAI on Bedrock
- MediaPost（May 4，2026）: 《Sam Altman's Warning: AI Is Starting To Replace Reality》；Nicholas Thompson Substack note
- arXiv cs.AI/cs.CV: Agentic World Modeling（2604.22748，April 24，已在April 30 candidates Candidate 3覆盖）；Hi-WM（2604.21741，April 30，已在May 4 candidates Candidate 3覆盖）；GSMem 3DGS spatial memory（2603.19137，March 2026，超7天窗口）；OpenUSD 26.03 3DGS 支持（March 2026，超7天窗口）；Pebblous 3DGS synthetic data for physical AI（April 2026 blog，无精确日期锚，暂排除）
- Air Street Press: "State of AI: May 2026"（分析综述，无单点事件锚）

**Total signals found**: 21 evaluated

**Why these 3**:
1. **Karpathy "Agentic Engineering"**（Candidate 1）：时效5天（4月30日），7天窗口内；Karpathy 是 Tier 1 必监控 KOL；"Agentic Engineering vs Vibe Coding"框架与4月30日 candidates 的 Karpathy CLAUDE.md-skills 故事（已选为 draft 010）完全不同维度——前者是"行为约束文件病毒式传播"，后者是"重新定义从业者专业标准"；中文媒体只在标题层面报道"vibe coding 已死"，框架本身中文零覆盖；AI 协作实践柱：May 3 候选已用 Anthropic+Blender（创意工具整合），不同方向，无重叠；Zico 的 Claude Code 日常工作方式本身就是 agentic engineering 的活案例，authenticity 护城河最强。

2. **Altman 合成数据/AI 认知基础**（Candidate 2）：时效最强（昨日5月4日）；Nicholas Thompson 的"I was surprised"为真实锚点（他是专业 AI 记者，surprised 就是信号）；The Atlantic Re:think 制作，来源可查；深层思考柱：May 4 用的是 Hi-WM（机器人物理训练），May 3 用的是 David Silver（Era of Experience），本篇是"AI 的认识论基础"，三者方向完全不同；中文媒体会做"Altman 谈数据"新闻，不会做"如果 AI 不需要人类经验，它在认识什么"这个哲学层面的推演；Zico 的"AI = 新物种"框架与此命题直接对接。

3. **AWS "What's Next 2026" + Amazon Quick + Connect 垂直 Agent**（Candidate 3）：时效7天（事件4月28日），在窗口边缘但 AWS 周报昨日发布给了新的出版锚点；4月30日 candidates 已覆盖"微软-OpenAI 独家终止"（战略层），本篇是"AWS 用这个机会做了什么"（产品层），角度不同；Agent 经济柱：May 4 是 Microsoft Agent 365（企业治理控制平面），本篇是 AWS 垂直领域捕获，两种完全不同的胜法叙事；中文媒体零覆盖 Amazon Connect 拆分为四条垂直 Agent 线的战略含义；企业 SaaS 替代逻辑（Workday/Salesforce/Epic 地盘被 Agent 直接攻击）是信息增量最高的角度。

**Excluded signals**:
- OpenAI Workspace Agents（4月22日）：13天前超7天窗口；且与4月30日候选的 OpenAI-微软重构故事链路相关，Zico 视角下重叠度高，排除
- Google Deep Research Max（4月21-22日）：4月30日 candidates 已 excluded（9天前），现已13天，继续排除
- OpenUSD 26.03 + 3DGS 标准化（3月2026年）：超出30天窗口
- GSMem 3DGS Spatial Memory（arXiv，March 2026）：超窗口
- Pebblous "3DGS for Physical AI" blog（April 2026）：无精确日期锚，且主题与May 4 Hi-WM 论文（机器人在世界模型内纠错）高度接近，不重复
- Karpathy-skills CLAUDE.md 95k stars（April 29-30）：4月30日 candidates Candidate 2已覆盖并选用为 draft 010，不重复
- Agentic World Modeling 2604.22748（April 24）：4月30日 candidates Candidate 3已覆盖，不重复
- Hi-WM 2604.21741（April 30）：May 4 candidates Candidate 3已覆盖，不重复
- Sam Altman "automated AI research intern by Sep 2026"：该声明来自2025年10月直播，非7天内事件，排除
- David Silver / Ineffable Intelligence（April 27）：May 3 candidates Candidate 1已覆盖（draft 012），不重复
- Claude Security public beta（April 30）：May 3 candidates Candidate 3已覆盖，不重复
- Meta 8000人裁员 + AI-pod（April 30 全员大会）：May 4 candidates Candidate 1已覆盖（draft 013），不重复
- Microsoft Agent 365 GA（May 1）：May 4 candidates Candidate 2已覆盖，不重复
