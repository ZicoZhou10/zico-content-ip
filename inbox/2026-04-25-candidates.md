---
date: 2026-04-25
status: written
selected: candidate 2 → drafts/006-world-model-wave-xhs.md
---

# Today's Candidates

## Candidate 1: GPT-5.5 发布，OpenAI 把它叫做通向"super app"的一步——这不是版本号，是平台战略宣言

- **Event**: 2026年4月23日，OpenAI 正式发布 GPT-5.5，面向 Plus、Pro、Business、Enterprise 用户全面上线；4月24日 API 公开访问。联合创始人兼总裁 Greg Brockman 公开表示，GPT-5.5 让 OpenAI "向 super app 更近了一步"——将 ChatGPT（消费者）、Codex（开发者）、AI 浏览器（操作系统层）统一成单一平台的愿景。模型分三个版本：GPT-5.5 标准、GPT-5.5 Thinking（扩展推理）、GPT-5.5 Pro（最高精度）。基准表现：FrontierMath Tier 4 得分 39.6%（Claude Opus 4.7 为 22.9%），Terminal-Bench 2.0 得分 82.7%（自主命令行任务执行能力）。距上一版 GPT-5.4 仅六周。
- **Source**: https://openai.com/index/introducing-gpt-5-5/ | https://techcrunch.com/2026/04/23/openai-chatgpt-gpt-5-5-ai-model-superapp/ | https://siliconangle.com/2026/04/23/openai-releases-gpt-5-5-advanced-math-coding-capabilities/
- **Timeliness**: 2 days ago（2026年4月23日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 中文媒体铺天盖地在分析跑分。但 Brockman 说的"super app"才是真正有信息量的信号。OpenAI 不是在宣布一个更好的模型，是在宣布一个平台战略目标：把 ChatGPT（消费者入口）、Codex（开发者工具）、AI 浏览器（系统层控制）合并成统一平台。这是在追 iPhone 时刻——控制运行时环境、分发渠道、付费机制。Anthropic 的策略是"做最好的模型，让企业主动来找你"（Claude Code 是基础设施，不是超级应用）；OpenAI 的策略正在变成"成为 AI 时代的 iOS"。两种截然不同的产品哲学，背后是两种完全不同的竞争判断：前者押注的是"AI 能力稀缺"，后者押注的是"分发和用户习惯才是护城河"。从产品战略角度，这比任何跑分都值得认真想。
- **Resonance hook**: 跑分中文圈已经分析到位了。但没人说清楚 Greg Brockman 为什么在发布一个模型的时候用"super app"这个词——这是平台战略宣言，不是功能公告。
- **Recommended priority**: high

---

## Candidate 2: Tencent 和 Alibaba 在同一天发布世界模型——下一波 AI，中国不是陪跑

- **Event**: 2026年4月16日，Tencent 开源 HY-World 2.0（arXiv: 2604.14268），一个基于 3D Gaussian Splatting（3DGS）的多模态世界模型，支持文本/单张图像/多视角/视频输入，生成可导航的三维场景，集重建、生成、仿真于一体。同日，Alibaba 发布 Happy Oyster，一个面向游戏/影视的交互式世界模型，支持实时导演模式（Directing mode）控制生成世界。4月14日，Nvidia 发布 Cosmos Predict 2.5 和 Cosmos Reason 2，用于物理 AI 合成数据生成和机器人策略评估，Agility Robotics、Figure AI、Uber 等已在接入。4月23日，Bloomberg 发表文章《World Models Understand Space and Physics ChatGPT and Claude Can't Grasp》，指出不到两周内 Nvidia、Alibaba、Tencent 三家公司集中发布世界模型，并明确指出中国在这一赛道"不像大语言模型时代那样落后"。
- **Source**: https://arxiv.org/abs/2604.14268 | https://www.bloomberg.com/opinion/articles/2026-04-23/world-models-understand-space-and-physics-chatgpt-and-claude-can-t-grasp | https://www.buildfastwithai.com/blogs/tencent-alibaba-world-models-april-2026 | https://nvidianews.nvidia.com/news/nvidia-announces-major-release-of-cosmos-world-foundation-models-and-physical-ai-data-tools
- **Timeliness**: 2 days ago（Bloomberg 综述文章：4月23日；模型发布：4月14–16日，9–11天前）
- **Topic pillar**: 深层思考（与空间智能前沿交叉）
- **Zico's angle**: 我在做 3DGS 产品，所以我知道世界模型不是"又一个大模型"，而是一个架构层面完全不同的东西。LLM 在预测下一个 token；World Model 在预测下一个状态——空间、物理、时间。ChatGPT 理解不了一个房间的深度关系；HY-World 2.0 用 3DGS 直接生成可导航的三维场景。Bloomberg 说的那个缺口——"ChatGPT 和 Claude 无法理解空间和物理"——不是 LLM 的 bug，是 LLM 架构的基本上限。这意味着存在一整个能力维度，LLM 的军备竞赛无论打多激烈都无法触及。更值得关注的是：Tencent 和 Alibaba 在同一天发布了世界模型，Nvidia 两天前刚刚发布了物理 AI 基础设施。这是一个集体涌现的信号，不是散点。而在这个赛道上，中国公司和美国公司的起跑线更接近。LLM 时代，中文圈追了很久；World Model 时代，起跑线不一样了。
- **Resonance hook**: Tencent 和 Alibaba 在同一天发布了世界模型。Bloomberg 说这类 AI 能理解空间和物理，但 ChatGPT 和 Claude 做不到。这不是跑分竞争，是 AI 能力的另一个维度——中国这次不是在追跑。
- **Recommended priority**: high

