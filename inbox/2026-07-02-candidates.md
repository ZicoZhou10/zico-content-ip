---
date: 2026-07-02
status: pending_selection
---

# Today's Candidates

## Candidate 1: Fable 5 昨日全球恢复——19天关停暴露AI基础设施的政府可控开关，Amazon CEO亲自把越狱报告交给白宫（June 12 停服，June 30 解禁，July 1 全球恢复）

- **Event**: 2026年6月12日，美国商务部向Anthropic下达指令：在90分钟内在全球范围关停 **Claude Fable 5** 和 **Claude Mythos 5**。触发原因：**Amazon** 研究员发现 Fable 5 可被越狱——一种可让模型识别软件漏洞并生成漏洞利用代码的攻击路径。**Amazon CEO Andy Jassy 本人**将该报告直接递交给白宫，由此触发联邦政府行动。6月9日 Fable 5 刚刚上线，3天后即被关停。19天全球停服期间：① 无任何预警，无任何豁免（包括盟国），无任何法律正当程序要求；② 约6月26日，**Mythos 5** 率先恢复——仅面向约100家美国受信机构（白名单审批制）；③ 6月30日，美国商务部长 **Howard Lutnick** 宣布解除出口管制，条件是 Anthropic 承诺：主动检测和修复与模型相关的安全风险 + 与政府合作制定未来发布协议 + 向政府汇报在模型中发现的"恶意活动"；④ **2026年7月1日（昨天）**，Fable 5 全球恢复，覆盖 Claude Platform、Claude.ai、Claude Code 和 Claude Cowork，Pro/Max/Team 用户在7月7日前使用限额为原先50%，之后转为用量计费。Anthropic 新训练了一个分类器，针对 Amazon 报告描述的具体越狱路径，**拦截成功率超过99%**。来源：**CNBC**（2026年6月30日，《Anthropic says Trump admin has lifted export controls on Claude Fable 5 and Mythos 5》）、**VentureBeat**（2026年7月1日，《Anthropic is bringing back Claude Fable 5 globally after US lifts export control order》）、**Forbes**（2026年7月1日，《Trump Administration Lifts Export Controls on Anthropic's Fable 5 and Mythos 5 AI Models》）、**MarketScale**（2026年7月1日，《Fable 5 and Mythos 5 Are Back. What the 19-Day Shutdown Taught Every Enterprise About AI as Infrastructure.》）、**The Hacker News**（2026年7月1日，《Anthropic Restores Claude Fable 5 After U.S. Lifts Jailbreak-Linked Export Controls》）、**Anthropic 官方博客**（《Redeploying Claude Fable 5》）。
- **Source**: https://www.cnbc.com/2026/06/30/anthropic-says-trump-admin-has-lifted-export-controls-on-claude-fable-5-and-mythos-5.html | https://venturebeat.com/technology/anthropic-is-bringing-back-claude-fable-5-globally-after-us-lifts-export-control-order-where-can-enterprises-access-it | https://www.forbes.com/sites/siladityaray/2026/07/01/trump-administration-lifts-export-controls-on-anthropics-fable-5-and-mythos-5-ai-models/ | https://www.marketscale.com/industries/software-and-technology/fable-5-and-mythos-5-are-back-what-the-19-day-shutdown-taught-every-enterprise-about-ai-as-infrastructure | https://thehackernews.com/2026/07/anthropic-restores-claude-fable-5-after.html | https://www.anthropic.com/news/redeploying-fable-5
- **Timeliness**: 1 天前（2026年7月1日全球恢复）；关停事件 20 天前（6月12日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 这件事的核心不是越狱，不是安全事件，是关于 **AI 基础设施的控制权归属** 这个问题在现实中第一次被测试。

  有一个关系需要先看清楚：Amazon 是 Anthropic 最大的投资方（2023年起已承诺投资约50亿美元），同时也是 Anthropic 最大的云服务合作伙伴（Claude API 在 AWS Bedrock 上运行）。6月12日，是 Amazon 研究员发现了 Fable 5 的越狱路径，是 Amazon CEO Andy Jassy 亲自把这份报告递给了白宫。同一家公司，既是 Anthropic 最大的结构性支持者，也是触发政府关停 Anthropic 旗舰模型的那只手。

  这种关系在商业史上很少见，但在 AI 基础设施时代可能会越来越常见：**当 AI 模型变成基础设施，监管它的人和运营它的人在产业链上必然有重叠**。Jassy 把报告交给白宫，是 CEO 在尽职——国家安全风险在他的运营环境（AWS）里被发现，他有义务上报。但结果是，他的合作伙伴的旗舰产品被关停了19天。这不是背刺，这是 AI 基础设施时代的系统性现实：安全合规义务和商业合作义务会发生结构性冲突。

  解禁的条件也值得看：Anthropic 承诺向政府汇报在模型中发现的"恶意活动"。翻译成更直白的产品语言：**全球最先进的 AI 模型的运营商，现在是美国国家安全信息体系的一个上报节点**。这不仅仅是 Anthropic 的处境，这是所有依赖前沿 AI 能力的企业需要认真考虑的基础设施假设：你的工具链里有一个政府可控的开关，随时可以在90分钟内关掉。

  19天停服给每个把 Fable 5 接进生产流程的企业上了一课：**AI 模型不是云服务（有 SLA、有灾备、有多可用区），它是政府可以随时施加出口管制的战略资产**。没有任何现有的 AI 采购合同覆盖这种风险。Agentjacking 安全研究报告（6月12日 Sentry 越狱）还没讨论完，Fable 5 已经因为不相关的越狱被关停19天了。现在 Fable 5 回来了，但解禁条件里已经嵌入了下一次关停所需要的信息上报义务。

  中文媒体会报"Fable 5 解封了，好消息"，不会分析：**解封的代价是 Anthropic 正式成为美国国家安全信息链的一部分**——以及这对把 Claude 接进产品的公司意味着什么。

