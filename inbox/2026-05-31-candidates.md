---
date: 2026-05-31
status: pending_selection
---

# Today's Candidates

## Candidate 1: 一家企业一个月烧掉 $5 亿在 Claude 上——因为没给 Agent 工作流设用量上限（May 28–29）

- **Event**: 2026年5月28–29日，一名 AI 顾问公开披露：其企业客户在没有设任何用量上限的情况下，**30 天内**在 Anthropic Claude 上产生了超过 **$5 亿（$500 million）** 的账单。机制：员工获得无限制访问后，大量工作负载迁移到 Agent 形态（software development agents、自主管道），Agent 在自动化循环中运行，单次任务的 token 消耗量最高是普通线性对话的 **1000 倍**。并行事件：① **Uber** 将 Claude Code 部署给 5,000 名工程师，到2026年4月月均使用率 84–95%，每名工程师月均 API 费 $500–$2,000，在**4个月内**耗尽全年 **$34 亿 AI 预算**；② **Microsoft** 2025年12月将 Claude Code 推广至 Experiences & Devices 部门（Windows、Microsoft 365、Outlook、Teams、Surface），工程师用量超标，2026年5月14日宣布截至6月30日取消该部门大多数 Claude Code 许可证，转向 GitHub Copilot CLI。来源：Tech Startups（May 28，首发）、BusinessToday（May 29）、Yahoo Finance（May 29）、Windows Central（Microsoft 取消细节）、The Next Web（May 29，企业 AI 成本深度报道）。
- **Source**: https://techstartups.com/2026/05/28/company-accidentally-spent-500-million-on-claude-ai-in-one-month-after-forgetting-usage-limits/ | https://www.businesstoday.in/technology/artificial-intelligence/story/ai-spending-nightmare-companies-spend-over-a-500-million-in-30-days-on-anthropics-claude-533824-2026-05-29 | https://www.windowscentral.com/microsoft/microsoft-cancels-claude-code-licenses-shifting-developers-to-github-copilot-cli-a-move-likely-driven-by-financial-motives | https://thenextweb.com/news/microsoft-claude-code-retreat-ai-cost
- **Timeliness**: 2–3 days ago（Tech Startups: May 28；BusinessToday: May 29）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 中文媒体的报道会停在"$5 亿太荒唐了"这一层。值得停下来看的是：**这不是治理错误，是架构错误**。

  传统 IT 采购的所有控制机制——每席位授权、月度预算、年度框架——设计在一个假设下：人类以人的速度使用软件。一个人一个月能发多少条消息，有上限的。

  Agent 不是这样运作的。Agent 在自动化循环里运行，不等待人类确认，不停下来问"继续吗"。一个软件开发 Agent 处理一个 ticket，后台可以并行启动多个子 Agent，每个再调用代码执行器、测试框架、文档检索。**单次任务的 token 消耗是普通对话的最高 1000 倍**。

  Uber 四个月烧完全年 $34 亿，Microsoft 工程师把全年额度烧光，无名客户一个月烧 $5 亿——三件事发生在同一季度，不是巧合。这是企业 AI 采购进入 Agent 时代后必然遭遇的第一批账单。

  问题不是"应不应该设上限"——这人都知道。问题是：**谁在公司内部负责为 Agent 工作流建立用量模型？** CTO 团队设计了工作流，IT 采购团队签了合同，Finance 以为这是 SaaS 年费。没有一个人全程看到这条链路。这是组织结构里的一个新盲区，不是某个人犯了错。
- **Resonance hook**: 2026年5月29日，一名 AI 顾问披露：一家企业客户在没给员工设任何 AI 用量上限的情况下，一个月在 Claude 上花了 $5 亿。同一个季度，Uber 四个月烧完了全年 $34 亿 AI 预算；Microsoft 因为工程师用量超标，取消了整个 Windows/Office 部门的 Claude Code 许可。这不是三个人犯了同一个错——是同一个架构缺陷在三家公司同时撞墙。
- **Recommended priority**: high

---

## Candidate 2: KPMG 把 Claude 部署给全球 276,000 名员工——"powered by Claude"出现在客户合同级的交付物里（May 20）

