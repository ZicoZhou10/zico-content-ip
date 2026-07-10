---
date: 2026-07-10
status: written
selected: candidate 2 → drafts/071-cowork-delegation-xhs.md
---

# Today's Candidates

## Candidate 1: SpaceXAI + Cursor 联合发布 Grok 4.5——$60B 收购后第一个联合训练模型，Opus 级能力、$2/$6 定价，比 Anthropic Opus 4.8 便宜 60–76%（July 8）

- **Event**: 2026年7月8日，**SpaceXAI**（Elon Musk 旗下 AI 部门）和 **Cursor** 联合发布 **Grok 4.5**，这是 SpaceX 以 **$60B** 完成收购 Cursor 后推出的第一个联合训练模型。模型规格：**1.5 万亿参数**，Opus 级别能力（接近 Anthropic Opus 4.8 和 OpenAI GPT-5.5），在 Colossus 计算集群上完成训练，生产测试在 SpaceX 和 Tesla 内部进行。定价：**$2/M input、$6/M output**，比 Anthropic Opus 4.8 便宜约 **60%（input）和 76%（output）**。发布即上线：在 Cursor 全部订阅方案中作为可用模型，同时开放 Grok Build 和 SpaceXAI console API。一个关键细节：Grok 4.5 **训练数据包含 Cursor 的真实编程交互数据**（Cursor 拥有数百万活跃开发者用户），这是任何纯 API 模型无法复制的数据飞轮。**EU 暂不可用**（监管合规原因）。Bloomberg（7月8日）、Axios（《Scoop: Musk's SpaceXAI releases new model, Grok 4.5》）、VentureBeat（《SpaceX's Grok 4.5 launches at half the price of rivals — here's why that could rattle Anthropic and OpenAI》）均有深度报道。
- **Source**: https://www.bloomberg.com/news/articles/2026-07-08/spacexai-cursor-unveil-grok-ai-model-for-legal-finance-tasks | https://www.axios.com/2026/07/08/spacexai-grok-new-model | https://cursor.com/blog/grok-4-5 | https://x.ai/news/grok-4-5 | https://venturebeat.com/technology/spacexs-grok-4-5-launches-at-half-the-price-of-rivals-heres-why-that-could-rattle-anthropic-and-openai
- **Timeliness**: 2 天前（2026年7月8日发布）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 这件事真正值得分析的，不是"又来了一个便宜的 Opus 级模型"，而是 SpaceX 用 $60B 买的是什么。

  Cursor 的月活用户是数百万开发者。这些用户每天在 Cursor 里写代码、接受补全、修改建议、回退 diff。每一个这样的交互都是真实的人类偏好数据——哪种补全被接受、哪种被拒绝、哪种情况下用户会立刻修改 AI 的输出。这些数据 Anthropic 没有、OpenAI 没有、任何纯 API 模型公司都没有。

  $60B 买的不是 Cursor 的订阅收入，是这个数据飞轮，以及飞轮绑定的数百万开发者用户。Grok 4.5 是这个并购逻辑的直接产物：用 Cursor 数据训练，嵌回 Cursor 作为默认模型，用户在不换工具的情况下就绑定了 SpaceXAI 的模型。

  竞争维度也由此改变。过去 AI 的竞争是"谁的模型能力更强"，现在是"谁能把最强模型植入用户最高频的工作场景并控制数据回路"。Grok 4.5 的定价（比 Opus 4.8 便宜 60-76%）只是吸引流量的入场价，真正的护城河是：训练数据来自真实用户 × 模型内嵌进工具 × 用户换工具的迁移成本。这是 AI 时代的垂直整合，逻辑和 Google 买 Waze 获取地图数据、Meta 买 Instagram 获取社交图谱，是同一件事。

- **Resonance hook**: 昨天（7月8日），SpaceXAI 和 Cursor 联合发布 Grok 4.5。Opus 级，$2/$6 per million tokens——比 Anthropic Opus 4.8 便宜 60-76%。立刻上线 Cursor 全平台。训练数据来自 Cursor 数百万用户的真实编程交互。SpaceX 花 $60B 收购 Cursor。这个价格买的不是 SaaS 订阅收入——是 Cursor 用户每天产生的真实偏好数据，和绑定在这个工具上的数百万开发者。AI 时代第一个"模型+分发+数据飞轮"垂直整合案例已经落地。
- **Recommended priority**: high

---

## Candidate 2: Anthropic 发布 Claude Cowork 使用数据：90%+ 会话与写代码无关，#1 用例是"业务流程与运营"（33.4%）（July 7）

