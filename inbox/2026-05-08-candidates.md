---
date: 2026-05-08
status: written
selected: candidate 2 → drafts/016-endpoint-optimism-trap-xhs.md
---

# Today's Candidates

## Candidate 1: OpenAI 发布三款语音新模型——GPT-Realtime-2 把 GPT-5 级别推理搬进了实时对话

- **Event**: 2026年5月7日，OpenAI 在官方博客发布三款全新实时语音模型，即日起向 API 开发者开放。① **GPT-Realtime-2**：OpenAI 首个搭载 GPT-5 级别推理能力的语音模型，上下文窗口从 32K 扩展至 **128K tokens（4 倍增长）**，支持五档推理强度：minimal / low（默认）/ medium / high / xhigh，开发者可按应用场景在速度和准确度之间自由调校；在 Big Bench Audio 音频智能评测上比上一代 GPT-Realtime-1.5 高 **15.2%**，Instruction Following 评测（Audio MultiChallenge）高 13.8%；② **GPT-Realtime-Translate**：实时语音翻译，支持 **70+ 种输入语言翻译成 13 种输出语言**，$0.034/分钟；③ **GPT-Realtime-Whisper**：流式语音转文字，$0.017/分钟。GPT-Realtime-2 定价 $32/M 音频输入 token、$64/M 音频输出 token。OpenAI 官方博客原文标题：《Advancing voice intelligence with new models in the API》，TechCrunch、Neowin、9to5Mac 等同日报道。
- **Source**: https://openai.com/index/advancing-voice-intelligence-with-new-models-in-the-api/ | https://techcrunch.com/2026/05/07/openai-launches-new-voice-intelligence-features-in-its-api/ | https://www.neowin.net/news/openai-unveils-trio-of-realtime-audio-models-to-power-next-gen-voice-agents/
- **Timeliness**: 1 day ago（2026年5月7日）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 中文科技媒体把这件事报道成"OpenAI 语音模型更新，支持多语言翻译"，然后给出价格表，结束。但有一个 API 设计细节被完全忽略：**五档推理强度（minimal → xhigh）**。这不是技术参数，这是一个产品架构声明。在文字模型里，推理能力和回复速度从来是绑定的——更聪明的模型总是更慢。GPT-Realtime-2 把这两个维度分开了：同一个模型，同一套权重，开发者选择"思多少"。这意味着语音 Agent 的产品设计获得了一个全新维度。以前的选择是"用哪个模型"，现在是"这个场景需要多深的思考"。举例：一个银行客服语音 Agent，处理"请查询我的余额"时用 minimal（毫秒级响应），处理"帮我分析我的消费结构，推荐储蓄方案"时用 xhigh（GPT-5 级别推理，慢一点但精确）。同一个 Agent，动态调整推理深度。更深一层：128K 上下文是语音 Agent 生产化的临界点。32K tokens 对应约 25 分钟的语音转录，适合短对话；128K 约 100 分钟，覆盖完整的咨询、诊断、谈判会话。这两个数字加在一起——**推理可调 + 100 分钟记忆**——意味着语音 Agent 第一次可以胜任企业级工作流场景，不再只能处理简单问答。从产品战略角度，这是 OpenAI 对语音作为第三个 Agent 部署通道的正式押注：文字 UI（ChatGPT）、API（编程接口）、语音（无界面的实时交互）。语音是唯一一个可以在用户不打开任何 App 的情况下运行 Agent 的通道。
- **Resonance hook**: OpenAI 给语音模型加了一个"思考深度调节旋钮"：开发者可以选择 minimal（快，浅）到 xhigh（GPT-5 级推理，慢，精）。同一个 Voice Agent，处理不同任务时思考深度不同。这看起来是 API 细节。实际上是语音 Agent 第一次可以胜任复杂企业任务的标志——上下文窗口同时扩大到 128K（约 100 分钟语音）。
- **Recommended priority**: high

---

## Candidate 2: a16z 说"AI 抢走工作"是"完全的幻觉"——同一周 Dario 刚刚用同一个经济学框架为自己的警告辩护