- **Resonance hook**: 19天前，Fable 5 在90分钟内被全球关停。Amazon CEO 亲自把越狱报告交给了白宫。Amazon 是 Anthropic 的最大投资方，也是触发关停的那只手。昨天，Fable 5 回来了——条件是 Anthropic 承诺向政府汇报它在自己模型里发现的"恶意活动"。这是 AI 模型历史上第一次，最强的商业 AI 被政府关停、谈判、带着监控义务恢复。企业 AI 基础设施里有一个政府可控的开关，没有写在任何合同里。
- **Recommended priority**: high

---

## Candidate 2: Claude Sonnet 5 成为所有用户的默认模型——"Agentic"从旗舰功能变成免费账户基线，但新tokenizer使实际成本高于标价（June 30）

- **Event**: 2026年6月30日，Anthropic 发布 **Claude Sonnet 5**，定位为"有史以来最有 agentic 能力的 Sonnet 模型"，并立即成为 **claude.ai 所有 Free 和 Pro 用户的默认模型**。核心基准：① **SWE-bench Pro（长时程编程任务）**：63.2%（Claude Opus 4.8：69.2%）；② **OSWorld-Verified（计算机操作 Agent）**：81.2%（vs Opus 4.8 的 83.4%）；③ **Terminal-Bench 2.1（终端 Agent 任务）**：80.4%，**超过 Opus 4.8 的 74.6%**；④ **BrowseComp Agentic Search**：84.7%。定价结构：介绍价（至2026年8月31日）**$2/百万输入token + $10/百万输出token**；之后调整为 $3/$15。Claude Opus 4.8 定价为 $5/$25。**关键隐藏细节**：Sonnet 5 使用了**新的 tokenizer**，同样的文本会比旧 tokenizer 生成约 **1.35 倍的 token 数量**——实际成本节省比标价表面呈现的更少（介绍价 60% 折扣中，有 ~35% 被 token 通胀抵消）。Sonnet 5 同日上线于 **GitHub Copilot**（GitHub Changelog，6月30日）和 **AWS Bedrock**。Anthropic 描述 Sonnet 5 "可以制定计划、使用浏览器和终端等工具，并以几个月前还需要更大更贵的模型才能完成的水平自主运行"。来源：**TechCrunch**（2026年6月30日，《Anthropic launches Claude Sonnet 5 as a cheaper way to run agents》）、**TechRadar**（2026年6月30日，《Claude Sonnet 5 is here, and the 'most agentic Sonnet model yet' shows that the AI war is shifting from chat to agents》）、**VentureBeat**（2026年6月30日，《Anthropic launches Claude Sonnet 5 at a steep discount to its top model as the company races toward a blockbuster IPO》）、**Finout**（《Claude Sonnet 5 Pricing 2026: The Hidden Costs — and Real Savings — Behind the 'Cost-Neutral' Launch》）、**Anthropic 官方博客**（《Introducing Claude Sonnet 5》）、**GitHub Changelog**（2026年6月30日，《Claude Sonnet 5 is generally available for GitHub Copilot》）。
- **Source**: https://techcrunch.com/2026/06/30/anthropic-launches-claude-sonnet-5-as-a-cheaper-way-to-run-agents/ | https://www.techradar.com/ai-platforms-assistants/claude/claude-sonnet-5-is-here-and-the-most-agentic-sonnet-model-yet-shows-that-the-ai-war-is-shifting-from-chat-to-agents | https://venturebeat.com/technology/anthropic-launches-claude-sonnet-5-at-a-steep-discount-to-its-top-model-as-the-company-races-toward-a-blockbuster-IPO | https://www.finout.io/blog/claude-sonnet-5-pricing-2026-the-hidden-costs-and-real-savings-behind-the-cost-neutral-launch | https://www.anthropic.com/news/claude-sonnet-5 | https://github.blog/changelog/2026-06-30-claude-sonnet-5-is-generally-available-for-github-copilot/
- **Timeliness**: 2 天前（2026年6月30日）
- **Topic pillar**: Agent经济
- **Zico's angle**: Sonnet 5 的基准数字没什么特别值得展开的——Anthropic 每次发中间层模型都会有类似的"接近旗舰水平，更便宜"的叙事。真正值得分析的是两个被大多数人忽略的信号。

  第一个信号：**Anthropic 把 Sonnet 5 设成了所有用户的默认模型，包括免费账户**。这是一个产品策略决策，不是功能特性决策。Agentic 能力——即让 AI 自主制定计划、使用工具、执行多步骤任务——在6个月前还是 Opus 层级的专属能力。现在 Anthropic 把这个能力推到了所有用户的默认体验里，包括那些从来没为 AI 付过一分钱的用户。这是 Anthropic 在说：**agentic 不是旗舰差异点，agentic 是基线**。中间层模型就应该默认具备 agentic 能力，旗舰层的差异在于精度和复杂任务极限，不在于"能不能自主运行"。

  这和 Agent 经济的成熟轨迹完全吻合：第一阶段，agentic 能力是少数人的实验性功能（GPT-4 Agents Preview，2023）；第二阶段，agentic 能力是旗舰用户的高级选项（Opus/Claude 3.5 时代）；第三阶段，agentic 能力是所有用户的默认体验（现在，Sonnet 5 作为 Free 用户默认模型）。当某个能力成为免费的默认功能，意味着它在商业价值生命周期里已经完成了从差异化优势到商品化基线的转变。

  第二个信号：**定价透明度问题**。Sonnet 5 的介绍价 $2/百万 token 比 Opus 4.8 的 $5/百万 token 便宜60%——但新的 tokenizer 让同样的文本消耗1.35倍的 token。这意味着实际成本节省约35%，不是60%。这在 GitHub Copilot 计量计费震惊开发者（$29/月→$750/月，昨天候选）的同一周发布，让 AI 定价的"真实成本 vs 标价表面"问题再次暴露：**AI 产品的定价越来越难被一个数字理解，需要知道 tokenizer 行为、计费周期、模型选择等底层细节，才能准确预测实际支出**。

  对做 AI 产品的人，这两个信号的组合有一个直接的影响：如果你今天正在用 Opus 4.8 跑 agentic 工作流，切换到 Sonnet 5 的实际成本节省大约是35%（不是60%）；而你的用户现在已经通过免费账户接触到了接近 Opus 水平的 agentic 能力——这会重新校准他们对"够用"的判断。

