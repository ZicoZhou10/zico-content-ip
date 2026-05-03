---
date: 2026-05-03
status: written
selected: candidate 1 → drafts/012-ceiling-hedge-xhs.md
---

# Today's Candidates

## Candidate 1: AlphaGo 之父 David Silver 拿下欧洲最大种子轮——押注"不用人类数据"的 AI 范式

- **Event**: 2026年4月27日，前 Google DeepMind 研究员、AlphaGo / AlphaZero / MuZero 联合创始人 David Silver 携 Ineffable Intelligence 从 Stealth 出发，宣布完成 $1.1B 种子轮融资，估值 $5.1B，成为欧洲有史以来最大种子轮融资纪录。投资方：Sequoia Capital + Lightspeed Venture Partners 联合领投，NVIDIA、Google、DST Global、Index Ventures、英国主权 AI 基金参投。核心主张：LLM 代表"数据时代"（Era of Data）——它们只能重组人类已经写下来的知识，无法发现真正新的东西。Ineffable 押注纯强化学习（RL），从零开始，不依赖任何人类数据，目标是构建"超级学习者"（Superlearner）——能够自主重新发现语言、数学、科学，然后超越它们。Silver 与 Richard Sutton（RL 领域奠基人）在 2025年联合发表论文《Welcome to the Era of Experience》，将这一路径命名为"经验时代"（Era of Experience）：AI 通过与世界直接交互学习，而非消化人类语料。Sequoia 的投资备忘录标题：「A Superlearner for the Era of Experience」。公司现无发布路线图和 benchmark 节点，预计最早 2026 年底出第一批模型结果。
- **Source**: https://techcrunch.com/2026/04/27/deepminds-david-silver-just-raised-1-1b-to-build-an-ai-that-learns-without-human-data/ | https://www.cnbc.com/2026/04/27/deepmind-ineffable-intelligence-record-seed-funding-nvidia-google.html | https://sequoiacap.com/article/partnering-with-ineffable-intelligence-a-superlearner-for-the-era-of-experience/ | https://tech.eu/2026/04/27/ineffable-intelligence-launches-with-record-breaking-11b-seed-round/ | https://pathfounders.com/p/ineffable-intelligence-breaks-out-of-stealth
- **Timeliness**: 6 days ago（2026年4月27日）
- **Topic pillar**: 深层思考
- **Zico's angle**: 中文媒体报道了"AlphaGo 之父拿了10亿美元"，然后就停了。没有人认真讲清楚这件事背后的宣言：Silver 和 Sutton 说，LLM 代表的整个范式有一个根本天花板——你问 GPT 一个人类从未想过的问题，它做不到，因为它没有读过关于这个问题的文章。强化学习不同：AlphaGo 没有看过任何一局人类棋谱，只靠自我对弈，打败了李世石。Ineffable 的赌注是：这个原理（从经验交互中学习，而不是从人类记录中学习）可以推广到通用智能。这件事里有一个容易被忽略的信号：NVIDIA 和 Google 同时参与了这个融资——而这两家公司也都在大力支持 LLM 路径。顶级战略投资人同时押两个看起来互相竞争的范式，只有一种解释：他们认为 LLM 路径的上限可见，RL-from-scratch 路径的上限未知。这不是"Scaling Law 已死"的结论，是"Scaling Law 之外还有另一条路"的开始。
- **Resonance hook**: David Silver 做了 AlphaGo——没有看过一局人类棋谱，只靠自我对弈，打败了世界冠军。他现在要用同一个逻辑做通用 AI，融到了欧洲史上最大种子轮。NVIDIA 和 Google 都押了。这不是在说 GPT 错了，是在说 GPT 之外，还有另一条路有人愿意下真注了。
- **Recommended priority**: high

---

## Candidate 2: Anthropic 同一天发了 9 个创意工具连接器，还出钱赞助了 Blender

