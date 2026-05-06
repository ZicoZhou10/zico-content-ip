---
date: 2026-05-06
status: written
selected: candidate 2 → drafts/015-default-aesthetic-xhs.md
---

# Today's Candidates

## Candidate 1: 五角大楼签了 8 家 AI 公司的军用合同——Anthropic 是唯一被排除在外的

- **Event**: 2026年5月1日，美国国防部宣布与 OpenAI、Google、Microsoft、Amazon Web Services、Nvidia、SpaceX、Oracle、Reflection 签署协议，将这八家公司的 AI 系统接入军方 IL6/IL7 级别（最高密级）网络，用于任务规划、武器瞄准、情报分析等场景。Anthropic 是唯一被排除在外的主要 AI 公司。背景：国防部长 Pete Hegseth 于2026年2月将 Anthropic 列为"供应链风险"——这是该称号首次用于美国本土科技公司，历史上仅用于外国对手。核心矛盾：五角大楼要求 Anthropic 授权其以"所有合法目的"（all lawful purposes）使用 Claude，包括全自主武器系统和大规模国内监控。Anthropic 拒绝，随即被排除出合同并被列为风险实体。Anthropic 已于3月对特朗普政府提起诉讼，试图推翻该裁定，4月上诉法院维持原判。4月17日，Dario Amodei 与白宫高级官员会面，讨论仍在进行，但5月1日合同签署时 Anthropic 依然缺席。CNBC（5月1日）报道五角大楼科技主管明确表态："Anthropic 仍在黑名单上，Mythos（其网络安全工具）是另一个独立问题。"
- **Source**: https://www.cnn.com/2026/05/01/tech/pentagon-ai-anthropic | https://www.cnbc.com/2026/05/01/pentagon-anthropic-blacklist-mythos-michael.html | https://www.defensenews.com/news/pentagon-congress/2026/05/01/pentagon-freezes-out-anthropic-as-it-signs-deals-with-ai-rivals/ | https://winbuzzer.com/2026/05/03/pentagon-classified-ai-agreements-nvidia-microsoft-aws-google-openai-spacex-oracle-reflection-xcxwbn/ | https://thehill.com/policy/technology/5858995-pentagon-ai-companies-classified-work-deal/
- **Timeliness**: 5 days ago（2026年5月1日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 中文媒体把这件事报道成"Anthropic 被军方排除"然后加一段"AI 安全之争"的背景介绍，就完了。但真正值得想的是：这是 AI 史上第一次"AI 安全"原则被真实市场成本检验的时刻。每家 AI 公司都说自己在乎安全，Anthropic 拒绝签"所有合法目的"条款——结果是失去整个美国政府国防合同市场，被列为"供应链风险"，和华为、中兴一起进入同一个黑名单。同时签了合同的包括：OpenAI（当年以"人类安全"为旗帜创立的公司）、Google、Microsoft、SpaceX（马斯克的公司，他正在同时起诉 OpenAI 背叛安全使命）。"AI 安全"作为企业定位策略的代价，在 5 月 1 日变成了可量化的商业损失。从 AI 产品策略角度有一个清晰的分叉：是选择"所有合法目的"（政府+军方+情报市场全开），还是维持用途限制（企业+消费者市场信任红利）？Anthropic 用实际行动给出了答案——但这个答案有真实成本。对中国 AI 从业者有一个隐性参照：在中国，百度文心、阿里通义、字节豆包会有这种选择的余地吗？答案已经非常清楚。这个问题的存在本身，就说明 AI 作为一种权力结构，和普通软件产品的逻辑是根本不同的。
- **Resonance hook**: Anthropic 是第一家因为拒绝军方"所有合法目的"条款而被美国政府列为供应链风险的美国公司。OpenAI 签了。Google 签了。SpaceX 签了。"AI 安全"这件事，5月1日第一次有了具体的市场价格标签。
- **Recommended priority**: high

---

## Candidate 2: OpenAI 把 ChatGPT 的默认模型换掉了——新标准：更短、更准、去掉多余的 emoji