- **Event**: 2026年5月7日，Andreessen Horowitz 普通合伙人 David George 在 a16z 官网发表长篇文章《The "AI Job Apocalypse" Is a Complete Fantasy》，Fortune 同日以《AI 末日论是"无用的营销、糟糕的经济学和更糟糕的历史学"》为题转载报道。核心论点：① **四项大规模调查显示 >90% 的企业报告 AI 对就业没有影响**（近三年数据）；② 援引 **Jevons 悖论**：当一种重要投入品价格下降，经济体不会"坐在那里不动"，它会做更多事——"化石燃料让能源变便宜时，我们不只是让鲸鱼捕手和伐木工失业；我们发明了塑料！"；③ **电子表格案例**：电子表格被普遍认为会淘汰簿记员，美国确实失去了约 100 万个簿记员岗位，但同期新增了约 150 万个财务分析师岗位；④ 历史正在重演：农业机械化消灭了美国 20 世纪初 1/3 的就业，但这些工人最终流向了工厂、办公室、医院，后来又流向了软件行业。背景：① 2026年1月，Anthropic CEO Dario Amodei 公开警告 AI 可能造成白领就业的"异常痛苦的"冲击；② 2026年5月5日（三天前），Amodei 在 Anthropic 华尔街发布会上与摩根大通 CEO Jamie Dimon 同台，**主动援引 Jevons 悖论为自己的立场辩护**；③ 今天（5月7日）a16z 同样援引 Jevons 悖论，结论却是"从来就不是问题"。Hacker News 讨论帖 #48046157 同日进入前页。
- **Source**: https://a16z.com/the-ai-job-apocalypse-is-a-complete-fantasy/ | https://fortune.com/2026/05/07/ai-job-apocalypse-unhelpful-marketing-bad-economics-worse-history/ | https://news.ycombinator.com/item?id=48046157
- **Timeliness**: 1 day ago（2026年5月7日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 中文媒体会把这件事报道成"VC 说 AI 不会抢工作"，然后配一张情绪化的标题图，结束。但有一个叙事层被完全忽略：**同一周里，同样的 Jevons 悖论，同时出现在悲观阵营和乐观阵营的口中**。Dario Amodei 在1月警告"异常痛苦"，在5月5日用 Jevons 悖论为"最终会好"辩护，在同一场发布会上立刻补充"AI 比历史上所有技术移动更快，过快的压力可能带来奇怪的行为和大规模混乱"。David George 在5月7日用同一个 Jevons 悖论说"从来就不是问题"。两个人，同一框架，结论截然不同。这说明什么？Jevons 悖论是对的：**宏观终态可能没问题**。分歧只在一个维度：**过渡速度**。如果过渡在20年内发生，历史上每次技术革命都吸收了；如果在3年内发生，没有任何社会缓冲机制能运转这么快。Amodei 的自相矛盾其实不是矛盾，是一个精确的陈述：他说的是"宏观 Jevons 我信，微观过渡速度我不信"。a16z 的回应是回避了速度问题，只讲了宏观终态。对做 AI 产品的人，这个争论有一个非常直接的产品含义：**你产品能否解决"过渡期间的人"的痛点，比解决"终态问题"更有市场**。Duolingo 不是在"解决语言学习这个永恒问题"，它在解决"我现在想学西班牙语但不知道从哪开始"的过渡期需求。AI 最有价值的产品窗口，是那些让"被替代的人"重新上车的工具，而不是那些替代他们的工具。
- **Resonance hook**: 2026年1月，Dario Amodei 警告 AI 将造成白领就业的"异常痛苦"冲击。5月5日，他在华尔街发布会上援引 Jevons 悖论说"自动化会创造更多需求"。5月7日，a16z 合伙人用同一个 Jevons 悖论说整件事从来就是"完全的幻觉"。两边用一个经济框架，两种结论。真正的分歧不是"会不会"——是"多快"。
- **Recommended priority**: high

---

## Candidate 3: Demis Hassabis 在 YC 说他 50/50 认为 AGI 可以被解决——他点名了一个具体障碍