- **Event**: 2026年5月20日，**Anthropic** 与 **KPMG** 宣布全球战略联盟，KPMG 将 Claude 集成进 **Digital Gateway**——KPMG 做实际客户工作的核心交付平台。覆盖规模：**138 个国家，276,000 名员工**，全员获得 Claude 访问权限，直接集成在业务工作流中。实施路径：**Tax & Legal 先行，再扩展 Advisory，再覆盖全业务线；完整实施目标：2026年9月**。这是专业服务业迄今规模最大的企业级 AI 全员部署。Fortune 5月26日深度报道《Big Four consulting has 2 AI nightmares. KPMG's answer to both is the same》援引 KPMG 高管：Claude 将嵌入 KPMG 向客户交付工作成果的实际工具，并以 **"powered by Claude"** 标识对外展示。来源：Anthropic 官方博客（May 20）、Fortune（May 26，深度报道）、ResultSense（May 20）、Investing.com。
- **Source**: https://www.anthropic.com/news/anthropic-kpmg | https://fortune.com/2026/05/26/kpmg-anthropic-claude-partnership-big-four-ai/ | https://www.resultsense.com/news/2026-05-20-anthropic-kpmg-276k-alliance/
- **Timeliness**: 11 days ago（Anthropic 官方：May 20；Fortune 跟进：May 26）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 大多数"AI 改变职场"的报道停在"AI 工具帮员工提效"这层。KPMG 这个决定说的不是这件事。

  KPMG 把 Claude 嵌进的是 **Digital Gateway**——这是他们做实际客户工作的平台，不是员工可以选择用或不用的辅助工具。Tax & Legal 的员工在 Digital Gateway 里完成税务申报、法律尽调、合规报告。现在 Claude 在里面，不是旁路工具，是工作流的组成部分。

  关键信号：KPMG 对外的标识是"powered by Claude"——这意味着客户合同级别的交付物里，AI 是一个有名字的生产方。不只是内部用 AI，而是向客户承诺这件事。

  这是 **AI 改变组织形式三阶段** 里第三阶段开始清晰的信号：第一阶段，AI 作为个人工具（员工自选 ChatGPT）；第二阶段，AI 集成进工作流（公司采购 Copilot 嵌入 Office）；**第三阶段，AI 成为交付物的生产方之一，客户合同级别可见**。KPMG 是目前我看到的第三阶段最清晰的企业案例。

  Tax & Legal 先行，不是随机选择。这类工作流的特点：高度重复、依赖结构化知识、合规标准明确。AI 承接的逻辑不是"节省时间"，而是"AI 的覆盖面和一致性超过了人工的性价比"。276,000 人，138 个国家，9月全员上线——这个时间表是认真的。
- **Resonance hook**: 2026年5月20日，KPMG 宣布把 Claude 部署给全球 276,000 名员工，直接集成在实际做客户工作的平台里。不是试点，不是选配，是 138 个国家全员，从税务和法律开始，2026年9月全线上线。KPMG 对外展示的标识是"powered by Claude"——客户看到的交付物里，AI 已经是一个有名字的生产方。Big 4 会计师事务所里，第一次。
- **Recommended priority**: high

---

## Candidate 3: Google 把训练 Waymo 机器人的世界模型，开放给了付 $200/月的普通用户——物理 AI 基础设施开始平民化（May 19–20）

