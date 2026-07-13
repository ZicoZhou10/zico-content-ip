---
date: 2026-07-13
status: pending_selection
---

# Today's Candidates

## Candidate 1: 陶哲轩用 AI coding agent 在几小时内移植了他27年前的 Java 数学可视化工具——代理发现了他从未知晓的2个 bug，还完成了他1999年放弃的"相对论可视化"项目（July 11）

- **Event**: 2026年7月11日，菲尔兹奖得主、UCLA 数学教授 **Terence Tao（陶哲轩）** 在个人博客（terrytao.wordpress.com）发表文章《Old and new apps, via modern coding agents》。内容：他从1999年起为复变分析和线性代数课程用 Java 1.0 编写了约24个数学可视化 Applet，但随着网页标准停止支持 Java，这些 Applet 逐渐失效。7月初，他让一个 LLM-based coding agent 把所有 Applet 移植到 JavaScript——**几小时内完成**（~24个）。移植过程中，agent 发现了他1999年原始代码里**2个他本人从未察觉的 bug**。此外，他还提到了一个1999年因"实现复杂度太高"而**放弃了27年**的项目：一款"Minkowski 空间里的 Inkscape"（相对论可视化工具）。他花了"几小时 vibe coding"，AI agent 完成了这个被搁置27年的项目。文章发布次日（7月12日）登上 Hacker News 首页第一位。TechTimes 标题：《AI Agents Ported Tao's 27-Year-Old Math Code in Hours and Found Two Bugs He Had Missed》。
- **Source**: https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/ | https://news.ycombinator.com/item?id=48880170 | https://www.techtimes.com/articles/320238/20260712/ai-agents-ported-taos-27-year-old-math-code-hours-found-two-bugs-he-had-missed.htm
- **Timeliness**: 2天前（2026年7月11日，陶哲轩本人博客；7月12日 HN 首页第一位）
- **Topic pillar**: AI协作实践
- **Zico's angle**: 这件事真正有意思的地方不是"大数学家用AI写代码"——而是两个具体的细节，每一个都指向一个不同的问题。

  第一个细节：agent 发现了2个他在1999年写的代码里、存在了27年的 bug，是他本人从未知道的。这不是 AI 替代人类做代码移植——这是 AI 提供了一个人类注意力维持不了的质量层。一个写了27年的函数，你不会反复检查它。你认为它是对的，因为"它一直在工作"。Agent 没有这种先入为主。这是 AI 协作的一个具体功能：**扮演那个永远不会被习惯遮蔽视野的检查者**。

  第二个细节更有意思："Minkowski 空间里的 Inkscape"。这个项目1999年就有了，陶哲轩知道想要什么，知道它应该怎么工作，但因为"实现复杂度太高"就放弃了。27年来，这个想法一直是想法。然后他花几个小时 vibe coding，AI agent 做完了。这是 AI 对知识工作者最根本的价值变化，不是效率——是**执行壁垒的消失**。过去，有多少值得存在的东西，因为执行成本太高而永远停在"想法"阶段？

  中文媒体会报"世界顶级数学家也在用 AI 写代码"，不会问：**当执行壁垒消失，多少被搁置27年的想法会重新被完成？**

- **Resonance hook**: 7月11日，陶哲轩在博客写了一件事：他让 AI agent 在几小时内移植了他1999年写的24个 Java 数学 Applet。Agent 还顺手找到了他写了27年、自己从没发现的2个 bug。他还让 agent 完成了一个他在1999年构思、因为"太难实现"而放弃的项目——一款相对论可视化工具。从构思到放弃，中间过去了27年。现在，"太难实现"这个理由失效了。你搁置的那些想法，理由还成立吗？
- **Recommended priority**: high

---

## Candidate 2: Apple 起诉 OpenAI 窃取硬件商业机密——硬件主管 Tang Tan 被指控要求应聘者带"实物零件"来面试，Apple 称 OpenAI 硬件业务"烂到骨子里"（July 10）