- **Event**: 2026年4月29日，Google DeepMind CEO Demis Hassabis 在 Y Combinator × Google DeepMind Startups Day 上与 YC CEO Garry Tan 进行炉边对话，发表若干针对 AGI 的罕见具体判断。核心内容：① **"现有基础上，可能还差一两件事"**——Hassabis 认为当前最强 AI 系统已经具备了很多 AGI 所需要的能力，剩余差距是有限的而非无限的；② **"持续学习这个问题还没被解决"**（"Continuous learning has not been cracked yet"）——当前模型无法在部署后从真实体验中持续更新自身权重，每一个 Agent 跑的都是"冻结的大脑"；③ **"这些剩余问题能否被解决，我的判断是 50/50"**——这是 Hassabis 首次公开给出概率估计；④ **"AGI 可能在五年内到来"**；⑤ **"Agent 才刚刚开始"**（"Agents are just getting started"）。PANews 中文报道标题为《DeepMind 创始人到访 YC：AGI 只差一两块拼图；Agents 才刚刚起步》。背景：Hassabis 曾在 Davos 与 LeCun 就 AGI 路径展开争论（1月），此次 YC 对话是 Hassabis 今年最具体的 AGI 技术判断。距离 Google I/O 2026 大会（5月19日）还有 11 天。
- **Source**: https://events.ycombinator.com/gdm-startupday | https://www.panewslab.com/en/articles/019dde05-2a76-7628-955f-3976151af4d5 | https://www.startuphub.ai/ai-news/artificial-intelligence/2026/demis-hassabis-on-ai-s-future-beyond-current-models
- **Timeliness**: 9 days ago（2026年4月29日；略超7天窗口，30天内可接受；Google I/O 距今11天使内容时间价值高于均值）
- **Topic pillar**: 深层思考
- **Zico's angle**: 中文媒体把这件事报道成"DeepMind CEO 说 AGI 五年内到来"，然后加一段时间线对比表（各家 AGI 预测），结束。但 Hassabis 这次表态里最重要的信号被截掉了：**他是前沿实验室 CEO 里唯一一个公开说"我 50/50 不确定这些技术问题能否被解决"的人**。Altman 说"快了"，LeCun 说"现路径到不了 AGI"，Dario 说"50% 概率在我们有生之年"，马斯克说"不到两年"。Hassabis 说的是：方向对了，但有一个具体问题——持续学习——还没解决，而且我不确定它能不能被解决。这种"具体命名障碍 + 给出不确定概率"的表述，是一种非常稀有的认识论精确性，在以吹牛为生的 AI 行业里尤其罕见。更重要的是他命名的这个障碍：**持续学习**。现在所有的 AI Agent——包括 Claude、GPT-5.5、Gemini——跑的都是"冻结的大脑"。它们在部署之后学不到任何新东西。所有的"改进"都必须通过重新训练、RAG、或者 prompt 工程来实现。用一个不那么精确但更容易感知的类比：你雇了一个员工，他在入职第一天读完了所有的手册，然后，他的大脑就永远停在那一天了。他可以用记忆回答任何在入职那天已知的问题，但他无法从真实工作经历中学习。这是所有 Agent 今天共同的上限。Hassabis 说：我们不确定这个上限能否被打破。对做 AI 产品的人，这个洞察有一个直接的策略含义：**在持续学习被解决之前，Agent 的价值护城河必须建立在"数据飞轮 + 人类反馈回路"上，而不是"自我学习"上**。那些声称自己的 Agent 会"越用越聪明"的产品，多半在说的是 RAG 或 fine-tune 的变体，不是真正的持续学习。
- **Resonance hook**: Demis Hassabis 上周在 YC 说：距离 AGI 可能只差"一两件事"，但他给解决这些问题的概率打了 50/50。他说的那一两件事里，有一件是"持续学习"——当前所有 AI 模型在部署后都无法从实际体验中更新自己。每个你今天用的 AI Agent，都在用一个冻结在训练截止日的大脑工作。Hassabis 说他不确定这能改变。
- **Recommended priority**: medium（时效9天，略超窗口；但深层思考柱近日未用，Google I/O 前11天的时间节点使 Hassabis 的表态具有额外的信息价值）

---

## Scan summary

