---
date: 2026-04-30
status: written
selected: candidate 2 → drafts/010-behavior-programming-xhs.md
---

# Today's Candidates

## Candidate 1: OpenAI 结束与微软 7 年独家协议——次日模型已上架 AWS

- **Event**: 2026年4月27日，Microsoft 和 OpenAI 联合发布声明，宣布重构合作协议：微软放弃对 OpenAI 模型和产品的独家授权权利，OpenAI 可自由向所有云服务商（AWS、Google Cloud 等）分发产品。微软保留 OpenAI IP 的非独家授权至2032年；OpenAI 继续向微软支付收益分成（上限至2030年），但微软同时停止向 OpenAI 支付收益分成——双向支付关系翻转。背景：2026年2月，OpenAI 宣布500亿美元 Amazon 投资协议，与微软的独家条款产生法律冲突；此次重构是对该冲突的合规化处理。TechCrunch 标题直接点出：《OpenAI ends Microsoft legal peril over its $50B Amazon deal》。4月28日，CNBC 报道"OpenAI brings its models to Amazon's cloud after ending exclusivity with Microsoft"——重构公告次日，OpenAI 模型已完成 AWS 上架。"Azure 优先"条款保留：OpenAI 产品仍将优先在 Azure 上线，但不再是唯一选项。eWeek 标题：《Microsoft, OpenAI Rewrote Their Marriage Contract》。Dataconomy（4月29日）进一步报道 AWS 端具体产品上架细节。
- **Source**: https://blogs.microsoft.com/blog/2026/04/27/the-next-phase-of-the-microsoft-openai-partnership/ | https://openai.com/index/next-phase-of-microsoft-partnership/ | https://www.cnbc.com/2026/04/27/openai-microsoft-partnership-revenue-cap.html | https://techcrunch.com/2026/04/27/openai-ends-microsoft-legal-peril-over-its-50b-amazon-deal/ | https://www.cnbc.com/2026/04/28/openai-brings-models-to-aws-after-ending-exclusivity-with-microsoft.html | https://dataconomy.com/2026/04/29/openai-expands-to-aws-as-microsoft-exclusivity-ends/
- **Timeliness**: 3 days ago（2026年4月27日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 中文媒体的报道框架是"微软与 OpenAI 分手/独家关系结束"，然后就结束了。但战略信号要重要得多。2019年微软花10亿美元买到独家权利，之后七年累计投入约130亿美元。2026年4月，这个独家权利终止——不是因为微软做错了什么，而是因为 OpenAI 的多云分发战略比单一云独家授权更有价值。精确的战略读法：OpenAI 正在成为一个"模型层"，悬浮在所有云平台之上，不依附于任何一个。Anthropic 走的是同样的路径（$100B AWS 承诺 + 同时可用于 Google Cloud + Azure）。模型公司在赢得分发战争，云巨头从"独家战略伙伴"退化为"非独家基础设施"。微软花了130亿美元，最终拿到的是一张有效期到2032年的非独家授权——这个结果对理解 AI 分发权力结构极其清晰。对中国 AI 格局的直接参照：百度文心、阿里通义、字节豆包的云绑定策略在这个框架下应该如何评估？如果模型足够强，不被任何单一云绑住才是正确的分发战略。
- **Resonance hook**: 微软花了7年、约130亿美元，买到的独家授权3天前到期了。OpenAI 选择终止它，不是因为背叛，而是因为：在 AI 分发战争里，单一云独家已经不如多云触达更值钱。这个选择背后有一个关于谁控制 AI 最后一公里的清晰判断。
- **Recommended priority**: high

---

## Candidate 2: 1KB 的文本文件，9.5 万开发者下载——Karpathy 的 LLM 编码原则在 Claude Code 社群引爆

