---
date: 2026-06-29
status: pending_selection
---

# Today's Candidates

## Candidate 1: Z.AI（智谱）GLM-5.2 以 MIT License 开放全量权重，Fable 5 被封锁次日发布，1/6 成本超 GPT-5.5 编程基准——Z.ai 预告年底前开放 Fable 级别模型（June 13/16/26）

- **Event**: 2026年6月13日，北京智谱 AI（现品牌名 Z.ai）将旗舰模型 **GLM-5.2** 向付费编程用户开放；6月16日正式发布 MIT license 全量权重（744B 总参数、40B 激活参数的 MoE 架构，上下文窗口 100 万 token）。基准表现：**SWE-bench Pro 62.1%**（GPT-5.5 为 58.6%）；FrontierSWE（Dominance）**74.4%**（GPT-5.5 72.6%）；Design Arena **#1**；Agent Arena **开源模型第一**。API 定价约 $0.95-2/M input token——对比 Anthropic/OpenAI 前沿模型的 $5-15/M，约为后者的 **1/6**。关键时机：**Z.AI 于 6月13日发布，恰好是美国政府强制 Anthropic 将 Fable 5 下线的次日（6月12日）**。MIT License，无地区限制，无使用限制。**Z.ai 创始人向外界公开表示："open-weight Fable 级别能力将在2026年Q1之前到来"**（原话："open-weight Fable capabilities will be here sooner than Q1 2027"）。Latent Space/Swyx（6月16日，AINews 标题《GLM-5.2 is the real deal; Z.ai forecasts Open Fable by EOY》）；Interconnects.ai（《GLM-5.2 is the step change for open agents》）；VentureBeat（《Z.ai's open-weights GLM-5.2 beats GPT-5.5 on multiple long-horizon coding benchmarks for 1/6th the cost》）；**CNBC**（6月26日，《China's Zhipu is closing in on top U.S. AI models with Anthropic and OpenAI held back》）；South China Morning Post（6月26日，《China's Zhipu AI sparks new 'DeepSeek moment' with cost-effective coding model》）；explainx.ai（《GLM-5.2 Beats Fable 5 Reasoning — China AI Response to Export Ban 2026》）；Matt Velloso（前 Meta VP + Google DeepMind，X 发帖）："first open model that passes the bar as a daily driver"。
- **Source**: https://www.cnbc.com/2026/06/26/china-zhipu-z-ai-open-source-anthropic-openai.html | https://venturebeat.com/technology/z-ais-open-weights-glm-5-2-beats-gpt-5-5-on-multiple-long-horizon-coding-benchmarks-for-1-6th-the-cost | https://www.latent.space/p/ainews-glm-gpt-glm-52-passes-vibe | https://www.interconnects.ai/p/glm-52-is-the-step-change-for-open | https://www.scmp.com/tech/big-tech/article/3358434/chinas-zhipu-ai-sparks-new-deepseek-moment-cost-effective-coding-model | https://explainx.ai/blog/glm-5-2-zhipu-china-ai-response-fable-5-ban-2026
- **Timeliness**: 3 天前（CNBC + SCMP 6月26日主流报道）；MIT 权重发布 13 天前（6月16日）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 这件事最值得分析的不是"中国模型追上了"，而是**一个监管反馈回路正在生效，且方向和大多数人预期的相反**。

  时间线：6月12日，美国政府强制 Anthropic 在 90 分钟内关停 Fable 5 和 Mythos 5——全球最强的 AI 模型从市场上消失。6月13日，Z.AI 发布 GLM-5.2，MIT license，无地区限制，全球可用。这不是巧合，这是**AI 能力真空的市场填补**。

  GPT-5.6 Sol 现在也是政府逐客户白名单审批，只有约 20 个机构能用。Mythos 5 回来了，但仅限 100 家美国受信机构。Fable 5 至今仍封锁。与此同时，GLM-5.2 在全球任何人的服务器上都可以运行，没有申请流程，没有审批名单，没有地区限制。

  Z.AI 的价格是 Anthropic/OpenAI 的约 1/6。SWE-bench Pro 上 GLM-5.2 已经超过了 GPT-5.5（62.1% vs 58.6%）。Matt Velloso（前 Meta VP 和 Google DeepMind）是第一个说"这是我第一个可以日常使用的开源模型"的权威声音。Swyx 的标题直接：GLM-5.2 is the real deal。

  Z.ai 创始人说，"开源 Fable 级能力，年底前到来"。翻译成产品语言：**在美国政府把最前沿模型锁进审批名单的同时，中国的开源模型正在对准同一个能力目标——而且不需要任何审批就能全球部署**。

  这对做 AI 产品的人有一个直接含义：如果你今天做的产品建立在"只有美国顶级闭源模型才能做到这件事"的假设上，这个假设的保质期正在缩短。GLM-5.2 的出现不是威胁，是一个倒计时信号：**未来 6-12 个月，开源模型的能力上限将决定哪些产品需求不再是差异化护城河**。