- **Event**: 2026年4月28日，Anthropic 宣布「Claude for Creative Work」，同步向 9 款创意工具发布 Claude MCP 连接器：Adobe、Blender、Ableton、SketchUp（Trimble）、Autodesk Fusion 360、Resolume、Affinity（Canva）、Splice。同日，Blender 基金会宣布 Anthropic 加入 Blender 开发基金（Blender Development Fund）成为企业赞助人（Corporate Patron），承诺每年出资 €240,000（约 175 万人民币），专门用于 Blender 核心开发，重点是 Python API 层。Blender Lab 同步上线了 MCP 服务器，允许 Claude 通过自然语言直接操控 Blender 场景：调试3D场景、批量修改对象属性、调用 Blender Python API。SketchUp 连接器的具体行为：用户用自然语言描述房间/家具/建筑概念 → 生成可编辑起点 → 在 SketchUp 中直接打开精修，完成 Text→3D 工作流闭环。Blender 当前企业赞助人名单：NVIDIA、AMD、Epic Games、Unity Technologies、Meta、Apple——Anthropic 是第一家加入 Blender 开发基金的前沿 AI 实验室。Blender CEO Ton Roosendaal 在回应时特别强调"This is not an AI takeover"——需要专门解释这句话，反映社区敏感度。
- **Source**: https://9to5mac.com/2026/04/28/anthropic-releases-9-new-claude-connectors-for-creative-tools-including-blender-and-adobe/ | https://www.blendernation.com/2026/04/29/anthropic-adds-blender-support-joins-the-blender-development-fund-as-corporate-patron/ | https://www.cgchannel.com/2026/04/ai-developer-anthropic-becomes-blenders-latest-corporate-patron/ | https://digitalproduction.com/2026/04/30/anthropic-funds-blender-ships-claude-connector/ | https://80.lv/articles/blender-ceo-on-anthropic-funding-this-is-not-ai-takeover
- **Timeliness**: 5 days ago（2026年4月28日）
- **Topic pillar**: AI 协作实践（与空间智能前沿交叉）
- **Zico's angle**: 我在做 AI+3D 产品（3DGS 方向），对这件事的解读角度和一般科技媒体不同。Blender 的赞助商名单是一个信号密度极高的列表：NVIDIA（想让 3D 跑在 GPU 上）、Epic Games（想用 3D 作为游戏引擎入口）、Meta（想用 3D 构建元宇宙基础层）——现在加上 Anthropic（想用自然语言控制 3D 工具）。这些公司赞助 Blender 的理由各不相同，但方向一致：3D 工具是下一代创意生产流程的核心节点。Anthropic 的 SketchUp 连接器做的事——"用文字描述空间概念，直接生成可编辑的 3D 起点"——和我在产品里思考的路径是同一个问题的不同切入点。中文 AI 媒体报道这件事的框架是"Claude 支持更多工具了"，完全忽略了"前沿 AI 实验室开始投资 3D 工具底层基础设施"这一层信号。Blender CEO 需要专门出来说"这不是 AI 接管"，说明社区已经感受到了范式转移的压力。AI 进入 3D 工具，不是功能迭代，是工作流重构的起点。
- **Resonance hook**: Anthropic 在同一天做了两件事：给 Blender 装上了 Claude 连接器，然后出了真金白银每年 €24 万资助 Blender 开发。Blender CEO 需要出来说"这不是 AI 接管"。Anthropic 为什么要赌 3D 工具的基础设施？
- **Recommended priority**: high

---

## Candidate 3: 代码漏洞发现到可用攻击代码：2023年5个月，2026年10小时——Anthropic 的 Claude Security 就是这个数字逼出来的