- **Event**: 2026年5月19–20日，**Google I/O 2026** 期间，**Google DeepMind** 宣布将 **Genie 3** 的 **Street View grounding** 功能面向全球开放，入口：**Google AI Ultra 订阅，$200/月**。Genie 3 是 DeepMind 建立在 **2800 亿张 Google Street View 照片** 上的通用世界模型，能基于真实地理位置生成**可导航的交互式 3D 环境**，并同步输出 **2D 视频和 3D 激光雷达数据**。**Waymo 连接**：这套 Genie 3 架构已经是 **Waymo** 自动驾驶训练系统的组成部分。Waymo 用它生成自动驾驶车辆在现实中极难遇到的稀有场景——龙卷风、动物横穿高速公路、多系统同时故障——并在虚拟环境中训练自动驾驶模型，同步生成摄像头和激光雷达的双模态训练数据。**新开放的能力**：Street View grounding 允许将视角切换至其他 Agent（行人、骑手、外卖机器人），为多 Agent 场景训练提供基础——这是目前以汽车为中心的模拟器无法做到的。来源：Techtimes（May 20）、The-Decoder、Sci-Tech Today、Automotive World、Google DeepMind 官方。
- **Source**: https://www.techtimes.com/articles/316902/20260520/genie-3-trains-waymos-robotaxis-rare-scenarios-street-view-grounding-now-global-200-ultra.htm | https://the-decoder.com/waymo-taps-google-deepminds-genie-3-to-simulate-driving-scenarios-its-cars-have-never-seen/ | https://www.sci-tech-today.com/news/waymo-deepmind-genie-3/ | https://www.automotiveworld.com/news/waymo-unveils-deepmind-powered-world-simulation-model/
- **Timeliness**: 11 days ago（2026年5月19–20日，Google I/O 2026）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: 中文媒体报道 Google I/O 会聚焦 Gemini 新模型和消费者功能。Genie 3 会被提到，但通常被描述为"酷炫 AI 演示"。报道里最重要的东西不是消费者产品，是**基础设施路径**。

  Waymo 用 Genie 3 解决了一个具体问题：自动驾驶训练数据里，稀有危险场景的样本不够，现实中收集这类数据既危险又无法系统化。Genie 3 的解法是：用一个世界模型**生成这些场景的高保真模拟**——同步输出 2D 视频和 3D 激光雷达数据，逼真到可以作为训练数据。

  新的是：**Google 把训练 Waymo 机器人的基础设施，开放给了 $200/月的订阅用户**。不是一个独立的消费者产品——是同一套 Genie 3 架构，建立在 2800 亿张真实地理位置照片上的世界模型，现在任何人可以用它构建基于真实地点的可导航 3D 环境。

  这是一个我见过不多次的路径转折：一个先服务于机器人训练的基础设施，开始以 API 形式向下渗透。类比：AWS 最初是亚马逊自己的后端基础设施，后来开放成了云计算行业的基础设施。Genie 3 正在走一条类似的路——只不过处理的不是计算资源，而是**真实物理世界的先验知识**。

  在 3DGS 和 NeRF 这两条技术路线上，我一直在思考的一个问题是：空间 AI 的护城河最终在哪里？Genie 3 给出了一个答案的方向：2800 亿张照片积累的地理先验知识，不是任何一家公司可以重建的。物理 AI 的竞争，可能最终不是模型架构的竞争，而是**谁覆盖的真实世界更完整**的竞争。
- **Resonance hook**: 2026年5月19日，Google DeepMind 宣布 Genie 3 的 Street View grounding 向 $200/月的 Google AI Ultra 用户开放。这套系统已经在给 Waymo 的自动驾驶 AI 训练"龙卷风""动物横穿高速"这类稀有场景。2800 亿张真实地理位置照片 × 世界模型 = 可导航的物理世界数字孪生。Waymo 用它训练机器人，现在 $200/月可以访问同一套基础设施。物理 AI 的训练数据层，正在经历和 LLM API 相同的平民化过程。
- **Recommended priority**: medium

---

## Scan summary