---

## Candidate 3: OpenAI 用 Infosys、TCS、Accenture 来卖 Codex——正在给自己造一个结构性矛盾的渠道

- **Event**: 2026年4月21日，OpenAI 宣布与 Accenture、Capgemini、CGI、Cognizant、Infosys、PwC、塔塔咨询（TCS）七家全球最大咨询公司/系统集成商达成合作，共同推动大型企业部署 Codex。同时正式启动 Codex Labs——OpenAI 自有专家驻场进入客户企业内部，直接协助集成和落地。背景数据：Codex 周活跃开发者从 3 月的 300 万增至 4 月初的 400 万；OpenAI 在公告中说"需求增速已超过我们帮客户落地的能力"（"The demand we're seeing is outpacing our ability to help enterprises adopt Codex as quickly as they'd like"）。4月22日，Infosys 同步发出独立新闻稿，宣布与 OpenAI 的"战略合作协议"。
- **Source**: https://openai.com/index/scaling-codex-to-enterprises-worldwide/ | https://techcrunch.com/2026/04/22/openai-teams-up-with-infosys-to-bring-ai-tools-to-more-businesses/ | https://finance.yahoo.com/sectors/technology/articles/openai-leans-global-consultancies-expand-135737223.html
- **Timeliness**: 4 days ago（4月21日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: Infosys、TCS、Cognizant——这些公司靠"替企业提供大批量软件工程师"活了几十年。它们的商业模式是人头乘以工时。Codex 的核心价值是减少这些人头。OpenAI 现在用这些公司作为分销渠道——经典的"借助老渠道颠覆老渠道"策略。但结构性张力非常清晰：咨询公司帮客户买了 Codex → 客户的工程成本下降 → 客户未来需要的咨询时数也下降 → 咨询公司给自己掘了坑。这不是第一次（云计算转型时咨询公司卖 Salesforce 也经历过相似的逻辑），但这次破坏速度更快，影响更深。更有意思的是 Codex Labs 这个动作——OpenAI 自己的专家进驻企业，绕过咨询公司直接触达客户。表面上是合作，实际上是两条腿走路：一条用渠道扩张，一条用自营卡住关键账户。从组织设计角度：这个渠道战略的生命周期大概是多长？当咨询公司意识到这件事，他们会怎么反应？
- **Resonance hook**: OpenAI 找了全球最大的 IT 外包公司来卖 Codex——而 Codex 的核心价值，就是减少这些公司赖以生存的人头需求。没人说这件事里的结构性矛盾。
- **Recommended priority**: medium

---

## Scan summary

**Sources scanned**:
- X/Twitter: Karpathy（second brain follow-up、growing gap in AI capability）、Altman（Hollywood remarks、Jakub quote）相关近期推文
- GitHub Trending: 2026-04-22 weekly report（shareuhack.com），agents-radar issue #652（2026-04-19）
- Hacker News: 2026-04-22、04-23 首页（news.ycombinator.com）
- OpenAI 官方博客: introducing-gpt-5-5（4月23日）、scaling-codex-to-enterprises-worldwide（4月21日）
- Anthropic 官方博客/发布说明: Managed Agents（4月8日）、Claude Design（4月初）— 已排除（超过7天）
- Google Cloud Blog: A2A v1.2、Gemini Enterprise Agent Platform — 已排除（前两天已选用）
- DeepMind: 无新发布
- arXiv: HY-World 2.0（2604.14268，4月16日）、TEMPO test-time training（4月21日）、Scaling Self-Play with Self-Guidance（4月22日）
- Bloomberg: "World Models Understand Space and Physics"（4月23日）
- TechCrunch、CNBC、SiliconAngle、Reuters: GPT-5.5 报道（4月23–24日）、Codex/Infosys（4月22日）
- Nvidia Newsroom: Cosmos Predict 2.5 / Cosmos Reason 2（4月14日）
- Hugging Face Papers: HY-World 2.0（4月16日）

**Total signals found**: 14 evaluated

**Why these 3**:
- **Candidate 1（GPT-5.5 Super App）**：时效最强（2天），中文圈大量报道跑分但无人拆解"super app"平台战略含义，直接命中 AI 产品战略柱，Zico 有能力从产品哲学层面切入。
- **Candidate 2（世界模型浪潮）**：Bloomberg 综述锚点（2天），一周内 Nvidia + Alibaba + Tencent 集中发布构成趋势信号，命中深层思考/空间智能柱，Zico 3DGS 一线经验赋予真实第一视角，信息差极大（中文圈几乎无严肃分析）。
- **Candidate 3（Codex Labs + 咨询渠道）**：时效良好（4天），OpenAI 公告本身清晰，Infosys/TCS/Accenture 的渠道悖论是组织形式变革柱的具体落地案例，中文圈讨论此事几乎为零。

**Excluded signals**:
- Anthropic Managed Agents（4月8日）：超出7天窗口，且更接近开发者工具而非 Zico 内容策略核心主题，排除。
- Karpathy "growing gap in AI capability"推文：内容有价值，但无法确认精确发布日期在7天内；且 Karpathy 内容已在 draft 003 使用，避免重复，排除。
- TEMPO test-time training arXiv（4月21日）：技术价值高，但缺乏足够强的叙事锚点，Zico 角度难以形成有共鸣的内容，排除。
- Google Cloud Next A2A v1.2 / Workspace Agents / Demis Hassabis：均已出现在4月23日或4月24日候选，排除。
- Anthropic Mythos breach：已在4月23日候选中使用，排除。