- **Event**: 2026年5月5日，OpenAI 发布 GPT-5.5 Instant，正式取代 GPT-5.3 Instant 成为 ChatGPT 的默认模型，面向所有用户（包括免费用户）滚动更新。核心改进数据：GPT-5.5 Instant 在高风险提示词（医疗、法律、金融）上的幻觉声明比 GPT-5.3 Instant 减少 52.5%；在用户标记过的高错误率对话中，不准确声明减少 37.3%；平均回复用词减少 30.2%，行数减少 29.2%。新的记忆溯源功能：跨所有模型显示记忆来源，让用户看到每个答案从哪次过去的对话、文件或 Gmail 中获取的信息。API 端以 "chat-latest" 提供 GPT-5.5，GPT-5.3 Instant 对付费用户仍可用三个月后下线。OpenAI 博客原文特别点名了一项变化："fewer gratuitous emojis"（减少多余的 emoji）。TechCrunch（5月5日）、Axios（5月5日）、The Decoder（5月5日）均有详细报道。
- **Source**: https://openai.com/index/gpt-5-5-instant/ | https://techcrunch.com/2026/05/05/openai-releases-gpt-5-5-instant-a-new-default-model-for-chatgpt/ | https://www.axios.com/2026/05/05/openai-chatgpt-update-default-model | https://the-decoder.com/chatgpt-update-rolls-out-gpt-5-5-instant-with-fewer-hallucinations-and-more-personalized-answers/ | https://rollingout.com/2026/05/05/openais-gpt-5-5-instant-reduces/
- **Timeliness**: 1 day ago（2026年5月5日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 中文科技媒体的报道是"ChatGPT 更换默认模型，幻觉减少 52.5%"，然后就是参数对比表格。但有一个更重要的产品信号被忽略了："fewer gratuitous emojis"——这不是技术指标，这是一个产品哲学声明。ChatGPT 过去两年多的默认风格是"高能量、全面覆盖、反应热烈"——大量 emoji、长段落、多维度展开。这种风格被 Karpathy 在一月份预警的"slopacolypse"所批评：AI 生成内容正在用热情掩盖准确性。GPT-5.5 Instant 的方向是反过来的：更短、更准、更冷静。OpenAI 在训练默认模型时，明确选择了"准确" > "印象深刻"。这个选择的影响力远超一次模型更新：ChatGPT 是全球 ~6 亿用户的 AI 使用第一现场，"默认模型"决定了最多人对"AI 应该怎么说话"的预期。当 OpenAI 决定默认模型要更简洁，他们在重新定义大众对 AI 质量的感知标准。这个决定会影响 Google Gemini、Claude、DeepSeek 在产品端的竞争压力方向。一个延伸的产品思考：如果默认模型代表了产品理念，那 OpenAI 正在走向的是"AI 应该更像一个精确的工具"而非"更像一个热情的助理"——这两条路会带来完全不同的产品护城河。
- **Resonance hook**: OpenAI 把 ChatGPT 默认模型换了。新标准里有一条很具体：去掉多余的 emoji。这不是技术更新，这是 OpenAI 对 AI 应该怎么说话给出的最新判断——而这个判断现在是约 6 亿人的默认体验。
- **Recommended priority**: high

---

## Candidate 3: 马斯克在法庭上亲口承认：xAI 蒸馏了 OpenAI 的模型