- **Resonance hook**: 昨天，Anthropic 把 Sonnet 5 设成了 claude.ai 所有人的默认模型，包括免费用户。这个模型在终端 Agent 任务上实际上超过了 Opus 4.8。"Agentic AI"从旗舰差异点变成了免费基线。但这里有一个隐藏的定价问题：Sonnet 5 用了新的 tokenizer，同样的文本要消耗1.35倍的 token——实际成本节省大约35%，不是标价说的60%。在 GitHub Copilot 用量冲击的同一周，AI 定价里藏着越来越多需要自己算的细节。
- **Recommended priority**: high

---

## Candidate 3: Agents-A1——35B模型用"视野缩放"超越万亿参数模型，重写Agent能力的成本方程（June 29，arXiv 2606.30616）

- **Event**: 2026年6月29日，**InternScience 团队**（上海 AI Lab 关联研究组）在 arXiv（论文编号 **2606.30616**）发布 **Agents-A1**，提出论点：**"Scaling the Horizon, Not the Parameters"（缩放视野，而非缩放参数）**。核心发现：一个 **35B 参数的 MoE 架构**，通过系统性地缩放 **长视野轨迹**（long-horizon trajectories，平均 45K tokens/轨迹）和 **异质 Agent 能力**（long-horizon search、engineering tasks、scientific research、instruction following、general/scientific agentic tasks 六类），达到了 **万亿参数（1T+）级别模型**（Kimi-K2.6、DeepSeek-V4-pro）的 benchmark 性能：**SEAL-0 56.4、IFBench 80.6、HiPhO 46.4**。训练采用三阶段方案：全领域 SFT 对齐 → domain-specific 能力缩放 → verifier-guided 强化学习。关键技术创新："长视野知识-行动基础设施"——将外部知识库、工具调用、环境观察、验证器输出统一编排进 agentic 轨迹，让模型在任务执行过程中形成持续更新的工作记忆。来源：**arXiv 2606.30616**（2026年6月29日，《Scaling the Horizon, Not the Parameters: Reaching Trillion-Parameter Performance with a 35B Agent》）、**Hugging Face Papers**（2026年6月30日，论文高亮收录）、**explainx.ai**（《Agents-A1 — 35B MoE Agent Model: June 2026》）、**InternScience GitHub**（https://github.com/InternScience/Agents-A1）。
- **Source**: https://arxiv.org/abs/2606.30616 | https://huggingface.co/papers/2606.30616 | https://explainx.ai/blog/agents-a1-internscience-35b-moe-agent-model-2026 | https://github.com/InternScience/Agents-A1/
- **Timeliness**: 3 天前（2026年6月29日，arXiv 首发）
- **Topic pillar**: 深层AI思考
- **Zico's angle**: AI 领域过去5年的主叙事是"参数缩放定律"：训练更多数据、更大模型，性能就会提升。这条叙事催生了 GPT-4（约1.8T参数）、Kimi-K2.6（约1T参数），也催生了数以千亿计的算力投资。

  Agents-A1 的论文做了一个直接的反驳实验：**用35B参数+视野缩放，达到1T+参数模型的性能**。不是接近，是在 SEAL-0、IFBench、HiPhO 等 agentic benchmark 上正面对比。

  两种缩放方式的成本结构完全不同：参数缩放（Scaling Model Size）= **训练时一次性投入**，成本在训练阶段，之后每次推理成本恒定。视野缩放（Scaling Horizon）= **推理时按任务复杂度投入**，每次执行的计算量跟着视野长度线性增长（平均45K tokens/轨迹，就是说每次执行要处理45K token 的上下文）。这两种路径的应用场景也完全不同：参数缩放适合那些"每次对话都要精确"的任务（比如短对话、代码补全、单次问答）；视野缩放适合那些"可以花更多时间思考但结果更重要"的任务（比如长时程研究、复杂代码库修改、多步骤规划）。

  对 AI Agent 产品的直接含义：**你为 Agent 选模型的问题，比"哪个模型更强"要复杂得多**。如果你的 Agent 主要做长视野任务（比如 Claude Code 改一个复杂 codebase），用一个设计了更好工具访问权限和更长轨迹的较小模型，可能比直接调 Opus 旗舰更高效。这个结论和 VirBench 的发现（工具集成质量比模型质量对科学 AI 准确率的影响更大）指向同一方向：**AI 能力的瓶颈经常不在参数大小，在工具设计、轨迹工程和验证器质量**。

  另一个背景值得注意：InternScience 是中国研究团队，论文6月29日发出时，Fable 5 刚结束关停第17天。在美国出口管制把最前沿闭源模型锁住的同一时期，中国研究者正在发表"用更小的参数达到更强的 agentic 性能"的论文。这两件事放在一起，构成了 AI 能力竞争的一个真实截面：**规模不是前沿 AI 能力的唯一路径，也不是最难被复制的那条护城河**。