**Sources scanned**:
- Tech Startups（May 28，$500M Claude billing incident 首发）
- BusinessToday（May 29，$500M 账单确认报道）
- Yahoo Finance（May 29，$500M 账单及机制分析）
- The Next Web（May 29，Microsoft Claude Code retreat 深度报道）
- Windows Central（May 2026，Microsoft 取消 Claude Code 许可细节）
- People Matters（May 2026，Microsoft Claude Code cancellation 确认）
- AI Weekly（Microsoft drops Claude Code after budget overrun 确认）
- Anthropic 官方博客（May 20，KPMG 战略联盟公告）
- Fortune（May 26，《Big Four consulting has 2 AI nightmares》深度报道）
- ResultSense（May 20，KPMG Anthropic 联盟 276K 数据确认）
- Investing.com（KPMG 276K 部署独立确认）
- Techtimes（May 20，Genie 3 + Waymo 自动驾驶 + Street View 开放首报）
- The-Decoder（Waymo taps DeepMind's Genie 3 驾驶场景生成 深度报道）
- Sci-Tech Today（Waymo + DeepMind Genie 3 技术细节确认）
- Automotive World（Waymo world model DeepMind powered 独立确认）
- BuildFastWithAI（May 30，AI news roundup — "enterprise AI cost reckoning"叙事验证）
- Karpathy X（May 19 加入 Anthropic，已在 May 19-20 candidates 覆盖，排除）
- Sam Altman（May 26 jobs walk-back，已在 May 29 candidates Candidate 3 覆盖，排除）
- Dario Amodei（同上，排除）
- Demis Hassabis（May 26 "deliberate provocation"，已在 May 29 candidates Candidate 3 覆盖，排除）
- OpenAI Frontier Governance Framework（May 29，已在 May 30 candidates Candidate 2 覆盖，排除）
- Groq $650M / NVIDIA not-acqui-hire（May 28–29，已在 May 30 candidates Candidate 1 覆盖，排除）
- Anthropic $65B / $965B / $47B ARR（May 28，已在 May 29 candidates Candidate 2 覆盖，排除）
- Claude Opus 4.8 Dynamic Workflows（May 28，已在 May 29 candidates Candidate 1 覆盖，排除）
- MIT Technology Review 16% entry-level decline（May 26，已在 May 30 candidates Candidate 3 覆盖，排除）
- arXiv 2605.23972 "Why We Need World Models for AGI"（May 13，18天，超7天窗口；534分且非官方事件锚点，排除）
- OpenAI DeployCo 发布（May 11–13，20天，超7天窗口，排除）
- OpenAI 机密 S-1 申请（May 22，9天，超7天窗口；AI产品战略柱已被 C1 覆盖，排除）
- Sam Altman $2M 代币 / YC 权益互换提案（May 20，11天；无法形成独立于"Altman IPO叙事管理"的新视角，排除）
- AGIBOT World 2026 数据集开源（The Robot Report，日期未精确确认；Tier 2 信源，缺乏足够细节，排除）
- 世界智能博览会天津（May 28–30）/ BEYOND Expo 澳门（May 27–30）：PaXini 数据集、AlphaBot Cube；中国垂直活动，信息来源为 Xinhua 和 GadgetFlow，非 Tier 1；无 Zico 独特分析角度，排除
- Anthropic $200B Google Cloud 5年协议（May 5，26天，超7天窗口；近30天边界但 AI产品战略柱已饱和，排除）
- Swyx / Latent Space（最近 Substack 文章无精确 May 25–31 事件锚点，排除）
- Jim Fan "Robotics Endgame" at Sequoia AI Ascent（April 20，41天，超7天窗口，排除）
- GitHub Trending OpenClaw 302K stars（Mid-May，无精确 May 25–31 锚点，排除）
- Google Antigravity 2.0（May 19，11天；功能性产品更新无独立叙事深度，与 Genie 3 同一天但分析价值更低，排除）
- Illinois Companion Model Safety Act（May 31 立法截止日；AI regulation / mental health，与 Zico 五大主题柱契合度偏低，排除）

**Total signals found**: 31 evaluated

**Why these 3**:
- **Candidate 1（$500M enterprise Claude billing accident）**：时效最强（May 28–29，2–3 天前），Tech Startups + BusinessToday + Yahoo Finance + Windows Central 四方独立确认；AI 产品战略柱：过去3天 candidates 覆盖了 Groq/NVIDIA 授权结构（产品战略：基础设施权力）、Anthropic $65B ARR 飞轮（产品战略：企业部署速度）——今天的角度完全不重叠："企业 Agent 工作流的用量治理架构缺失"是一个独立叙事；Uber/Microsoft/无名客户三件事同一季度同时发生提供了完整的模式证据；"这是架构问题不是治理错误"是中文媒体报道中完全缺席的分析视角；与 Zico 的 Agent 经济/产品战略认知深度高度匹配；HIGH 优先级。
- **Candidate 2（KPMG + Claude 276,000 employees）**：11天前（May 20），在30天可接受窗口内；Anthropic 官方 + Fortune + ResultSense 三方确认；组织形式变革柱：过去3天 candidates 在此柱只覆盖了 MIT Tech Review 16% 就业数据（May 30），那是"量化AI就业冲击"叙事；KPMG 是完全不同的叙事——不是冲击而是实施，不是理论而是合同；"powered by Claude 出现在客户交付标识里"是第三阶段最清晰的公开案例；Zico 的组织形式变革三阶段框架在此有直接映射；HIGH 优先级。
- **Candidate 3（Genie 3 + Waymo World Model）**：11天前（May 19–20，Google I/O），在30天可接受窗口内；Techtimes + The-Decoder + Sci-Tech Today + Automotive World 四方确认；深层AI思考柱：过去3天 candidates 在此柱覆盖了 Hassabis "deliberate provocation"（叙事策略分析）和 OpenAI Governance Framework（AI 治理结构分析）——今天角度完全不同："世界模型基础设施平民化路径"是独立叙事；"训练 Waymo 机器人的同一套系统开放给 $200/月用户"是可独立验证的发现式角度；Zico 在酷家乐做 3DGS 产品，这个叙事对他来说有直接的认知对照价值；中文媒体 Google I/O 报道聚焦 Gemini 消费者功能，Genie 3 的 Waymo 物理 AI 基础设施叙事几乎未被覆盖；MEDIUM 优先级（11天稍老，深层思考柱近期已有覆盖）。