- **Event**: 2026年7月7日，**Anthropic** 宣布 **Claude Cowork** 正式扩展至 web、iOS 和 Android（此前仅 desktop），Max 用户开始分批获得 beta 访问。在这次发布中，Anthropic 同步披露了 Cowork 的真实使用数据：**90%+ 的会话与软件开发无关**。具体分布：**业务流程与运营**占 **33.4%**（最大单一类别），**内容创作与文案**占 **16.4%**，**软件开发**仅占 **8.7%**。新功能：会话跨设备同步、后台异步任务执行（用户不在线时 Claude 继续执行）、Claude 遇到需要判断的节点时主动向用户手机推送决策请求。同周背景：两周前，Anthropic 还发布了 **Claude Tag**——一个原生运行在 **Slack** 里的团队协作 AI Agent，定位是多人协同任务。VentureBeat 标题直接说明了含义：《Anthropic brings Claude Cowork to mobile and web as usage data shows most users aren't coding》。TechCrunch 的报道角度是：《The coding agent wars are spilling into the rest of the office》。
- **Source**: https://venturebeat.com/technology/anthropic-brings-claude-cowork-to-mobile-and-web-as-usage-data-shows-most-users-arent-coding | https://techcrunch.com/2026/07/07/the-coding-agent-wars-are-spilling-into-the-rest-of-the-office-claude-cowork/ | https://9to5mac.com/2026/07/07/anthropic-expanding-claude-cowork-to-mobile-and-web-details-here/
- **Timeliness**: 3 天前（2026年7月7日，Anthropic 官方发布）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 8.7% 这个数字，把过去两年"AI Agent = 开发者工具"的叙事结构性地推翻了。

  Claude Cowork 是作为 Claude Code 的平行产品发布的——它在产品定义上靠近开发者生态，在发布节奏上跟着 AI coding agent 的竞争周期走。但用户完全不顾产品定位，把它做成了通用知识工作委托层：业务运营（33.4%）+ 内容创作（16.4%）= 超过一半的 Cowork 使用量，和软件没有关系。

  这不是意外，是用户在告诉产品方：他们想要的不是"AI 帮我写代码"，是"AI 帮我处理工作里的高频、低复杂度、但很耗时的任务"。这两件事对大多数知识工作者来说，从来不是写代码，是撰写、整理、分析、跟进、执行。

  把 8.7% 和另外一件事放在一起看：同期 Anthropic 在 Slack 里发布了 Claude Tag。Cowork 是个人任务委托，Claude Tag 是团队级协作层。两件事同步推进的组织含义是：Anthropic 正在把 AI Agent 从"开发者生产力工具"迁移到"组织基础设施"——个人有 Cowork 委托，团队有 Tag 协作，下一步会是什么？

  对 Zico 而言，这个数据是"人类退出生产环节"这个框架的直接例证——不是写代码这个专业场景，是全部知识工作场景。8.7% 的代码会话比例意味着：AI 代理的扩散路径，正在从"开发者 → 其他人"演进，而且速度比大多数组织的 AI 采用计划要快。

- **Resonance hook**: 7月7日，Anthropic 发布了一个数字：**Claude Cowork 90%+ 的会话与软件开发无关**。8.7% 是代码。33.4% 是业务流程运营。这个工具以 AI coding agent 的面貌发布，用户把它做成了通用知识工作代理。同一周，Anthropic 在 Slack 里上线了 Claude Tag，做团队级协作。"AI Agent = 开发者工具"的时代，数据显示已经结束了。
- **Recommended priority**: high

---

## Candidate 3: Mistral 发布 Robostral Navigate——8B 模型，单 RGB 摄像头，零真实世界训练数据，机器人导航 76.6% 成功率（July 8）