- **Event**: 2026年4月30日，在加州奥克兰联邦法院 Musk v. Altman 庭审第一周，马斯克在交叉盘问中承认：xAI 的 Grok 模型"部分蒸馏"（partly distills）了 OpenAI 的模型输出。法庭有观众发出倒吸气声。马斯克的辩护是："这是所有实验室现在的标准做法（standard practice），xAI 没有做超出其他所有人的事情。"TechCrunch（4月30日）直接以此为标题报道；MIT Technology Review（5月1日）在第一周综述中以此作为最重要披露之一，标题直接包含"admits that xAI distills OpenAI's models"。背景的结构性讽刺：2026年2月，OpenAI 公开指控中国 AI 公司 DeepSeek 蒸馏其模型输出，措辞强烈，OpenAI CEO Sam Altman 明确将其定性为 IP 问题。Musk 的证词等于在同一个法庭背景下、以同样的行为定性为"标准做法"。当前试验状态：庭审仍在进行，Greg Brockman 于5月5日完成作证（揭示 Musk 在开庭前两天尝试私下和解），预计5月中旬责任认定，法官 Yvonne Gonzalez Rogers 做出最终裁定。
- **Source**: https://techcrunch.com/2026/04/30/elon-musk-testifies-that-xai-trained-grok-on-openai-models/ | https://www.technologyreview.com/2026/05/01/1136800/musk-v-altman-week-1-elon-musk-says-he-was-duped-warns-ai-could-kill-us-all-and-admits-that-xai-distills-openais-models/ | https://www.cnbc.com/2026/05/02/musk-testimony-dominated-first-week-musk-v-altman-trial-in-oakland.html | https://techstartups.com/2026/05/04/elon-musk-admits-xai-distilled-openai-models-as-trial-reveals-last-minute-settlement-push/
- **Timeliness**: 6 days ago（庭审证词：2026年4月30日；MIT 综述：2026年5月1日）
- **Topic pillar**: 深层思考
- **Zico's angle**: 中文媒体会把这件事报道成"马斯克打脸：起诉 OpenAI 同时自己也在用他们的模型"，加一个嘲讽表情包，结束。但这件事有一个比讽刺更深的结构性意义：OpenAI 在2月指控 DeepSeek 蒸馏其模型，语气是"IP 窃取"；马斯克在法庭上把同样的行为称为"所有实验室都在做的标准做法"。这两个陈述不能同时成立——除非"谁在蒸馏谁"的问题本来就没有一个清晰的道德/法律答案。AI 模型蒸馏的本质是：用一个更大、更强的模型的输出作为训练数据，训练出一个更小、更快、更便宜的模型。这和人类学习没有本质区别——我们也是通过消化老师、书本、更优秀的人的"输出"来构建自己的认知。问题在于：人类学习这个过程从来不被叫作"IP 侵权"，但 AI 做相同的事却是法律模糊地带。马斯克的"标准做法"辩护，无意中揭示了整个 AI 行业 IP 结构的根本矛盾：模型权重可以私有化，但从人类集体创作中涌现的"智识模式"——那属于谁？每家 AI 公司建立在之前所有 AI 的肩膀上，也建立在人类数千年写作和思考的肩膀上。在这个链条里主张独家所有权，是一种在认识论上站不住脚的主张。对做 AI 产品的人，这个洞察有一个非常实际的策略含义：真正的护城河不是模型权重，而是数据飞轮、分发能力、和用例锁定——因为模型知识最终都会扩散。
- **Resonance hook**: 马斯克以"OpenAI 背叛使命"为由起诉对方 1300 亿美元。在法庭上，他亲口说 xAI 蒸馏了 OpenAI 的模型。他的辩护是："这是标准做法，所有实验室都在这么做。" 这一句话，把整个 AI 行业的 IP 争议说清楚了。
- **Recommended priority**: medium

---

## Scan summary