- **Resonance hook**: 一个35B参数的模型在 Agent 基准上超过了万亿参数级别的 Kimi 和 DeepSeek。不是靠更大的模型，靠的是更长的工具调用轨迹和更好的任务结构设计。如果这个结论成立，"买更强的旗舰模型"不是 Agent 产品优化的唯一出路，也不是最便宜的那条。这篇论文是中国研究团队在美国出口管制升级的同一周发出来的。
- **Recommended priority**: medium-high

---

## Scan summary

**Sources scanned**:
- CNBC（2026年6月30日，《Anthropic says Trump admin has lifted export controls on Claude Fable 5 and Mythos 5》）
- VentureBeat（2026年7月1日，《Anthropic is bringing back Claude Fable 5 globally after US lifts export control order》）
- Forbes（2026年7月1日，《Trump Administration Lifts Export Controls on Anthropic's Fable 5 and Mythos 5 AI Models》）
- MarketScale（2026年7月1日，《Fable 5 and Mythos 5 Are Back. What the 19-Day Shutdown Taught Every Enterprise About AI as Infrastructure.》）
- The Hacker News（2026年7月1日，《Anthropic Restores Claude Fable 5 After U.S. Lifts Jailbreak-Linked Export Controls》）
- Anthropic 官方博客（《Redeploying Claude Fable 5》，2026年7月1日）
- 9to5Mac（2026年7月1日，《Claude Fable 5 cleared to return as US lifts Anthropic's export control restriction》）
- MindStudio（《AI Model Export Controls Explained: What the Claude Fable 5 Shutdown Means for Enterprise Builders》）
- TechCrunch（2026年6月30日，《Anthropic launches Claude Sonnet 5 as a cheaper way to run agents》）
- TechRadar（2026年6月30日，《Claude Sonnet 5 is here, and the 'most agentic Sonnet model yet'》）
- VentureBeat（2026年6月30日，《Anthropic launches Claude Sonnet 5 at a steep discount to its top model》）
- Finout（《Claude Sonnet 5 Pricing 2026: The Hidden Costs — and Real Savings — Behind the 'Cost-Neutral' Launch》）
- Anthropic 官方博客（《Introducing Claude Sonnet 5》，2026年6月30日）
- GitHub Changelog（2026年6月30日，《Claude Sonnet 5 is generally available for GitHub Copilot》）
- The New Stack（《Anthropic Sonnet 5: It closes the gap with Opus 4.8, and is cheap until August》）
- AWS Blog（《Introducing Claude Sonnet 5 on AWS: Anthropic's most capable Sonnet model》，2026年6月30日）
- arXiv 2606.30616（2026年6月29日，《Scaling the Horizon, Not the Parameters: Reaching Trillion-Parameter Performance with a 35B Agent》）
- Hugging Face Papers（2606.30616 收录，2026年6月30日高亮）
- explainx.ai（《Agents-A1 — 35B MoE Agent Model: June 2026》）
- InternScience GitHub（https://github.com/InternScience/Agents-A1/）
- Adversa AI（2026年6月30日，GuardFall — 10/11开源 AI coding agents shell injection漏洞——已排除，与Agentjacking主题重叠）
- SecurityWeek（2026年6月30日，《Decades-Old Bash Tricks Expose AI Coding Agents to Supply Chain Attacks》——同上排除）
- llm-stats.com（《AI Updates Today — July 2026》——汇总源，已用于发现 Sonnet 5 和 Fable 5 线索）
- Nat Friedman "Entire"（$60M seed，git observability for AI agents）——发布时间为2026年2月，超出30天窗口，排除
- OpenAI S-1 保密递交（2026年6月1日，超出7天最优窗口，叙事强度不及三个候选，排除）
- Karpathy / Altman X（无6月30日-7月2日独立可锚定新帖，排除）
- Jim Fan / NVIDIA GR00T N1.6——发布时间不确定，叙事锚点弱于三个候选，排除
- GitHub Trending（AI coding agent工具集中——无7月1-2日独立叙事锚点，排除）
- HN 高热AI帖（GuardFall + Fable 5 恢复为主导话题，无额外独立候选）