- **Event**: 2026年4月29日，BrightCoding 发表文章《Karpathy Skills: The LLM Coding Manifesto》，记录 GitHub 仓库 forrestchang/andrej-karpathy-skills 的病毒式传播：95,400 stars、9,200 forks，ClaudePluginHub 收录并列为推荐插件。该仓库由开发者 Forrest Chang 创建，将 Andrej Karpathy 于2026年1月26日在 X 发布的 LLM 编码失败模式观察，浓缩为单一 CLAUDE.md 文件——零代码，只有四条行为原则，可直接安装为 Claude Code Skills 插件。四条原则：不假设（Explicit assumptions over silent interpretation）、不隐藏困惑（Ask when uncertain, never guess）、暴露取舍（Surface tradeoffs without picking silently）、强成功标准（Verifiable success criteria that let the LLM loop independently）。社区在此基础上继续扩展：gist renezander030/2898eb5f 发布"karpathy-skills CLAUDE.md v2"，加入从构建真实项目中提炼的新原则；alphasignalai substack 推荐"30秒安装到任意项目"。
- **Source**: https://www.blog.brightcoding.dev/2026/04/29/karpathy-skills-the-revolutionary-llm-coding-manifesto | https://github.com/forrestchang/andrej-karpathy-skills | https://github.com/forrestchang/andrej-karpathy-skills/blob/main/CLAUDE.md | https://www.claudepluginhub.com/plugins/forrestchang-andrej-karpathy-skills | https://alphasignalai.substack.com/p/karpathy-inspired-claudemd-how-to
- **Timeliness**: 1 day ago（BrightCoding 分析文章：2026年4月29日；仓库持续活跃至今日）
- **Topic pillar**: AI 协作实践
- **Zico's angle**: 中文 AI 开发者社区几乎没有覆盖这件事。值得认真想的问题是：为什么一个1KB的文本文件在 AI 开发者社群里成为最热的"工具"之一？Karpathy 的核心观察：LLM 是"充满自信的初级工程师"——它不会说"我不知道"，它会默默假设你的意图然后继续写代码。CLAUDE.md 的解法是：用文字编程 AI 的行为，而不是用代码。这是 AI-Native 开发工作流的一个核心洞察：你在"对齐 AI 行为"上投入的时间，回报远高于学一个新工具。9.5万个项目下载了这个文件，意味着整个 Claude Code 社群已经收敛到同一个答案：模型能力不等于任务质量，差距在指令质量。这件事也有更深一层的含义：当最流行的"开发者工具"变成一个原则声明文件，编程的边界已经在移动——从写代码，到写约束 AI 的规则。
- **Resonance hook**: Karpathy 说 LLM 编码有四个典型失败模式。一个叫 Forrest Chang 的开发者把这四条原则写成了一个文件。9.5万个人下载了它。当年最流行的"开发者工具"，变成了一个 .md 文件。
- **Recommended priority**: high

---

## Candidate 3: "代理式世界建模"系统综述——AI Agent 失败的根本原因，有了更精确的名字

- **Event**: 2026年4月24日，arXiv 论文 2604.22748《Agentic World Modeling: Foundations, Capabilities, Laws, and Beyond》发布，综合400余项研究提出"层级 × 定律"二维分类框架。三个能力层级：L1 预测器（学习单步本地转换算子，当前主流大模型）；L2 模拟器（组合多步动作条件 rollout，部分当前 AI Agent）；L3 进化器（当预测与新证据冲突时，自主修订自身世界模型，研究前沿）。四类定律体系：物理定律 / 数字定律 / 社会定律 / 科学定律。论文覆盖100+代表性系统，涵盖模型化强化学习、视频生成模型、Web/GUI Agent、多智能体社会模拟、AI驱动科学发现，并提出以决策为中心的评估原则。伴随 GitHub 仓库 matrix-agent/awesome-agentic-world-modeling 同步上线；HuggingFace 论文主页已收录。
- **Source**: https://arxiv.org/abs/2604.22748 | https://huggingface.co/papers/2604.22748 | https://github.com/matrix-agent/awesome-agentic-world-modeling
- **Timeliness**: 6 days ago（2026年4月24日）
- **Topic pillar**: 深层思考（与 Agent 经济、空间智能前沿交叉）
- **Zico's angle**: 这篇论文在 AI 学术圈以外几乎没有中文报道。但它提供了一个理解当前 AI Agent 为何频繁失败的精确框架。当前被部署为"Agent"的大多数 AI 其实是 L1 到 L2——它们能预测下一步，也能模拟多步流程，但当现实世界的状态与它们内部的世界模型不符时，它们不会更新模型，它们只会用错误的地图继续行动。这是当前 AI Agent 最常见、最难调试的失败模式的准确描述。L3 进化器的真正意义在于：它不仅是"更聪明的 Agent"，它是一个会自我纠错的系统——可以在新证据出现时修订自己对世界的整体理解。从 Zico 做空间智能产品的实战角度，这个框架有直接的投射：一个 L2 级的3D空间设计工具可以模拟家具摆放方案；一个 L3 级的系统在用户说"这不对，我家的墙是斜的"后，能修订自己对整个空间的建模，而不是重新从头跑一次推理。空间 AI 从 L2 到 L3 的跨越，是当前实体 AI 最难啃也最有价值的方向。当前大多数 Agent 产品声称自己在做"世界模型"——这篇论文给了一把精确的尺子。
- **Resonance hook**: 现在大多数 AI Agent 用的是 L1 或 L2 的世界模型——它们能预测、能模拟，但当它们的内部模型是错的，它们不知道。这篇综合了400多项研究的论文定义了 L3：一个当预测失败时，能自主修订自己世界模型的系统。当前 AI Agent 频繁出错的根本原因，有了一个更精确的名字。
- **Recommended priority**: medium