- **Event**: 2026年7月10日，**Apple** 在加利福尼亚北区联邦法院对 **OpenAI** 及 **io Products**（Jony Ive 的设计公司，2025年被 OpenAI 以 **$65亿** 收购）提起诉讼，指控窃取硬件商业机密。核心指控分两条线：（1）**Tang Tan**（唐坦），前 Apple 工作**24年**、曾任 iPhone 与 Apple Watch 产品设计副总裁，现为 OpenAI 首席硬件官。Apple 指控他：**在招聘过程中要求仍在 Apple 任职的候选人带"实物零件"来面试做"show and tell"**；使用 Apple 内部保密项目代号引导候选人讨论；指导离职员工如何绕过 Apple 安保程序。（2）**Chang Liu**（刘翔），前 Apple 高级系统电气工程师，2026年加入 OpenAI 前**偷走一台 Apple 发放的笔记本电脑**，并下载了"数十份 Apple 机密硬件相关文件，包括大量关于未发布产品的详细信息、工程演示、技术规格和专有项目数据"。Jony Ive 本人未被列为被告，Apple 未指控其个人不当行为。Apple 对 OpenAI 硬件业务的定性原话："**rotten to its core**（烂到骨子里）"。来源：Bloomberg（《Apple Sues OpenAI for Trade Secret Theft in Blockbuster Case》）、CNBC（《Apple sues OpenAI alleging trade secret theft, says scheme was 'at every level'》）、TechCrunch（《Apple sues OpenAI over alleged trade secret theft》）、Fortune、CNN、Axios（均为7月10日同日报道）。
- **Source**: https://www.bloomberg.com/news/articles/2026-07-10/apple-sues-openai-for-trade-secret-theft-in-blockbuster-case | https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html | https://techcrunch.com/2026/07/10/apple-sues-openai-over-alleged-trade-secret-theft/ | https://fortune.com/2026/07/10/apple-openai-lawsuit-trade-secrets-theft-allegations/ | https://www.axios.com/2026/07/10/apple-sues-openai-trade-secret-theft
- **Timeliness**: 3天前（2026年7月10日，Bloomberg/CNBC/TechCrunch/Fortune/CNN/Axios 六家一线媒体同日报道）
- **Topic pillar**: AI产品战略
- **Zico's angle**: 这件事真正值得分析的不是诉讼本身，而是诉讼揭示的结构性逻辑：**当 AI 软件公司决定进入硬件，它们需要的不只是设计师——它们需要40年的供应链机构记忆，而那东西只存在于 Apple 的工程师脑子里。**

  先把 OpenAI 的硬件战略逻辑说清楚。OpenAI 花 $65亿 买了 Jony Ive 的 io Products。表面上是"Jony Ive 的设计基因"。但设计审美是最不稀缺的东西——Ive 的联系名单随便一个设计师都找得到。OpenAI 真正需要的是：怎么把消费级硬件推向量产，怎么和芯片供应商谈判，怎么做热管理、天线设计、摄像头模组的工程决策。这些能力在 Apple 的工程体系里沉淀了40年，是隐性机构知识，不写在任何文档里，只存在于做过这些决策的人身上。

  Tang Tan 的24年 Apple 履历（VP of product design for iPhone and Apple Watch）正是这种机构知识的载体。而 Apple 描述的招聘行为——要求候选人"带实物零件来做 show and tell"——是把这种机构知识从 Apple 提取出来最直接的方式：不是问"你知道什么"，是"把你知道的东西的实物证明带来"。

  这件事对 AI 产品战略的框架性含义是：进入硬件不等于有硬件能力。进入硬件意味着需要获取供应链机构知识，而供应链机构知识是现有硬件寡头的最深护城河。当 OpenAI 试图跨越这条护城河，Apple 回应的不是竞争——是诉讼。"烂到骨子里"这句话，是 Apple 在表态：**硬件领域有一套不成文的获取规则，AI 公司刚刚越线了。**

  对 Zico 关注的 AI 产品战略：这是 AI 时代第一个清晰的案例，说明"软件公司进入硬件"这件事的隐性成本不是研发费用，而是**与现有硬件寡头的正面法律冲突**。任何 AI 公司如果走这条路，都需要想清楚：你想要的供应链知识是否只能通过这种方式获取？如果是，你准备好应对 Apple 级别的法律机器了吗？

- **Resonance hook**: 7月10日，Bloomberg 等六家一线媒体同日报道：Apple 起诉 OpenAI 窃取硬件商业机密。关键细节：OpenAI 首席硬件官 Tang Tan（前 Apple VP，在 Apple 待了24年，负责 iPhone 和 Apple Watch 的产品设计）被指控**在招聘过程中要求仍在 Apple 任职的候选人把"实物零件"带来面试做"show and tell"**。Apple 对 OpenAI 硬件业务的评价：**"rotten to its core"（烂到骨子里）**。OpenAI 花 $65亿 买了 Jony Ive 的设计公司来造硬件——当你试图通过挖人来获取40年的 Apple 供应链机构知识，Apple 给出的回应不是竞争，是联邦诉讼。
- **Recommended priority**: high

---

## Candidate 3: Prime Intellect 完成 $130M Series A——帮企业自建 AI Agent 而非依赖 Anthropic/OpenAI，Nvidia/ICONIQ/Perplexity/Harvey/Cognition 创始人联合背书（July 8）