- **Resonance hook**: 6月12日，美国政府关停 Fable 5。6月13日，Z.AI 发布 GLM-5.2——MIT License，无地区限制，1/6 成本超 GPT-5.5 编程基准。现在，Fable 5 还在封锁，GPT-5.6 需要政府白名单审批，GLM-5.2 全球任何人都能下载。Z.ai 说：开源 Fable 级能力，年底前到来。这是第二次 DeepSeek 时刻，但背景比第一次更清醒。
- **Recommended priority**: high

---

## Candidate 2: CNBC 披露 Uber 用 4 个月烧完全年 AI 预算，95% 工程师用 Claude Code，70% 代码来自 AI——但找不到和"更有用的消费者功能"之间的直接关联（June 26）

- **Event**: 2026年6月26日，CNBC 发布报道《OpenAI and Anthropic face new AI reality as users shift from 'tokenmaxxing' to efficiency》，整合了一系列企业端 AI 使用数据，核心披露：① **Uber** 总裁兼 COO **Andrew Macdonald** 在 Rapid Response 播客上透露：Uber 在 **2026年前四个月内烧完了全年 AI 预算**，且 "the company doesn't see a direct correlation between token consumption and more useful consumer features"——尽管 **95% 的 Uber 工程师每月使用 Claude Code**，**70% 的代码提交来自 AI**，Uber 仍无法画出 token 消耗和消费者产品价值之间的连线；② **Amazon** 关停了内部 AI 使用排行榜（leaderboard）；③ **Microsoft** 撤销了内部员工的 Claude Code 许可；④ AI 初创公司 **Lindy** 的 CEO 将公司 100% 的流量从 Anthropic Claude 切换到 **DeepSeek**，理由是成本差距；⑤ **AT&T 和 Meta** 同期收紧 AI 支出。报道定义"tokenmaxxing"为：**企业激励开发者尽可能多地使用 AI 而不关注结果的时代**，现在这个时代正在结束。企业正在从"用最强的 AI"转向"用能证明 ROI 的 AI"，新的核心指标是 **"intelligence per dollar"**（每美元智能量）而非"最大智能"。来源：CNBC（6月26日）、TechCrunch（6月5日，《The token bill comes due: Inside the industry scramble to manage AI's runaway costs》）、Cybernews（《Uber spends entire 2026 AI budget in 4 months, sees no ROI》）、MyGreatLearning（《Tokenmaxxing Explained: The Hidden Cost of Workplace AI》）。
- **Source**: https://www.cnbc.com/2026/06/26/openai-anthropic-new-ai-spending-reality-as-users-shift-to-efficiency.html | https://techcrunch.com/2026/06/05/the-token-bill-comes-due-inside-the-industry-scramble-to-manage-ais-runaway-costs/ | https://cybernews.com/ai-news/uber-ai-return-of-investment-token-usage/
- **Timeliness**: 3 天前（2026年6月26日，CNBC）
- **Topic pillar**: AI协作实践
- **Zico's angle**: 70% 的代码提交来自 AI，但找不到和用户功能价值的关联——这是企业 AI 使用里一个结构性问题，不是工具问题。

  Uber 的处境值得仔细拆解。95% 工程师用 Claude Code，这是极高的渗透率。70% 代码提交来自 AI，这是极高的参与度。但 COO 站在播客里说"找不到 token 消耗和消费者功能改善之间的直接关联"——这不是在说 Claude Code 不好用。这是在说：**企业没有建立评估 AI 工作产出价值的能力**。

  token 消耗 ≠ 价值创造，这个等式在"tokenmaxxing"时代从来没有人去验证，因为没有人要求验证。Uber 的 AI 预算在 4 个月内耗尽，触发了这个验证时刻。结果是：测量 AI 贡献的机制根本不存在。

  这个问题比"哪个模型更好"深得多。它指向的是：**当 AI 工作产出大规模进入产品流程时，如何定义 AI 工作的"完成"？谁来 review 70% 由 AI 提交的代码？review 质量由谁保证？验证 AI 输出的能力，是否和使用 AI 的速度同步增长？**

  Amazon 关掉了 AI 使用排行榜——一个鼓励最大化 token 消耗的内部激励机制。Microsoft 撤销了内部 Claude Code 许可。这两个动作说明的不是 AI 没有价值，而是**当"用多少 AI"变成一个可以比较的指标时，它就变成了目标本身，而不是服务于真实目标的工具**。这是 Goodhart 定律在企业 AI 使用中的精确表现。

  对 AI 协作实践的直接含义：如果你今天的 AI 工作流里，评估的是"我用了多少 AI"而不是"AI 帮我交付了什么"，你的组织正在重复 Uber 的问题。tokenmaxxing 时代结束之后，真正的工作才开始：建立 AI 工作的输出评估标准，从 token 消耗 → 到结果追踪。这是 2026年下半年最重要的 AI 落地议题之一。