**Total signals found**: 约 24 个信号评估

**Why these 3**:

- **Candidate 1（Fable 5 恢复，7月1日）**：**组織形式変革柱**——过去7天 SELECTED 记录中，此柱距今最远（最近一次约在6月23日 057-behavioral-signature），为间隔最长的未用柱之一；时效最强（昨天）；Amazon CEO亲自上报白宫这一细节在中文媒体完全缺失（中文报道停在"Fable 5 解封了"），没有人分析 Amazon 作为投资方+触发者的双重身份所揭示的 AI 治理结构性矛盾；"解禁条件=向政府汇报恶意活动"这一信息在中文媒体几乎无深度分析；与6月29日候选（GLM-5.2 填补能力真空）形成完整叙事闭环：同一个事件，从"禁令创造机会"到"禁令解除后的新约束"；**HIGH 优先级**。

- **Candidate 2（Claude Sonnet 5，6月30日）**：**Agent経済柱**——7月1日候选 SELECTED（061 virbench → AI产品战略柱）后，Agent経済柱本身6月30日被Agentjacking覆盖（选中），距今2天；但 Sonnet 5 的角度（agentic能力商品化 + tokenizer隐性成本）完全不同于 Agentjacking（执行层安全）和 GitHub Copilot 计量冲击（计费机制）；"Free用户默认agentic"这一产品策略决策在中文媒体停在规格对比，无战略分析；tokenizer 1.35x 通胀导致实际成本节省被夸大这个隐藏细节，finout.io 的分析几乎无中文转载；与 Candidate 1 同在7月1日发生，两个候选共同构成 Anthropic 在极压力下的战略动作集合（Fable 5 返回 + Sonnet 5 普惠化 = 同一天的双重产品事件）；**HIGH 优先级**。

- **Candidate 3（Agents-A1，6月29日）**：**深层AI思考柱**——7月1日候选 SELECTED 中此柱未被选中（候选3 Gemini 2.5 Pro Deep Think 为medium-high优先级）；arXiv 来源符合 Tier 2 源；"35B超越1T参数"的论点是反直觉判断，属 B 类钩子（钩子结论式）；"视野缩放 vs 参数缩放"这一技术框架差异在中文 AI 媒体几乎无深度分析（中文媒体会转载"中国模型赶上了"，不会分析两种缩放方式的成本结构差异及产品决策含义）；InternScience 是中国研究团队，在出口管制背景下有额外叙事价值，与 Candidate 1 的地缘AI竞争背景形成共鸣；与7月1日已选中的 VirBench 候选（工具质量比模型质量更决定 AI 科学准确率）有深层理论一致性（两者都在质疑"更强的模型=更好的结果"）；**MEDIUM-HIGH 优先级**。