- **Event**: 2026年7月8日，**Prime Intellect**（成立于2024年，总部旧金山）完成 **$130M Series A**，估值达 **$10亿**。本轮由 **Radical Ventures** 领投，参与方包括：**Nvidia Ventures**、**Intel Capital**、**Dell Technologies Capital**、**ICONIQ**，以及 **Aravind Srinivas（Perplexity CEO）**、**Winston Weinberg（Harvey 联创）**、**Jeff Wang（Cognition 联创）**、**Aaron Levie（Box CEO）**等知名个人投资人。公司定位：帮助企业**不依赖 Anthropic、OpenAI、Google 等前沿实验室**，自建和训练自己的 AI Agent 系统。核心产品架构："全栈" AI Agent 开发平台，包括：（1）计算资源接入、（2）强化学习训练框架、（3）Agent 评测工具体系。商业模式：模块化市场化访问，客户按需选择工具，不需要全栈捆绑购买。现有客户：**Ramp、Zapier、Flapping Airplanes** 等。TechCrunch 标题：《Prime Intellect raises $130M Series A to help enterprises build their own AI agents》。PYMNTS 标题：《Prime Intellect Raises $130 Million to Help Companies Train AI Agents》。
- **Source**: https://techcrunch.com/2026/07/08/prime-intellect-raises-130m-series-a-to-help-enterprises-build-their-own-ai-agents/ | https://www.pymnts.com/news/investment-tracker/2026/prime-intellect-raises-130-million-to-help-companies-train-ai-agents/ | https://finance.yahoo.com/technology/ai/articles/prime-intellect-raises-130m-series-162238596.html
- **Timeliness**: 5天前（2026年7月8日，TechCrunch 报道）
- **Topic pillar**: Agent经济
- **Zico's angle**: 这件事真正值得注意的不是融资金额，而是**谁在投、投的逻辑是什么**——因为这个投资人名单本身就是一张 Agent 经济进入新阶段的信号地图。

  先把 Prime Intellect 的核心命题说清楚：如果你是一家严肃的企业，你的 AI Agent 应该跑在谁的基础设施上？答案在过去两年是默认的：Anthropic API 或 OpenAI API。Prime Intellect 的押注是：这个答案正在改变。他们做的事情是把"训练和运行自己的 Agent"这件事的成本和复杂度压到企业可接受的范围——计算、RL 框架、评测，全栈打包，但模块化。

  投资人名单的含义需要拆开读。**Nvidia Ventures 进场**：Nvidia 的利益在于更多 GPU 训练需求——如果更多企业自训 Agent，Nvidia 的市场就扩大了。**Perplexity 的 Aravind Srinivas、Harvey 的 Winston Weinberg、Cognition 的 Jeff Wang 作为个人投资人**：这三家都是在前沿实验室 API 之上建产品的公司——他们在投 Prime Intellect，是在用自己的判断告诉市场：**前沿实验室不会永远是 Agent 的供应方**，而这个判断来自他们实际经历过的供应商依赖成本。

  这件事和微软 MAI 替换 OpenAI/Anthropic（7月7日）放在一起读，会看到同一个方向的两侧：大企业（微软）在自建模型替换 API，中企业在用 Prime Intellect 这样的平台自训 Agent。从两侧同时压缩，前沿实验室 API 作为"企业 AI 基础设施"的垄断地位，正在被 make vs. buy 决策重新定价。

  对 Zico 的 Agent 经济框架：**Agent 经济第一阶段是"用谁的 Agent"，第二阶段是"谁拥有 Agent 训练数据和能力"**。Prime Intellect 的 $130M 是第二阶段开始的资金信号。