- **Resonance hook**: 2026年前四个月，Uber 烧完了全年 AI 预算。95% 工程师用 Claude Code，70% 代码提交来自 AI。然后 Uber COO 在播客里说：我们找不到 token 消耗和更有用的消费者功能之间的直接关联。tokenmaxxing 时代结束了。下一个时代的问题不是"用多少 AI"，是"AI 输出怎么被验证，怎么和产品价值挂钩"。这个能力，现在几乎没有企业有。
- **Recommended priority**: high

---

## Candidate 3: NVIDIA Cosmos 3 技术报告（June 22）：$60 亿 Q1 投资涌入具身 AI 世界模型，但 NVIDIA 自己说"WAMs 和 VLAs 之间还没有赢家"（June 18-22）

- **Event**: 2026年6月1日，NVIDIA 在 COMPUTEX 2026 上正式发布 **Cosmos 3**——"Open Frontier Foundation Model for Physical AI"，核心架构：mixture-of-transformers（视觉推理 + 世界生成 + 动作预测三合一），训练数据：**20 万亿 token 的多模态数据**（近 10 亿张图像 + 4 亿个真实和合成视频 + 环境音频 + 人类和机器人动作数据）。6月22日，NVIDIA Research 发布完整技术报告《Cosmos 3: Omnimodal World Models for Physical AI》，引入了"simulator-grounded embodied spatial reasoning"——在可执行物理模拟器状态中标注空间推理。关键背景数据：① **2026年 Q1，具身 AI 世界模型领域单季度吸引了 $60 亿投资**；② 中国初创公司 **Omega-EVA** 于6月17日成为该领域最新进入者；③ 面对两种主流技术路径的竞争，NVIDIA **在自己的 June 2026 技术博客中明确写道："there is currently no real winner between WAMs and VLAs"**（世界动作模型 vs. 视觉-语言-动作模型之间，目前没有赢家）；④ arXiv 论文 2506.22355《Embodied AI Agents: Modeling the World》（Pascale Fung 等 20 位作者，2026年6月），正式提出世界模型是具身 AI 推理和规划的核心，不只是感知工具；⑤ TechTimes（6月18日）：《Embodied AI World Models Attracted $6 Billion, But the LLM Parallel May Not Hold》。来源：NVIDIA investor relations（6月1日）、GlobeNewswire（6月1日）、Axios（6月1日，《Nvidia's Cosmos 3 open AI world model helps robots, autonomous vehicles》）、NVIDIA Research 技术报告（6月22日）、TechTimes（6月18日）。
- **Source**: https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Launches-Cosmos-3-the-Open-Frontier-Foundation-Model-for-Physical-AI/default.aspx | https://research.nvidia.com/labs/cosmos-lab/cosmos3/technical-report.pdf | https://www.axios.com/2026/06/01/nvidia-ai-push-cosmos-3-world-model | https://www.techtimes.com/articles/318671/20260618/embodied-ai-world-models-attracted-6-billion-llm-parallel-may-not-hold.htm | https://arxiv.org/abs/2506.22355
- **Timeliness**: 7 天前（NVIDIA Research 技术报告 6月22日）；11 天前（TechTimes 6月18日）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: NVIDIA 自己说"WAMs 和 VLAs 之间没有赢家"——这是具身 AI 领域里最重要的一个承认，因为这个结论来自在这场比赛里下注最重的公司。

  先厘清两个技术路径的差异。WAMs（World Action Models / 世界动作模型）：先学物理世界的预测模型，再把动作嵌入其中——模型会理解"推一个物体会发生什么"，再规划下一步。VLAs（Vision-Language-Action / 视觉-语言-动作模型）：直接从视觉感知到语言理解再到动作输出，没有显式的世界物理模型——类似 ChatGPT 但加了"手"。两种路径都有强支持者：DeepMind Gemini Robotics 更偏 VLA，NVIDIA Cosmos 更偏世界模型方向。

  $60 亿进了 Q1 的具身 AI 世界模型赛道。但 NVIDIA 说："没有赢家"。这和 LLM 时代的一个关键对比值得认真考虑。GPT-3 出来的时候，Transformer 架构已经是公认的赢家——研究者在追缩放（scaling），不在辩架构。具身 AI 的技术路径辩论，在 $60 亿资本涌入之后仍然是开放的。这意味着：**这笔钱里，有一半以上可能押注在了最终不会成为主流的架构上**。

  从 Zico 在酷家乐做 AI+3D 产品的视角，具身 AI 的空间理解问题在室内场景已经真实存在——3DGS 生成的空间表征能不能直接接进 WAM 或 VLA 的训练管道，答案目前是"两种都在试，都没有明确答案"。Cosmos 3 的"simulator-grounded embodied spatial reasoning"是 NVIDIA 的技术赌注——用物理模拟器的 ground truth 来训练空间推理，而不是依赖纯语言/视觉的自监督信号。

  这个"没有赢家"的现状，本身就是信号：**2026年的具身 AI 投资，很大程度上是在赌架构，不是在赌应用**。比较接近 2012-2015 年深度学习初期：钱在流动，研究者知道"这个方向对了"，但还不知道"哪条路到终点"。