- **Event**: 2026年4月30日，Anthropic 宣布 Claude Security 从受邀内测转为公测（public beta），向所有 Claude Enterprise 客户开放。Claude Security 由 Claude Opus 4.7 提供支持，核心功能：自动扫描代码库漏洞 + 生成修复补丁，支持定时扫描和定向扫描，集成企业审计系统。企业安全生态整合：CrowdStrike、Palo Alto Networks、SentinelOne、Trend.ai、Wiz 均已接入或正在整合 Opus 4.7 作为核心引擎。背景数据（来源 Security Affairs / Anthropic）：从安全漏洞被发现到攻击者写出可用的漏洞利用代码（working exploit），平均时间：2023年约 5 个月；2026年约 10 小时。同期并行消息：Anthropic Project Glasswing（Claude Mythos 安全应用版）已向 Apple、Microsoft、Google、Amazon 开放，用于在攻击者利用前发现并修复零日漏洞。Anthropic 同时推出 Cyber Verification Program：允许经认证的安全研究人员/渗透测试人员绕过 Opus 4.7 的高风险网络安全请求拦截。
- **Source**: https://siliconangle.com/2026/04/30/anthropic-announces-claude-security-public-beta-find-fix-software-vulnerabilities/ | https://www.infosecurity-magazine.com/news/anthropic-claude-security-for-ai/ | https://thenewstack.io/anthropics-claude-security-beta/ | https://securityaffairs.com/191532/ai/anthropic-launches-claude-security-to-counter-rapid-ai-powered-exploits/ | https://www.business-standard.com/technology/tech-news/anthropic-announces-claude-security-beta-for-enterprise-customers-126050100019_1.html
- **Timeliness**: 3 days ago（2026年4月30日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 中文媒体的报道是"Anthropic 推出安全扫描工具"，然后结束。没有人把这件事和那个数字放在一起讲：漏洞从发现到被利用，2023年要等5个月，2026年只需要10小时——这是 Claude Security 诞生的真实背景，不是"AI 功能扩展"。这件事的深层逻辑：攻击方已经在大规模使用 AI（AI 生成漏洞利用代码的速度 ≈ 人类的 360 倍），传统安全工具的扫描频率和修复速度跟不上。CrowdStrike 和 Palo Alto Networks 选择整合 Opus 4.7，不是因为"Claude 会写代码"，是因为 AI 攻击速度倒逼了 AI 防守速度必须同步提升——这是一个军备竞赛，而不是功能升级。更深一层的产品战略读法：Anthropic 正在以一种非常精准的方式切入企业预算——不是"更多人付订阅费"，是"进入企业安全这个年合同单价 $50万-$500万、几乎没有砍预算风险的预算池"。一旦 Opus 4.7 成为 CrowdStrike 的核心引擎，这是比 API 调用费更稳定的收入结构。中文 AI 讨论通常停留在"模型哪家强"——这件事是关于 AI 如何建立不可替代的企业基础设施地位。
- **Resonance hook**: 从发现漏洞到有人写出可以实际利用的攻击代码，2023年需要5个月，现在只需要10小时。Anthropic 的 Claude Security 不是在追"AI+安全"风口——它是在解一个数字倒逼出来的产品命题。CrowdStrike 和 Palo Alto Networks 都接入了。
- **Recommended priority**: medium（时效最新3天，但本周 Anthropic 相关候选已出现两次，建议 Zico 权衡；独立角度充分，信息差高）

---

## Scan summary

