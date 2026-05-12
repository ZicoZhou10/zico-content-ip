---
date: 2026-05-12
status: pending_selection
---

# Today's Candidates

## Candidate 1: Google 确认历史首个"AI 写的 exploit"已用于真实网络攻击——比 Anthropic Mythos 发布晚了整整 35 天

- **Event**: 2026年5月11日，Google Threat Intelligence Group（GTIG）发布报告，确认一个知名网络犯罪团伙使用 AI 生成的零日漏洞（zero-day exploit），针对一款广泛使用的开源 Web 系统管理工具，计划发动大规模利用攻击，已被 Google 拦截。**这是 Google 首次确认在真实攻击活动中发现 AI 生成的 zero-day exploit。** 攻击目标是该工具的双因素认证机制，漏洞类型为语义逻辑错误（开发者硬编码了一个与认证执行逻辑矛盾的信任假设）。Google 研究人员识别 AI 参与的证据：exploit 代码含有"教学式 docstrings"、一个被 AI 幻觉出来的 CVSS 评分、以及典型的教科书式 Pythonic 格式——这是 LLM 训练数据风格的典型特征。Google 表示高度确信 AI 被用于漏洞发现和武器化，但不认为使用的是 Anthropic Mythos 或 Google Gemini。Google 在事件被利用前已通知受影响厂商完成修复。背景：Anthropic 在 5月5日 CEO Dario Amodei 明确警告"危险时刻"（moment of danger），同日 Anthropic 推出 Project Glasswing，向亚马逊、苹果、微软、Cisco 等防御端伙伴提供 Mythos 定向访问（2026年4月7日 Mythos Preview 正式发布）；OpenAI 在 5月7日发布 GPT-5.5-Cyber，向特定网络安全团队开放更宽松的安全研究用途。
- **Source**: https://www.bloomberg.com/news/articles/2026-05-11/hackers-used-ai-to-build-zero-day-attack-google-researchers-say | https://www.securityweek.com/google-detects-first-ai-generated-zero-day-exploit/ | https://www.cnbc.com/2026/05/11/google-thwarts-effort-hacker-group-use-ai-mass-exploitation-event.html | https://fortune.com/2026/05/11/google-catches-hackers-cybersecurity-warning-ai-anthropic-mythos/ | https://cyberscoop.com/google-threat-intelligence-group-ai-developed-zero-day-exploit/
- **Timeliness**: 1 day ago（2026年5月11日）
- **Topic pillar**: 深层思考
- **Zico's angle**: 整个"AI 安全"讨论在 5月11日之前，都建立在一个隐含假设上：**防御者先于攻击者掌握 AI 能力**。Anthropic Mythos 的叙事是：Anthropic 先用 AI 发现漏洞，再把修复权给防御端伙伴，攻击者没有这个能力。4月7日 Mythos 发布，5月7日 OpenAI 推出 GPT-5.5-Cyber，5月11日 Google 确认攻击者已经在用 AI 写 zero-day——这个窗口期是 **35 天**。AISI（英国 AI 安全研究所）对 Mythos 的评估、OpenAI 的"受信任访问层"设计、Anthropic 的 Project Glasswing——所有这些治理框架只管约束前沿实验室。犯罪团伙用的是开源权重或越狱 API，不受任何合规要求约束。能力扩散的速度比治理框架的设计速度快。更值得注意的是那个 AI 留下的代码指纹：**幻觉出来的 CVSS 评分**。AI 写了一个攻击脚本，并对自己写的 exploit 打了一个它自己幻觉出来的危险等级评分——既是 AI 能力的证明，也是 AI 理解自己在做什么的上限的证明。这个指纹可能是短期内唯一能用来在归因层面识别 AI 生成攻击代码的信号。对做 AI 产品的人，这个事件有一个直接的产品安全含义：如果 AI 降低了 zero-day 发现的边际成本，每一个有 API 或 Web 界面的产品，就是在一个攻击成本更低的世界里运行。
- **Resonance hook**: 2026年4月7日，Anthropic 发布 Mythos，用 AI 替防御者找零日漏洞。5月11日，Google 确认：一个犯罪团伙已经在用 AI 生成 zero-day exploit，差点发动大规模攻击。防御端 AI 领先攻击端的窗口期：35 天。AI 写的攻击代码有一个独特指纹——exploit 脚本里含有一个它幻觉出来的 CVSS 评分。
- **Recommended priority**: high

---

## Candidate 2: Karpathy 说"大多数 AI 应用都是模型局限性的临时包装"——Software 3.0 给产品存活率打了一个测试