- **Event**: 2026年7月8日，**Mistral AI** 发布 **Robostral Navigate**，这是 Mistral 的首个机器人学模型，也是 physical AI 领域的首次进军。核心规格：**8B 参数**视觉语言模型，输入仅需**单普通 RGB 摄像头**（无 LiDAR、无深度摄像头、无多摄像头阵列），接受自然语言指令如"走出大厅，穿过走廊，进入储藏室，面对第二层货架停止"，输出指向坐标或位移命令。训练数据：**完全在仿真环境中**完成（**40 万条轨迹，6,000 个场景**），零真实世界机器人训练数据，随后通过在线强化学习微调。性能：在 **R2R-CE（Room-to-Room Continuous Environments）验证集（unseen）** 上成功率 **76.6%**，跨平台泛化：**轮式机器人、足式机器人、飞行器**均可使用同一模型。当前开放给制造业、物流、配送、酒店行业的合作伙伴测试。Bloomberg（7月8日）：《Mistral AI Releases Robotics Model to Support Physical AI Push》。
- **Source**: https://mistral.ai/news/robostral-navigate/ | https://www.bloomberg.com/news/articles/2026-07-08/mistral-ai-releases-robotics-model-to-support-physical-ai-push | https://www.verdict.co.uk/mistral-unveils-robostral-navigate/ | https://theaiinsider.tech/2026/07/08/mistral-ai-introduces-robot-navigation-model/ | https://quasa.io/media/mistral-robostral-navigate-single-camera-8b-model-transforms-robot-autonomy
- **Timeliness**: 2 天前（2026年7月8日，Mistral 官方发布）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: 这件事有两个层次值得分开说。

  第一层是硬件约束的消解。LiDAR——自动驾驶和机器人导航的"标配"传感器——工业级单元成本在 $10,000–$75,000 之间。Robostral Navigate 的主张是：一个 8B 模型加上一颗普通 RGB 摄像头（成本 <$50）可以在 unseen 环境中达到 76.6% 的导航成功率。如果这个数字在真实部署中站得住，机器人导航的硬件门槛从"昂贵传感器堆叠"降到了"一颗摄像头+边缘推理芯片"——这是实体 AI 部署成本的结构性坍塌。

  第二层是仿真训练的能力边界。40 万条轨迹、6,000 个场景，全部在仿真环境生成，模型在发布前从未接触过真实物理环境。Sim-to-real transfer（仿真到真实的迁移）一直是 embodied AI 的最大技术壁垒——仿真里学到的技能在真实世界往往失效。Robostral Navigate 的数字表明这个壁垒在特定任务（室内导航）上已经可以用大规模仿真数据绕过。这和 3DGS 技术的趋势方向一致：更好的环境表征 → 更高质量的仿真数据 → 更少的真实世界训练成本。

  Mistral 的战略信号不容忽视：一家欧洲纯语言模型公司把第一个非语言产品做成了机器人导航模型。physical AI 的前沿已经足够近，连 LLM 原生公司都开始跨界了。

- **Resonance hook**: 7月8日，Mistral 发布 Robostral Navigate。8B，单 RGB 摄像头——不需要 LiDAR（$10K-$75K 的工业级传感器），不需要深度摄像头，不需要多摄阵列。训练：完全在仿真中（40 万条轨迹，6,000 个场景）——零真实世界机器人训练数据。上线即泛化：轮式、足式、飞行器同一模型，unseen 环境 76.6% 成功率。硬件门槛是传感器成本，一直是 physical AI 大规模部署最大的障碍之一。Robostral 的主张：障碍在模型，不在传感器。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**:
  - Bloomberg（2026年7月8日，Grok 4.5 发布、Mistral Robostral 发布）
  - Axios（2026年7月8日，《Scoop: Musk's SpaceXAI releases new model, Grok 4.5》）
  - VentureBeat（2026年7月7-8日，Claude Cowork 使用数据、Grok 4.5 分析）
  - TechCrunch（2026年7月7日，Claude Cowork 扩展报道）
  - Cursor 官方博客（2026年7月8日，Grok 4.5 发布声明）
  - Mistral 官方博客（2026年7月8日，Robostral Navigate 发布）
  - 9to5Mac、DigitalToday、MetaversePost（Claude Cowork 跟进报道）
  - Verdict.co.uk、TheAIInsider（Robostral Navigate 技术细节）
  - HN Frontpage（2026年7月8日，Robostral Navigate 出现在 HN 首页）
  - AI Weekly、MLQ.ai、ExplainX.ai（Grok 4.5 分析）

- **Total signals found**: 15+
- **Why these 3**:
  - Candidate 1（Grok 4.5）：最新（2天前），信息量最大的战略事件——$60B 并购 + 垂直整合逻辑，中文圈会报发布但不会分析数据飞轮和竞争护城河转移。AI产品战略柱最强素材。
  - Candidate 2（Cowork 使用数据）：独家数据（8.7% 代码会话）直接颠覆"AI Agent = 开发者工具"叙事，信息差极大。与 Zico 的组织形式变革框架精准对应，是"人类退出生产环节"从理论到数据的例证。
  - Candidate 3（Robostral Navigate）：Zico 的 3DGS/physical AI 一线背景在这里有最强共鸣，单 RGB 摄像头+纯仿真训练的技术选择值得深入拆解。欧洲 LLM 公司进军 physical AI 的战略信号本身也值得一说。
  - 三者覆盖三个不同主题柱（AI产品战略、组织形式变革、深层AI思考），时效性均在 3 天内，与过去 3 天候选无重叠。