- **Sources scanned**: X/Twitter（Karpathy 无5月7-8日独立新信号；Altman/OpenAI 官方博客 May 7 发布 GPT-Realtime-2；Dario Amodei：May 5 Wall Street 发布会发现 Jevons 悖论切入作为 Candidate 2 背景；Jim Fan 无 May 5-8 新事件锚点；LeCun 无7天内新信号；Demis Hassabis：April 29 YC fireside chat；Swyx 无7天内独立信号；Nat Friedman 无7天内独立信号）、GitHub Trending（Week 18 May 2026：InsForge、OpenClaw 继续增长、Local Deep Research；无单点爆发式新项目）、HN 前页（OpenAI GPT-Realtime-2 上榜；a16z AI job essay #48046157 进入前页）、OpenAI 官方博客（GPT-Realtime-2 May 7；ChatGPT for Excel/Google Sheets GA May 5，与 May 7 candidates Anthropic/Microsoft 365 主题高度重叠排除）、Anthropic 官方（无 May 5-8 新独立发布；May 5 Wall Street 发布会已在 May 7 candidates 覆盖）、DeepMind/Google（Gemini 3.1 Flash-Lite 发布：$0.25/M token，2.5× 速度提升；Google I/O May 19 预告期；Hassabis YC April 29）、a16z（David George "AI Job Apocalypse" essay May 7）、arXiv cs.AI/cs.CV（XPENG X-World April 29技术报告，9天前，时效弱；HY-World 2.0 Tencent April 16，22天前，超7天窗口；2604.14268 arXiv提交时间为4月）、CNBC/Fortune/9to5Mac/Neowin/TechCrunch（OpenAI voice models May 7 多媒体同日覆盖）
- **Total signals found**: 19 evaluated
- **Why these 3**:
  - **Candidate 1（OpenAI GPT-Realtime-2）**：时效最强（1天），OpenAI 官方博客 + TechCrunch + Neowin + 9to5Mac + The New Stack 同日多媒体覆盖；中文媒体停留在"支持多语言翻译"的功能层，无人从"推理可调 + 128K 上下文 = 语音 Agent 产品化临界点"切入；AI 产品战略柱：May 7 已用 Anthropic Wall Street（垂直金融模板），本篇是 OpenAI 语音 Agent 战略，公司不同、技术层不同、切入完全不同；五档推理强度 API 是发现式钩子——开发者可自己在 OpenAI playground 验证，创造自我传播验证行为；语音作为第三 Agent 部署通道的框架在中文圈几乎零覆盖。
  - **Candidate 2（a16z AI Job Apocalypse）**：时效1天（May 7），Fortune/HN 同日覆盖；Jevons 悖论出现在同一周三个不同声音（Amodei警告→Amodei辩护→a16z反驳）形成独特叙事张力；组织形式变革柱：May 7 已用 OpenAI DeployCo（AI 公司组织形态），本篇是"AI 与工作的宏观经济框架"，方向完全不同；"过渡速度是真正分歧"这个切入点中文媒体零覆盖；产品含义（解决过渡期人的需求 > 解决终态问题）对 Zico 受众直接相关；电子表格案例（-100万簿记员 → +150万财务分析师）是可独立验证的历史数据锚点，强信息增量。
  - **Candidate 3（Demis Hassabis YC × DeepMind）**：时效9天（April 29），略超7天理想窗口但在30天可接受范围内；"50/50 概率"是 Hassabis 公开发言中首次可量化的不确定性表述，极具信息增量；深层思考柱：May 7 candidates 未使用；Google I/O 前11天的时间窗口使 Hassabis 的判断具有额外的信息价值（I/O 公告后中文媒体会报道 Google AI 产品，先发 Hassabis 对 AGI 局限性的坦诚判断形成对比）；"持续学习 = 冻结的大脑"类比对 Agent 产品开发者有直接策略含义。

- **Excluded signals**:
  - Google Remy（May 6）：May 7 candidates Candidate 3 已完整覆盖，排除
  - Anthropic Wall Street 发布会（May 5）：May 7 candidates Candidate 2 已完整覆盖，排除
  - OpenAI DeployCo / 17.5% 保底（May 4）：May 7 candidates Candidate 1 已完整覆盖，排除
  - ChatGPT for Excel/Google Sheets GA（May 5）：与 May 7 candidates 的 Anthropic/Microsoft 365 主题高度重叠（两者都是 AI 接管 Excel），排除
  - Gemini 3.1 Flash-Lite（发布日期不明确）：无精确 May 5-8 事件锚点确认，且为 Google I/O 前低调发布，中文圈已有覆盖，无 Zico 独特角度，排除
  - XPENG X-World 技术报告（April 29）：时效9天，与 Candidate 3 Hassabis（同日）竞争同一时效窗口，但 Hassabis 在深层思考柱的信息增量远高于 XPENG 在空间智能柱的信息增量；XPENG 中文媒体覆盖已饱和（国内自动驾驶媒体全覆盖），排除
  - Tencent HY-World 2.0（April 16-17）：22天前，超7天理想窗口；国内媒体已大量覆盖，信息差极小，排除
  - Oracle 裁员 30000 人（March 31）：38天前，超出30天窗口，排除
  - Novo Nordisk + OpenAI（April 14）：24天前，超7天窗口，且中文科技媒体已有报道，信息差有限，排除
  - IBM Think 2026 发布会（May 2026）：IBM 与 Zico 受众（AI 产品经理、创业者、中国大厂从业者）相关性低；IBM Bob 等产品无强 Zico 视角切入点，排除
  - Dario Amodei Jevons 悖论表态（May 5 Wall Street 发布会）：已作为 Candidate 2 的叙事背景使用；May 7 candidates Candidate 2 已深度覆盖 Anthropic 金融 AI 战略，本次以不同视角（a16z 反驳）切入同一话题流，不独立成篇，排除