- **Resonance hook**: 2026年 Q1，具身 AI 世界模型吸引了 $60 亿投资。NVIDIA 在6月22日的 Cosmos 3 技术报告里说："WAMs 和 VLAs 之间，目前没有赢家。"这是在 Physical AI 上投注最重的公司对自己押注领域的坦诚判断。$60 亿进去了，两条技术路径都在，谁会赢还不知道。这种处境上一次出现在深度学习的2012-2015年。
- **Recommended priority**: medium-high

---

## Scan summary

**Sources scanned**:
- CNBC（6月26日，《China's Zhipu is closing in on top U.S. AI models with Anthropic and OpenAI held back》）
- CNBC（6月26日，《OpenAI and Anthropic face new AI reality as users shift from 'tokenmaxxing' to efficiency》）
- VentureBeat（《Z.ai's open-weights GLM-5.2 beats GPT-5.5 on multiple long-horizon coding benchmarks for 1/6th the cost》）
- Latent Space / Swyx（6月16日，AINews《GLM-5.2 is the real deal; Z.ai forecasts Open Fable by EOY》）
- Interconnects.ai（《GLM-5.2 is the step change for open agents》）
- South China Morning Post（6月26日，《China's Zhipu AI sparks new 'DeepSeek moment' with cost-effective coding model》）
- explainx.ai（《GLM-5.2 Beats Fable 5 Reasoning — China AI Response to Export Ban 2026》）
- theairankings.com（GLM-5.2 benchmarks，Z.ai 完整数据）
- TechCrunch（6月5日，《The token bill comes due》）
- Cybernews（《Uber spends entire 2026 AI budget in 4 months, sees no ROI》）
- BigGo Finance（《Silicon Valley's AI Bubble Burst: Three Months to Burn a Year's Budget, Tokenmaxxing Implodes》）
- MyGreatLearning（《Tokenmaxxing Explained: The Hidden Cost of Workplace AI》）
- NVIDIA investor relations（6月1日，Cosmos 3 官方发布）
- NVIDIA Research 技术报告（6月22日，Cosmos 3: Omnimodal World Models for Physical AI）
- Axios（6月1日，Cosmos 3 报道）
- TechTimes（6月18日，《Embodied AI World Models Attracted $6 Billion, But the LLM Parallel May Not Hold》）
- arXiv 2506.22355（Pascale Fung et al., 《Embodied AI Agents: Modeling the World》，2026年6月）
- Anthropic newsroom（无6月27-29独立新事件，排除）
- OpenAI news（o3 退休通知、无6月28-29独立事件锚点，排除）
- Demis Hassabis / Google DeepMind（6月23日 Semafor 专访"Google 仍在赢得 AI 人才"——叙事强度不及今日三候选，排除）
- Karpathy X（6月24日后无新帖相关，排除）
- Altman X（无6月27-29独立事件锚点，排除）
- Jim Fan / NVIDIA GR00T（近期无独立6月27-29事件锚点，已通过 Cosmos 3 覆盖 NVIDIA 角度，排除）
- Colorado AI Act（原法律 6月30日生效日期，但 SB 189 于5月14日已签署替代——关键事件发生在5月而非本周，排除）
- GitHub Trending AI（awesome-ai-agents-2026 汇总清单、OpenClaw 210k stars——无精确6月27-29独立叙事锚点，排除）
- YC Blog（无6月27-29独立新文章，排除）
- HN top AI posts June 28-29（主导话题：AI 安全/CVE、coding agent 工作流——无独立单一事件锚点，排除）