---

## Scan summary

- **Sources scanned**: X/Twitter（Karpathy: skills CLAUDE.md 相关，vibe coding，autoresearch；Altman/OpenAI: Musk 庭审 Day 2 4月29日；Microsoft X: 4月27日 partnership 公告）、GitHub Trending（forrestchang/andrej-karpathy-skills 95.4k stars；matrix-agent/awesome-agentic-world-modeling 新上线；karpathy/autoresearch 已用 draft 003）、Hacker News 4月28-30日前页（Musk 庭审 Day 2；OpenAI-微软重构讨论；Karpathy skills 讨论）、Anthropic 官方博客（Claude Cowork GA 4月9日，21天前超窗口；Anthropic-Amazon 5GW 4月20日，10天前）、OpenAI 官方博客（"next phase of Microsoft partnership" 4月27日；GPT-5.5 4月23日，已覆盖前期）、Microsoft 官方博客（"next phase of the Microsoft-OpenAI partnership" 4月27日）、Bloomberg/CNBC/TechCrunch/eWeek（Microsoft-OpenAI 重构 4月27-28日）、BrightCoding（"Karpathy Skills: The LLM Coding Manifesto" 4月29日）、arXiv cs.AI（Agentic World Modeling 2604.22748 4月24日；Agent-World 2604.18292 4月20日）、Google DeepMind（Deep Research Max 4月21日；Accenture 合作 4月22日）、NVIDIA Blog（National Robotics Week 4月中旬，超7天窗口）、HuggingFace（Tencent HY-Embodied-0.5 4月9日，超窗口）
- **Total signals found**: 18 evaluated
- **Why these 3**:
  - **Candidate 1（Microsoft-OpenAI 独家结束）**：时效3天，双方官方博客 + CNBC + Bloomberg + TechCrunch 全覆盖，次日 OpenAI 模型上架 AWS 构成清晰执行锚点；中文媒体框架是"分手"，真正的战略信号是"模型层悬浮于多云之上"——完全不同的解读框架；AI 产品战略柱近3天未使用（4月29日 Candidate 2 是 Claude Design，4月28日 Candidate 2 是 Apple/Gemini，方向均不同）；中国 AI 云生态类比赋予独特地域共鸣价值。
  - **Candidate 2（Karpathy-skills CLAUDE.md 病毒式传播）**：时效最强（1天），BrightCoding 4月29日专文；95.4k stars/9.2k forks 是可量化的社群收敛信号；中文 AI 开发者社区几乎零覆盖；Zico 实际使用 Claude Code 的一线经验提供不可复制可信度；与 draft 003（Karpathy 第二大脑 = 知识管理）主题完全不同（本篇 = 编码行为约束），AI 协作实践柱近3天未使用。
  - **Candidate 3（Agentic World Modeling）**：时效6天，在7天窗口内；中文社媒覆盖率近零；L1/L2/L3 分类框架是罕见的"让 AI Agent 失败原因可命名、可沟通"的工具；深层思考柱（4月29日 Candidate 1 是 DeepMind 雇哲学家，完全不同议题）；Zico 空间智能 + 3DGS 实战背景使 L2→L3 空间 AI 投射具有真实性。

- **Excluded signals**:
  - Musk 庭审 Day 2（4月29日）：与4月28日已选 Candidate 1（庭审 Day 1 → draft 009-mission-paradox）高度重叠，连续两天同一事件，排除。
  - Google Deep Research Max（4月21日）：9天前略超理想窗口；中文圈已有零散报道；AI 产品战略柱被 Candidate 1 占用，排除。
  - Anthropic-Amazon 5GW/33B 计算合作（4月20日）：10天前超窗口；"AI 基础设施投入"主题与 Candidate 1（OpenAI 多云分发战略）存在概念重叠，排除。
  - Claude Cowork GA（4月9日）：21天前，超出合理窗口，排除。
  - Tencent HY-Embodied-0.5（4月9日）：21天前，时效弱，排除。
  - NVIDIA National Robotics Week（4月中旬）：约2周前，超7天窗口，排除。
  - Agent-World 2604.18292（4月20日）：10天前，且与 Candidate 3（2604.22748，4月24日）主题高度接近，后者更新，保留后者排除前者。