- **Event**: 2026年4月30日，Andrej Karpathy 在个人博客（karpathy.bearblog.dev）发布其在 Sequoia AI Ascent 2026（4月20日，旧金山）炉边对话的摘要，并于 **2026年5月9日更新**，同步在 X（@karpathy，tweet 2049903821095354523）推送。出席者包括 Demis Hassabis、Greg Brockman、Boris Cherny（Anthropic）、Jim Fan（NVIDIA）、Dmitri Dolgov（Waymo）。核心论点：**① "A lot of AI apps are temporary wrappers around model limitations. As models get better, entire product categories collapse into a prompt."**（大多数 AI 应用是模型局限性的临时包装，随着模型能力提升，整个产品品类会坍缩成一个 prompt）；② 提出 **Software 3.0** 框架：Software 1.0 是显式规则，Software 2.0 是学习权重，Software 3.0 是通过 prompt、context、agent、工具、记忆和验证来编程——context window 成为新的编程界面；③ "Vibe coding"已过时，进入 **Agentic Engineering** 时代：最好的工程师不是写每一行代码的人，而是能在不让质量崩塌的前提下指挥 Agent 的人；④ LLM 不只是"加速现有事物"，举例：menugen（LLM 可以给定菜单直接生成完整 Web App，UI 层被整个吸收）。Sequoia 合伙人 Sonya Huang 在同场发言中宣布"2026 年是 Agent 之年"，并描述已经到来的长链路 Agent 可恢复错误、持续运行的能力。
- **Source**: https://karpathy.bearblog.dev/sequoia-ascent-2026/ | https://x.com/karpathy/status/2049903821095354523 | https://sequoiacap.com/article/ai-ascent-2026/ | https://www.theaiopportunities.com/p/sequoia-ai-ascent-2026-andrej-karpathy | https://analyticsdrift.com/andrej-karpathy-agentic-engineering-software-3/
- **Timeliness**: 3 days ago（博客 5月9日更新；fireside chat 原发于 4月20日，博客初发 4月30日，超7天但在30天窗口内）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: "临时包装"这个词是过去一年 AI 产品讨论里说得最重要的一句话之一。但中文报道把它读成了"Karpathy 说 AI 产品快被淘汰了"——这个读法错过了真正有用的部分。Karpathy 不是在预言灭亡，他是在给出一个**产品存活率测试**：你的产品，是因为模型做不到某件事才存在的，还是因为模型能做到这件事而变得更有价值的？只有第二种产品能在模型持续迭代的环境里活下去。具体来说，能通过"包装测试"的产品形态只有三种：**① 网络效应产品**——价值来自其他用户的存在，不来自模型质量（Duolingo 的语言伙伴网络、GitHub 的 contributor graph）；**② 数据飞轮产品**——产品使用本身产生训练数据，数据改善模型，模型改善产品（每一次用户纠错都是训练信号）；**③ 品类创造产品**——创造了在 AI 之前不存在的体验，不是把旧事物做得更快，是让新事物变为可能（menugen 的逻辑：不是"更快做网站"，是"对话即网站"）。测试方法是一个问题：**如果 GPT-6 或 Claude 5 明天发布，用户能不能通过直接和新模型对话完成你产品的核心价值？** 如果答案是"能"，你是临时包装。如果答案是"不能，因为（用户网络/历史数据/新型交互范式）不在模型里"，你有真实护城河。
- **Resonance hook**: Karpathy 在 Sequoia 炉边对话说了一句话，现在在硅谷 AI 产品圈被反复引用："大多数 AI 应用都是模型局限性的临时包装，随着模型改进，整个产品品类会坍缩成一个 prompt。" 他的意思不是警告，是提供了一个测试：如果 GPT-6 明天发布，用户直接和它说话就能完成你的产品的核心价值——你就是临时包装。
- **Recommended priority**: high

---

## Candidate 3: Alphabet 市值 $4.8 万亿，超越 Nvidia——市场在给"拥有完整 AI 栈"定价