**Total signals found**: 约 29 个信号评估

**Why these 3**:

- **Candidate 1（Z.AI GLM-5.2，6月13/16日发布，6月26日 CNBC 主流曝光）**：**AI产品战略柱**——过去三天 SELECTED 覆盖了 组织形式变革（6月28日 Karpathy 第三范式）、深层AI思考（6月27日 dual-clock gap）、组织形式变革（6月26日 Alibaba 蒸馏攻击）——AI产品战略柱连续三天 SELECTED 未被使用；时效：CNBC 主流曝光3天前（6月26日）；MIT 权重发布13天前（6月16日）；"6月13日发布=Fable 5 被封次日"这个时间精确性在中文媒体完全缺席——中文媒体报道 GLM-5.2 停在"中国模型又赶上了"的层面，不会分析这是"美国出口管制创造的 AI 能力真空，正在被中国开源模型填补"的监管反馈回路；Z.ai 预告"年底前开源 Fable 级能力"这一前瞻信号在中文媒体几乎无战略框架分析；HIGH 优先级。

- **Candidate 2（Enterprise tokenmaxxing 终结，6月26日 CNBC）**：**AI协作实践柱**——连续四天 SELECTED 未被使用此柱；时效：3天前（CNBC 6月26日）；Uber COO 播客披露是首手数据（不是问卷，是 COO 公开承认）；"70% 代码提交来自 AI 但找不到消费者价值关联"这个矛盾在中文 AI 媒体几乎无深度分析（中文媒体会报道"Uber 用 AI 工具超预算了"，不会分析"token 消耗和价值创造之间的验证机制空白"这一结构性问题）；与 Zico 自身 AI 产品实践直接相关，可接真实经验；Amazon 排行榜关停 + Microsoft 撤销许可证两个具体数据点提供叙事厚度；HIGH 优先级。

- **Candidate 3（NVIDIA Cosmos 3 + WAMs vs VLAs，6月1/22日）**：**深层AI思考柱**——此柱6月27日刚被 SELECTED 用于 dual-clock gap；候选保留理由：①"WAMs vs VLAs no winner"来自 NVIDIA 自己（最权威的反直觉来源），有独立叙事力；② $60 亿 Q1 投资数字提供传播势能；③技术报告6月22日发布提供7天内锚点；④ 与 Zico 在酷家乐做 AI+3D 产品的空间智能背景有真实交集，可接个人判断；中文具身 AI 报道会覆盖 NVIDIA Cosmos 3 发布，但不会分析"为什么全领域投资者押注最重的公司说架构路径还没有赢家"这一深层认知问题；MEDIUM-HIGH 优先级（此柱近期已用，降为第三候选）。