**Sources scanned**:
- X/Twitter: Karpathy（slopacolypse 话题 Jan 26，超出窗口；Claude Code 使用经验综述 Jan 27，超出窗口）、Altman（近期无7天内强新锚点）、Dario Amodei（Claude Security 官方博客；Blender 资助同日）、Jim Fan（Genie 3 分析文章，1月底发布超窗口）、LeCun / Demis Hassabis（近7天无新锚点，前期候选已覆盖）、Swyx（无7天内具体锚点）、Nat Friedman（无7天内具体锚点）
- GitHub Trending: Craft Agents OSS by Lukilabs（May 2，Apache 2.0，desktop agent + Craft document tools，评估后信息增量有限，排除）；caramaschiHG/awesome-ai-agents-2026（持续更新，无单点事件）；GenericAgent（self-evolving，3.3K lines，系统级控制，有趣但无具体时效锚点）
- Hacker News: 4月29日-5月3日前页（Anthropic Claude Security 讨论；David Silver/Ineffable 讨论；"AI speed of attack" 线程）
- Anthropic 官方博客: Claude for Creative Work（4月28日）；Claude Security public beta（4月30日）；Claude Opus 4.7（4月16日，17天前，超7天窗口）
- OpenAI 官方博客 / CNBC: GPT-5.5（4月23日，10天前，超窗口；中文覆盖率高）
- Google DeepMind: Genie 3（1月底发布，超窗口）；Gemini 3.1（2-3月发布，超窗口）
- TechCrunch / CNBC / Sequoia Blog / Tech.eu: David Silver / Ineffable Intelligence（4月27日）
- arXiv cs.AI / cs.CV: HY-World 2.0（3DGS multi-modal world model，2604.14268）；"Do LLMs Build Spatial World Models?"（2604.10690，4月）；MetaEarth3D（2604.22828，4月19日，已用于4月25日 candidates 背景参考）；Agentic Reasoning survey（2601.12538，1月，超窗口）
- Blender Foundation / BlenderNation / CG Channel: Anthropic joins Blender Development Fund（4月28日-29日报道）
- Salesforce Newsroom / VentureBeat / SalesforceDevops.net: Headless 360（TDX 2026，4月15日，18天前——评估后认为时效性不足，但作为"agent economy"信号被记录）
- China AI: DeepSeek V4（4月24日，9天前，中文媒体覆盖率极高，信息差为零，排除）；Tencent/Alibaba 投资 DeepSeek（4月22日，中文媒体主战场，排除）；Huawei Ascend 950 订单（4月29日，同样中文信息差极低，排除）

**Total signals found**: 22 evaluated

**Why these 3**:
1. **David Silver / Ineffable Intelligence**（Candidate 1）：时效6天，7天窗口内；欧洲历史最大种子轮 + AlphaGo 创始人背书使锚点极强；中文媒体报了融资金额，100% 没有拆解 "Era of Experience" 论文的核心主张（LLMs 有认知天花板）；NVIDIA + Google 双押信号；深层思考柱近期候选（4月30日 Candidate 3=Agentic World Modeling，5月2日 Candidate 3=GR00T N1.7）均不同方向，无重叠
2. **Claude for Creative Work + Blender 资助**（Candidate 2）：时效5天；双重事件锚点（9个连接器发布 + 资助 Blender 成为 Corporate Patron）；Zico 的 3DGS 一线经验提供不可复制的真实性和产品直觉；中文媒体框架="AI工具集成"，完全未关注"前沿 AI 实验室首次为 3D 工具底层基础设施买单"这一层；AI 协作实践柱近期（4月30日 Candidate 2=Karpathy CLAUDE.md）不同方向，无重叠
3. **Anthropic Claude Security**（Candidate 3）：时效最强（3天）；"5个月→10小时"这个数字的冲击力极高；CrowdStrike / Palo Alto 整合 = 生态级信号；AI 产品战略柱近期（5月2日 Candidate 1=Anthropic ARPU）已用，主题完全不同（ARPU=商业模式，Security=产品品类扩张）；唯一风险是 Anthropic 本周出现频率高，降为 medium 优先级

**Excluded signals**:
- GPT-5.5（4月23日）：10天超窗口，中文媒体覆盖率极高
- DeepSeek V4 + Huawei/中国 AI 动态：中文媒体主战场，信息差为零
- Craft Agents OSS（5月2日）：GitHub trending 项目，但产品信息增量低、没有战略级洞察点
- Salesforce Headless 360（4月15日）：Agent Economy 好故事，但18天前超理想窗口；且昨日 Candidate 2（YC RFS）已覆盖"agents replacing SaaS"叙事框架，直接跟进会有概念重叠
- Claude Opus 4.7（4月16日）：17天前，且 Claude Security 角度已隐含 Opus 4.7 的能力叙事
- Genie 3（1月底）：超窗口
- arXiv 2604.10690 "Do LLMs Build Spatial World Models?"：Candidate 1 （Silver 的 LLM 认知局限论点）已覆盖同一方向，不重复