- **Resonance hook**: 7月8日，Prime Intellect 完成 $130M A 轮，$10亿估值。投资人：Nvidia Ventures、ICONIQ，以及 Perplexity CEO Aravind Srinivas、Harvey 联创、Cognition 联创个人跟投。公司做什么：帮企业自建 AI Agent，不依赖 Anthropic 和 OpenAI。同一周，微软把 Excel 和 Outlook 里的 Anthropic/OpenAI 换成了自家 MAI 模型。大企业在自建模型，中小企业在用 Prime Intellect 自训 Agent。从两侧同时压缩——前沿实验室 API 作为企业基础设施的地位，正在被重新定价。Nvidia 也在投资者名单里：更多企业自训，更多 GPU 需求。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**:
  - terrytao.wordpress.com（2026年7月11日，《Old and new apps, via modern coding agents》——陶哲轩本人博客）
  - TechTimes（2026年7月12日，《AI Agents Ported Tao's 27-Year-Old Math Code in Hours and Found Two Bugs He Had Missed》）
  - Hacker News（2026年7月12日，HN 首页第一位，item id 48880170）
  - Bloomberg（2026年7月10日，《Apple Sues OpenAI for Trade Secret Theft in Blockbuster Case》）
  - CNBC（2026年7月10日，《Apple sues OpenAI alleging trade secret theft, says scheme was 'at every level'》）
  - TechCrunch（2026年7月10日，《Apple sues OpenAI over alleged trade secret theft》）
  - Fortune（2026年7月10日，《Apple accuses OpenAI, and former design star Jony Ive's io Products firm, of stealing hardware trade secrets in blockbuster lawsuit》）
  - CNN（2026年7月10日，《Apple accuses OpenAI of using stolen trade secrets to create its upcoming AI gadgets》）
  - Axios（2026年7月10日，《Apple sues OpenAI for trade secret theft》）
  - TechCrunch（2026年7月8日，《Prime Intellect raises $130M Series A to help enterprises build their own AI agents》）
  - PYMNTS（2026年7月8日，《Prime Intellect Raises $130 Million to Help Companies Train AI Agents》）
  - Yahoo Finance（2026年7月8日，Prime Intellect 报道）
  - BuildFastWithAI（2026年7月12日，《AI News Today July 12 2026: 15 Biggest Stories》）
  - Medium/David Akpovi（2026年7月12日，《AI NEWS: Week of July 6 to July 12, 2026》）
  - ZoneTechify（2026年7月13日，《Latest AI News July 13 2026》）
  - asanify（2026年7月12日，《AI News Digest, July 12: Agentic AI Runtime Security Moves Into the Enterprise Stack》）
  - Gemini 3.5 Pro（计划7月17日发布——尚未发布，无事件锚点，排除）
  - Qualcomm/Tenstorrent（Jim Keller 6月30日否认收购谈判，Qualcomm 转向收购 Modular $39亿——收购 Modular 无具体日期确认，Tenstorrent 否认已超出信号范围，排除）
  - Claude Sonnet 5 tokenizer 价格争议（6月30日发布，已13天前——超出7天窗口，排除）
  - Anthropic Claude Science（6月30日发布——超出7天窗口，排除）
  - Qwen-AgentWorld（6月24日发布——超出7天窗口，排除）
  - Boston Dynamics + Gemini Robotics（4月8日正式上线——超出窗口，排除）
  - ICML 2026 Seoul（7月6日开幕——7天边界，学术信号，信号强度低，排除）

- **Total signals found**: 约25个信号评估

- **Why these 3**:
  - **Candidate 1（陶哲轩 coding agent 博客，7月11日）**：**AI协作实践柱**——该柱在过去3天（7月10-12日）未被覆盖，是最高优先空缺；陶哲轩是全球最受认可的在世数学家（菲尔兹奖），他的个人博客是主动分享、非企业公关话语；"agent 发现27年未知 bug"和"完成27年被搁置项目"两个具体细节直接指向 AI 协作的真实价值变化；7月12日登上 HN 首页第一位是额外信号验证；与 Zico"co-thinking with Claude"的个人实践框架直接共鸣；中文圈信息差极大（会报"数学家用AI"，不会分析执行壁垒消失对知识工作的结构性影响）；**HIGH 优先级**。
  - **Candidate 2（Apple 起诉 OpenAI 硬件商业机密，7月10日）**：**AI产品战略柱**——该柱在过去3天均有覆盖但今日这个角度完全不同（前3天：Grok 4.5 垂直整合、ChatGPT Work 架构选择、MAI 替换 API 成本路由；今日：AI 软件公司进入硬件遭遇法律壁垒）；Bloomberg+CNBC+TechCrunch+Fortune+CNN+Axios 六家一线媒体同日报道，信号强度最高；"带实物零件来面试"这个细节极具冲击力且高度可验证；与 OpenAI $65亿 IO Products 收购的战略背景深度关联；3天前，时效强；**HIGH 优先级**。
  - **Candidate 3（Prime Intellect $130M Series A，7月8日）**：**Agent经济柱**——该柱最近一次覆盖为7月11日（Lyzr SivaClaw，Agent 执行 VC 融资流程），角度完全不同（Lyzr：Agent 替代人类高信任流程；Prime Intellect：企业脱离前沿实验室自建 Agent 基础设施）；Nvidia Ventures 领衔投资人名单本身就是 Agent 基础设施层进入主流的信号；与7月12日 Microsoft MAI 替换 OpenAI/Anthropic 的故事形成互补（大企业自建 + 中企业用平台自训，同方向双侧压缩）；Perplexity/Harvey/Cognition 创始人个人背书提供圈层传播力；5天前，在7天窗口内；**HIGH 优先级**。
  - 三者覆盖三个不同主题柱（AI协作实践 / AI产品战略 / Agent经济），时效性均在7天窗口内（2天 / 3天 / 5天），与过去3天已入选/已写作的候选无重叠。