- **Event**: 2026年5月10日，CNBC 报道 Alphabet 过去12个月股价累计涨幅达 **160%**，市值达 **$4.8 万亿**，盘后曾短暂超越 Nvidia（$5.2 万亿），位列全球市值第二。Fortune（5月10日）、NAI 500（5月11日）同日报道：Alphabet 正逼近成为全球市值最大公司。核心归因：Deepwater 资产管理公司合伙人 Gene Munster："**Google 是定位最好的两家 AI 公司之一，因为他们拥有栈的大部分——芯片、模型、基础设施和分发。**"（"Google is one of the two best-positioned AI companies because they own most of the stack. Chips, models, infrastructure and distribution."）具体财务数据：① 2026年 Google Cloud 积压订单（backlog）较去年同期**近乎翻倍至 4620 亿美元**；② JPMorgan 分析师将 Google 列为科技板块"整体首选"，指向加速增长和云积压爆发；③ Alphabet 2026年预计资本支出高达 **$1900 亿**，是 2025年的两倍多；④ Anthropic 对 Google Cloud 的承诺（据报道高达 $2000 亿）可能占 Alphabet 未来合约云营收的 **40%+**。背景：同期 OpenAI 正在为新合资企业（The Development Company）以 $100 亿估值募集 $40 亿，Anthropic 估值讨论已触及 $9000 亿（VentureBeat 5月8日）。Sequoia AI Ascent 2026（4月20日）估计 AI 可触达的服务业市场规模为 **$10 万亿**。
- **Source**: https://www.cnbc.com/2026/05/10/alphabet-160percent-rally-in-year-reflects-value-of-owning-most-of-ai-stack.html | https://fortune.com/2026/05/10/ai-alphabet-stock-market-capitalization-nvidia-google-gemini/ | https://nai500.com/blog/2026/05/alphabets-rally-nears-worlds-largest-company-amid-ai-frenzy-bubble-warnings/
- **Timeliness**: 2 days ago（2026年5月10日）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 中文科技媒体把这个消息报道成"Google 股价大涨，市值逼近全球第一"，然后给出一张和 Nvidia/苹果/微软的市值对比图，结束。但 $4.8 万亿这个数字里埋着一个 AI 竞争结构的判断，被完全忽略了：**市场在给"谁拥有 Agent 经济的基础设施"定价，而不是给"谁有最好的模型"定价**。在 Agent 经济里，AI Agent 会消耗算力（Google TPU）、调用模型推理（Gemini）、部署在云上（Google Cloud）、并通过分发渠道触达用户（Android、Search、YouTube、Chrome）。Google 在这四层都有资产。Anthropic 的年化营收增长80倍、需要海量算力、付钱给 Google；Microsoft/Azure 是 OpenAI 的算力和分发渠道。前沿模型公司的增长越快，他们就越依赖 Google 和 Microsoft 的基础设施。这创造了一种反直觉的结构：**在 Agent 经济里，基础设施供应商是竞争对手最好的客户，也是市场里最重要的受益者之一**。Anthropic 付给 Google 的 $2000 亿可能占 Google Cloud 合同积压的 40%——这意味着 Claude 的每一个 API 调用都在给 Google 的 $4.8 万亿估值做贡献。对做 Agent 产品的人，这个结构有一个直接的战略含义：你的产品建立在谁的栈上，就意味着在规模化时你的边际成本流向谁。选择基础设施不只是技术决策——是决定谁会在你增长时跟你分走增长红利的商业决策。
- **Resonance hook**: Gene Munster（Deepwater）上周说了一句话：Google 是定位最好的 AI 公司之一，因为"他们拥有 AI 栈的大部分——芯片、模型、基础设施和分发"。市场的反应：Alphabet 过去12个月涨了160%，市值 $4.8 万亿，盘后短暂超越 Nvidia。最反直觉的细节：Anthropic 付给 Google 的钱可能占 Google Cloud 合同积压的 40%——Claude 增长越快，Google 赚得越多。
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**: X/Twitter（Karpathy：4月30日博客 + 5月9日更新，X thread 2049903821095354523；Altman/OpenAI：GPT-5.5-Cyber 5月7日，ChatGPT Gmail memory 5月9日——均已在 5月8日/5月11日 candidates 覆盖；Jim Fan/NVIDIA：DreamDojo/Physical AI 无5月9-12日独立新锚点；LeCun 无7天内新信号；Demis Hassabis 无5月9-12日新信号；Swyx 无独立新信号；Nat Friedman 无独立新信号）、GitHub Trending（Week 19：ChromeDevTools/chrome-devtools-mcp 于5月11日在 AIToolly 出现，但官方发布时间为 2025年9月，非新事件；addyosmani/agent-skills 已在5月11日 candidates 覆盖）、HN 前页（5月11日：Google AI zero-day 多家媒体同日覆盖，进入 HN 前页）、Google GTIG Report（5月11日：首个 AI 生成 zero-day exploit 确认报告）、Bloomberg/SecurityWeek/CNBC/Fortune/The Register/CyberScoop（5月11日 Google AI zero-day 多媒体同日覆盖）、Anthropic 官方博客（5月5日 Finance Agents——已在5月7日 candidates 覆盖；5月6日 Colossus——已在5月11日 candidates 覆盖）、OpenAI 官方（5月7日 GPT-5.5-Cyber——独立新信号，未在近期 candidates 直接覆盖）、CNBC/Fortune（5月10日 Alphabet 160% rally / "own the stack"）、Sequoia Capital AI Ascent 2026（4月20日活动；karpathy.bearblog.dev 4月30日发布/5月9日更新）、arXiv cs.AI/cs.CV（5月最新列表：无5月9日后强时效新论文锚点）、Google I/O 2026 预告（5月19日大会；The Android Show I/O Edition 5月12日直播，发布前无可用具体锚点）
- **Total signals found**: 21 evaluated
- **Why these 3**:
  - **Candidate 1（Google AI zero-day）**：时效最强（1天，5月11日），Bloomberg/SecurityWeek/CNBC/Fortune/CyberScoop 同日多媒体确认；"历史首次确认在真实攻击中使用 AI 生成 zero-day"是不可替代的事件锚点；AI 代码指纹（幻觉 CVSS 评分）是可独立验证的精确细节，创造发现式钩子；深层思考柱：5月11日 candidates 已用（xAI neocloud），但角度完全不同（那篇是商业结构分析，这篇是 AI 双重使用的实证转折点）；"防御者领先35天后失去先机"这个叙事在中文媒体零覆盖——国内报道停留在"黑客用 AI 攻击"的标题层。
  - **Candidate 2（Karpathy 临时包装）**：博客 5月9日更新（3天前），在30天可接受窗口内；"大多数 AI 应用都是临时包装"是过去两周英文 AI 圈被引用最高的单句话之一；AI 产品战略柱：5月11日 candidates Candidate 1 是"ChatGPT 记忆层护城河"（产品如何建立护城河），本篇是"产品护城河的存活率测试框架"（不同维度）；"包装测试"（GPT-6 发布后你还存在吗？）是中文 AI 产品圈几乎没有人用这个精确框架讨论过的议题；Zico 的 3D+AI 一线产品经验使"menugen" 类的品类创造案例有真实共鸣。
  - **Candidate 3（Alphabet $4.8T 栈所有权）**：时效2天（5月10日），CNBC + Fortune + NAI 500 同日覆盖；Agent 经济柱：近7天 candidates 未使用；"拥有栈 vs 拥有最好模型"的竞争框架是5月10日最强的 AI 战略信号；Anthropic 付给 Google 40%+ 云积压这一细节（援引具体数字 $2000亿/$4620亿）是可独立验证的结构性证据；中文媒体停留在市值对比图层面，无人从"谁在 Agent 经济里收过路费"切入；Sequoia AI Ascent $10 万亿可寻址服务市场作为背景锚点强化 Agent 经济叙事。