- **Sources scanned**: X/Twitter（Karpathy 2026年1月 slopacolypse 预警、2月3日 RSS feeds 推荐；Altman/OpenAI 官方博客；Dario Amodei/白宫会面 4月17日；Jim Fan/NVIDIA 无5月新信号，最新为1月 CES）、GitHub Trending（mattpocock/skills 55k stars、jcode 新代码 Agent 工具包5月3日、Agency-Agents、Langflow/Dify/Flowise 视觉化 Agent 构建器）、Hacker News 2026-05-02至05-04 前页（Musk 庭审第一周、Pentagon AI deals）、OpenAI 官方博客（GPT-5.5 Instant 5月5日；GPT-5.5 4月26日）、Anthropic 官方博客（Claude Opus 4.7 4月16日；Claude Security 公测）、Google DeepMind（Deep Research Max 4月21日；Genesis/DOE 合作；UK £5B 协议）、CNBC/CNN/Defense News/The Hill/Winbuzzer/Orbital Today（Pentagon AI deals 5月1-3日）、TechCrunch/MIT Technology Review/CNBC（Musk xAI 蒸馏 4月30日-5月4日）、arXiv cs.AI（2602.01644 Spatial AI Agents and World Models 2月；2510.16732 World Models for Embodied AI；无5月强锚点新论文）
- **Total signals found**: 16 evaluated
- **Why these 3**:
  - **Candidate 1（Anthropic Pentagon 排除）**：时效5天，CNN/CNBC/Defense News/The Hill 等主流媒体5月1日全覆盖，是 AI 历史上首次 AI 安全原则付出可量化商业成本的具体事件；中文媒体报道了表面事实但无人深入"安全定位的市场代价"框架；组织形式变革柱近7天未出现（4月28日 Candidate 1 是 Musk 庭审开庭，本次角度完全不同）；对比 OpenAI/Google 同时签约的并置构成强共鸣对比。
  - **Candidate 2（GPT-5.5 Instant 默认模型）**：时效最强（1天），OpenAI 官方博客 + TechCrunch + Axios 同日报道；中文媒体停留在参数对比，无人从"OpenAI 在重新定义大众 AI 质量标准"角度分析；"fewer gratuitous emojis"这个具体细节是极强的发现式钩子（可验证）；AI 产品战略柱近7天未使用（4月30日 Candidate 1 是 OpenAI-微软独家结束，角度不同）；GPT-5.5 Instant 与 Karpathy "slopacolypse" 的对话关系构成额外叙事层。
  - **Candidate 3（Musk xAI 蒸馏承认）**：时效6天，TechCrunch 4月30日即发，MIT Tech Review 5月1日综述，CNBC 5月2日确认；中文媒体将聚焦讽刺表层，AI IP 结构性矛盾角度几乎无人写；深层思考柱近7天未使用（4月29日 Candidate 1 是 DeepMind Philosopher，角度不同）；"OpenAI 控诉 DeepSeek 蒸馏 vs. Musk 自认蒸馏"的对比为读者创造可独立验证的认知冲突；与4月28日 draft 009-mission-paradox 使用同一庭审背景，但论点完全不同（非营利结构矛盾 vs. AI IP 认识论矛盾）。

- **Excluded signals**:
  - Karpathy RSS feeds 推荐（2月3日）：90+ 天前，超出任何合理窗口，排除。
  - Karpathy "slopacolypse"（1月26日）：约100天前，超窗口；已作为 Candidate 2 的背景信息使用，不独立成篇，排除。
  - Claude Opus 4.7（4月16日）：20天前，超理想窗口；Claude Design 已在4月29日 Candidate 2 中覆盖相关 Anthropic 产品线发布角度，排除。
  - Google DeepMind Deep Research Max（4月21日）：15天前；已在4月29日 Candidates 扫描中作为评估对象排除，不重复纳入。
  - jcode GitHub trending（5月3日）：信号真实，3天前，但 jcode 为个人开发者项目，知名度有限，可验证锚点弱，且 AI 协作实践柱被4月30日 Candidate 2（Karpathy skills CLAUDE.md）近期使用，排除。
  - Musk 开庭前和解提议（5月4日披露）：作为 Candidate 3 的补充背景信息使用；独立成篇戏剧性不足（谈判细节 < 技术承认的结构性意义），排除独立候选。
  - NVIDIA Jim Fan / GR00T / 空间智能（1月 CES）：无5月新具体事件锚点，最新为1月发布，排除。
  - SpaceX 进入 Pentagon IL6/IL7（5月1日）：与 Candidate 1 同一事件但从 SpaceX 视角切入，角度价值低于 Anthropic 排除叙事，合并入 Candidate 1 背景，排除独立候选。