---

**Excluded signals**:
- OpenAI GPT-5.5-Cyber 发布（5月7日）：时效5天，CNBC/Axios/Help Net Security 覆盖；角度与 Anthropic Mythos（5月6日 xAI candidates 背景）和 Google AI zero-day 高度重叠——三者同属"AI 网络安全双重使用"主题，今日选择 Google zero-day（时效最强 + 最具叙事转折价值），排除 GPT-5.5-Cyber 作为独立候选
- Chrome DevTools MCP（AIToolly 5月11日文章）：官方发布时间为 2025年9月，不符合7天时效要求；AIToolly 文章是回顾性介绍而非新发布，排除
- Anthropic Finance Agents 十大模板（5月5日）：已在5月7日 candidates 完整覆盖，排除
- Anthropic Managed Agents "dreaming" 功能（5月5日发布背景中提及）：与 Finance Agents 公告同日，已在5月7日 candidates 覆盖范围内，且无独立可验证发布日期确认，排除
- Google The Android Show I/O Edition（5月12日今日直播）：活动在今日 1PM ET 进行，发布前无具体可用事件锚点，候选等待 I/O 2026（5月19日）主会场实际发布内容
- Karpathy "stopped using AI to write code / second brain"（4月3日）：38天前，超30天窗口，排除
- McKinsey "93.2% cite cultural challenges" AI adoption（2026调查）：无具体5月内发布日期确认；角度（组织文化vs技术障碍）价值中等，但缺乏精确时效锚点，排除
- Sequoia AI Ascent "2026 年是 Agent 之年"（4月20日活动本身）：22天前，Karpathy 博客摘要（Candidate 2）已覆盖同一信号源，排除作为独立候选
- Trump 行政团队 AI 模型测试协议（Google/Microsoft/xAI，5月5日）：政策信号，Zico 受众（AI 产品经理、创业者）直接相关性较低；中文媒体已大量覆盖，信息差有限，排除
