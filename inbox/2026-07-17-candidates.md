---
date: 2026-07-17
status: pending_selection
---

# Today's Candidates

## Candidate 1: Google Gemini 3.5 Pro 今日上线——从零重建，2百万 token 上下文，Deep Think 锁在 $250/月 Ultra 订阅后面（July 17）

- **Event**: 2026年7月17日（今日），**Google DeepMind** 正式发布 **Gemini 3.5 Pro**——这是 Google 在 5月19日 I/O 大会宣布、原定6月 GA、因"质量精炼"推迟至今的旗舰模型。关键技术决定：Google **完全废弃了 Gemini 3.5 Pro 的原有基础模型**，从头重新预训练，专注数学推理、SVG 生成和长序列推理任务。核心规格：（1）**上下文窗口 2,000,000 token（200万）**——当前前沿模型中最大，是 Claude Opus 4.8（200k token）的10倍；（2）**Deep Think 推理模式**：专为复杂问题分解-分步求解-综合回答而设计，**仅对 $250/月 Ultra 订阅用户开放**；（3）**API 定价**：约 $1.25 / 百万 input token，$10 / 百万 output token（与 GPT-5.5 同级定价）；（4）**自主工作流能力**：可处理含工具调用和代码执行的多步骤任务，最小化人工干预。同一天，WAIC 2026 在上海开幕——Gemini 3.5 Pro 和 Xi Jinping 的 WAIC 主旨演讲选在同一天发布，是 AI 大国竞争叙事的一次有意识的时间碰撞。来源：TechTimes（2026年7月13日，重建确认）、Startup Fortune（架构重建报道）、Memeburn（2M token 上下文报道）、AIToolsRecap（综合规格与定价）、Enterprise DNA（重建 vs DeepSeek V4 竞争分析）。
- **Source**: https://www.techtimes.com/articles/320308/20260713/gemini-35-pro-targets-july-17-after-full-rebuild-every-spec-remains-unconfirmed.htm | https://startupfortune.com/google-delays-gemini-35-pro-launch-to-july-17-after-scrapping-its-base-model/ | https://memeburn.com/gemini-3-5-pro-targets-july-17-with-2m-token-context/ | https://aitoolsrecap.com/Blog/gemini-3-5-pro-july-17-launch-specs-pricing-2026 | https://enterprisedna.co/resources/news/gemini-35-pro-july-17-rebuild-vs-deepseek-v4-2026/
- **Timeliness**: 0天（今日2026年7月17日，Google 正式发布）
- **Topic pillar**: AI协作实践
- **Zico's angle**: 200万 token 是一个阈值，不是一个规格。

  先还原它的尺度。Claude Opus 4.8 当前上下文窗口是20万 token——大约是15万词，相当于一部中等篇幅的小说。200万 token 是20倍：整个代码仓库、完整法律合同库、团队内所有历史 PRD 文档，可以在一个请求里全部塞进去。

  这件事对"如何和 AI 工作"的影响，不是"AI 变聪明了"，是**AI 协作的工作流假设需要重写**。

  过去两年，"有效 prompt 工程"的核心技能是上下文选择——从大量信息里挑选哪些内容给模型，因为上下文是稀缺的。有专门的 RAG 框架、向量数据库、上下文压缩算法来解决这个稀缺性问题。当上下文窗口扩展到200万 token，这些围绕稀缺性构建的基础设施，其战略地位会系统性下移。不是没用，是"选什么给模型"这件事的认知负担变小了。

  取而代之的新技能是**全局上下文思维**：当你可以把整个项目扔给模型时，你怎么提问变得更重要——不是"我应该给它哪些文件"，而是"当它能看到所有文件时，我问的这个问题能拿到什么答案"。视角从"选择什么给 AI"变成了"在 AI 能看到一切的情况下，我问什么"。

  这也是 Google 的战略赌注：**上下文长度是 AI 助手的护城河之一**。OpenAI 在押模型能力（GPT-5.x 系列的推理分数），Anthropic 在押安全性和开发者信任（Claude Code 的贡献率），Google 在押上下文密度——先做到 2M，再看谁能跟上。

  对 Zico 的 co-thinking 实践：过去和 Claude 工作时，我需要把项目背景、框架、已有结论拼凑地传递——现在如果有 Gemini 3.5 Pro 的200万窗口，我可以直接把整个 content-ip repo 的文件树作为上下文传进去。工作流改变不是"功能变了"，是"注意力的分配方式变了"。

- **Resonance hook**: 今天，Google 正式发布 Gemini 3.5 Pro——从零重建，200万 token 上下文（当前前沿最大），Deep Think 推理模式，定价 $1.25/$10 per million token。200万 token 意味着什么：你可以把整个代码仓库、所有历史 PRD、全部设计文档，一次性塞进同一个请求。过去两年我们花时间搞 RAG、向量数据库、上下文压缩，是因为上下文稀缺。当上下文不再稀缺，和 AI 合作的核心技能从"选什么给它"变成了"在它能看到一切的情况下，我怎么问"。
- **Recommended priority**: high

---

## Candidate 2: ZTE Nubia NaviX Ultra 今日在 WAIC 亮相——全球首款 AI Agent 手机，可以不用手指自动用 App，但 WeChat 和支付宝还是封了它（July 17）

- **Event**: 2026年7月17日（今日），**ZTE**（中兴）旗下手机品牌 **Nubia**（努比亚）在上海 **WAIC 2026** 正式发布 **NaviX Ultra**——定位"全球首款 AI Agent 智能手机"（量产旗舰机，非技术展示版）。核心技术：**字节跳动豆包 AI** 运行在操作系统层，通过 **GUI Agent** 读取屏幕内容，自动执行 App 操作——包括打开 App、比价、填写表单、完成购买，全程不需要用户触摸屏幕。产品背景：前代产品 Nubia M153（"豆包手机"一代）在一天内销售 **30,000台**，但随即遭到主流 App 封锁——微信将自动登录标记为可疑行为并强制退出，支付宝和淘宝拒绝配合 AI 操作，钉钉也设有限制。NaviX Ultra 仍面临同样的生态壁垒：**微信正常登录，但 AI 功能尚未开放；阿里巴巴旗下所有 App（淘宝、闲鱼、盒马、高德、灵光）维持对 AI 操作的限制**。Nubia 总裁倪飞在发布会上的问题被媒体总结为："NaviX Ultra 在 WAIC 的问题不是 AI 能不能控制 App，而是 App 生态愿不愿意让它进来。"来源：GSMArena（7月17日，发布现场）、Notebookcheck（NaviX Ultra 发布报告）、BigGo Finance（"第二代豆包手机能否突破生态壁垒"分析）、KuCoin（WAIC 发布公告）、Digitimes（ZTE Nubia vs StepFun AI Agent 手机竞争分析）。
- **Source**: https://www.gsmarena.com/nubia_navix_ultra_unveiled_their_take_onn_aiagent_phone-news-73744.php | https://www.notebookcheck.net/Nubia-unveils-NaviX-Ultra-as-world-s-first-AI-agent-smartphone.1344390.0.html | https://finance.biggo.com/news/ba01fb49-6bb9-4e02-8e2f-73fcda2afb90 | https://www.kucoin.com/news/flash/nubia-to-launch-second-gen-dou-bao-ai-smartphone-at-waic2026 | https://www.digitimes.com/news/a20260709VL218/ai-agent-smartphone-zte-2026.html
- **Timeliness**: 0天（今日2026年7月17日，WAIC 2026 开幕日，NaviX Ultra 现场发布）
- **Topic pillar**: Agent经济
- **Zico's angle**: NaviX Ultra 告诉我们的不是"AI Agent 手机来了"，而是 **Agent 经济卡在了什么地方**。

  先把模型理清楚。Agent 经济的核心假设：AI Agent 能以低成本完成数字世界里的任务（购物、预约、填表、沟通），从而替代人类作为"数字劳动力"。这个假设成立的条件是：Agent 能自由访问任务所需的数字入口——App、网页、表单、API。

  NaviX Ultra 展示了这个假设的断层：**Agent 的能力已经到位了，但数字入口没有开放给它**。豆包 AI 可以读屏幕、操作 GUI、完成任务流；但微信说不，支付宝说不，淘宝说不。中国最核心的数字基础设施——微信支付、阿里系电商、字节系内容——对 Agent 操作保持封锁。

  为什么封？因为这些 App 的护城河恰好建立在**控制用户的操作路径**上。微信的社交关系网络之所以有价值，部分原因是用户必须手动操作——广告曝光、内容消费、社交互动都绑定了人工操作。AI Agent 如果能自动执行"打开微信→发消息→点击链接→完成购买"，整个注意力经济的数据采集逻辑就会断裂。平台封 Agent 不是因为技术障碍，是因为**Agent 威胁了它们的商业模式**。

  这是 Agent 经济里没有被充分讨论的结构问题：**Agent 的软实力是 UI 访问权，而 UI 访问权由平台掌控**。这不是模型能力问题——NaviX Ultra 背后的豆包 AI 已经足够强——是一个生态政治问题。谁能谈判出 Agent 的 App 访问权，谁就控制了 Agent 经济的关键入口。MCP 协议（Anthropic 发布的）正在做这件事，A2A、ARD 在做这件事——NaviX Ultra 的困境，是所有 Agent 经济参与者都面临的困境的硬件具现。

  对 Zico 做 AI 产品的视角：酷家乐的 Agent 集成也面临同样的问题。不是我们的 Agent 不够聪明，是我们 Agent 能操作的数字接口有多少、由谁定义。"Agent 能力"和"Agent 访问权"是两个不同的维度，后者决定前者能干什么。

- **Resonance hook**: 今天，WAIC 2026 上，ZTE Nubia 发布了 NaviX Ultra——它自称"全球首款 AI Agent 手机"。字节豆包 AI 运行在操作系统层，可以读屏、开 App、填表、下单，不需要你动手。听起来完美。但上一代豆包手机卖出 3 万台后，微信封了它的自动登录，支付宝和淘宝拒绝配合，钉钉也不让进。NaviX Ultra 同样面对这个困境：手机已经能用 App，但最重要的 App 不让 AI 用它。Agent 经济的瓶颈从来不是模型能力——是谁有权定义 Agent 能操作哪些数字入口。
- **Recommended priority**: high

---

## Candidate 3: OpenAI 九个月内杀掉两个产品——先关 Sora，再关 Atlas 浏览器，"消灭副业"策略把一切并入 ChatGPT 超级 App（July 9–11）

- **Event**: 2026年7月9日，**TechCrunch** 率先报道：**OpenAI** 宣布将于 **2026年8月9日**关闭 **Atlas**——其于 2025年10月发布的 AI 浏览器，距首发仅9个月。Atlas 的核心设计是把 ChatGPT 嵌入浏览器核心（"agent mode"可自动订票、网购），但面临两个致命问题：（1）**安全漏洞**：易受 prompt injection 攻击，存在暴露用户浏览历史的缺陷；（2）**极慢速度**：Agent 在亚马逊购物车加入3件商品需要10分钟。关闭 Atlas 是 OpenAI 2026年以来第二次关闭独立产品线：此前，**Sora 视频生成工具**于 **2026年4月26日**正式停服——Sora App 关闭，API 将于9月关闭，原因是日均运营成本约 **$100万**，而累计总收入仅约 **$210万**，远未能覆盖成本。Atlas 和 Sora 的关闭均被指向同一内部指令：前应用程序 CEO **Fidji Simo**（已于 2026年宣布转为兼职顾问角色）下达的"**消灭副业（eliminate side quests）**"令。关闭后，Atlas 的 agentic 浏览功能被折叠进：（1）**ChatGPT 桌面 App**（整合 ChatGPT、Codex、Atlas 功能，连接本地文件和企业系统）；（2）**Google Chrome 扩展**；（3）**ChatGPT Work**（7月同期发布，基于 GPT-5.6 模型，通过 MCP 插件连接 Gmail、Google Calendar、Slack、GitHub，支持独立完成复杂多步骤任务）。来源：TechCrunch（2026年7月9日，首发）、The Register（2026年7月10日）、TechTimes（2026年7月11日）、Eastern Herald（2026年7月10日，战略分析）、ValueAddVC（ChatGPT Work + Atlas 关闭综合报道）。
- **Source**: https://techcrunch.com/2026/07/09/openai-is-shutting-down-atlas-but-its-ai-browser-ambitions-are-still-growing/ | https://www.theregister.com/ai-and-ml/2026/07/10/openais-atlas-browser-doesnt-make-it-to-its-first-birthday/5269818 | https://www.techtimes.com/articles/320183/20260711/openai-kills-atlas-browser-after-8-months-what-replaces-it-what-users-must-do-now.htm | https://easternherald.com/2026/07/10/openai-atlas-browser-shutdown-chatgpt-strategy/ | https://valueaddvc.com/pulse/chatgpt-work-enterprise-agent-atlas-shutdown-2026
- **Timeliness**: 6-8天前（TechCrunch 首发 2026年7月9日；The Register / TechTimes / Eastern Herald 7月10-11日跟进）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: OpenAI 九个月关闭两个产品。这个速度本身就是信号。

  先把两次关闭放在一起看：Sora——2024年发布，被认为是 OpenAI 进入视频 AI 的旗帜，1M 次下载，4月关闭，理由是$100万/天运营成本和$210万总收入无法匹配；Atlas——AI 浏览器，2025年10月发布，被认为是浏览器市场的 Trojan Horse，8月关闭，理由是安全漏洞和用户行为研究显示"浏览器是功能，不是目的地"。两个产品关闭后，它们的能力都没有消失——而是**被折叠进 ChatGPT 的平台层**（桌面 App、Chrome 扩展、ChatGPT Work）。

  这不是失败，是战略归因的修正。OpenAI 的判断转变了：**不是"我们需要独立的 AI 产品"，而是"我们需要 ChatGPT 成为平台，其他功能是它的接口"。**

  这个逻辑有一个清晰的历史先例：微软 Office 的演化路径。Word、Excel、PowerPoint 最初是独立产品，逐渐融合进 Office 套件，最后嵌入 Microsoft 365 的 SaaS 平台。用户不是在"用 Excel"，而是在"用 Microsoft 365 的电子表格"。OpenAI 现在在做同样的事：不是"用 Sora"或"用 Atlas"，是"用 ChatGPT 的视频功能"和"用 ChatGPT 的浏览功能"。品牌和用户关系集中于一个平台名称。

  对 Zico 的 AI 产品战略视角：这件事对"如何做 AI 产品"有一个直接的含义。独立的 AI 产品在早期可以作为实验和用户验证的手段，但最终要么成为平台（极少数），要么被平台吸收（大多数）。**如果你是在大公司内部做 AI 产品，决策点不是"这个功能能独立存在吗"，而是"这个功能最终应该并入哪个平台层"。** OpenAI 用关闭 Sora 和 Atlas 回答了这个问题：并入 ChatGPT。

  这件事在组织层面的含义比产品层面更深：**Fidji Simo 的"消灭副业"令是一个组织重心的信号**。AI 公司内部的产品多元化冲动（视频、浏览器、各类垂直工具）在 2026年遇到了一个反力：专注平台、消灭散点、把注意力收回到可以形成飞轮的核心产品上。这不只是 OpenAI 一家的选择——它可能是 AI 时代大公司产品策略的一个样本。

  中文媒体会报"OpenAI 关闭了两个产品"，不会分析：**关闭 Sora 和 Atlas 是 OpenAI 从"产品公司"向"平台公司"转型的组织决策，而不是失败案例——被关闭的产品功能全部保留了，只是失去了独立的产品身份。**

- **Resonance hook**: 7月9日，TechCrunch：OpenAI 将在8月9日关闭 Atlas 浏览器，距发布仅9个月。再往前3个月：4月26日，OpenAI 关闭 Sora。两个产品都没有被彻底杀掉——Sora 的视频能力进了 ChatGPT，Atlas 的浏览 Agent 进了桌面 App 和 Chrome 扩展。产品死了，功能没死，它被并入了平台。这是 OpenAI 内部"消灭副业"指令的最终形态：不是 AI 产品不够好，是独立的 AI 产品不是 OpenAI 想要的组织形式。ChatGPT 不是一个产品，是一个操作系统层——其他功能是它的接口。你怎么看 AI 时代的"平台 vs 产品"这道选择题？
- **Recommended priority**: high

---

## Scan summary

- **Sources scanned**:
  - BuildFastWithAI（2026年7月14-15日，《AI News Today》系列）
  - TechTimes（2026年7月8日，《Gemini 3.5 Pro Targets July 17 as DeepSeek's July 24 Deadline Hits Developers Now》；2026年7月13日，重建确认报道；2026年7月11日，Atlas 关闭细节）
  - Memeburn（《Gemini 3.5 Pro Targets July 17 With 2M Token Context》）
  - Startup Fortune（《Google Delays Gemini 3.5 Pro Launch to July 17 After Scrapping Its Base Model》）
  - AIToolsRecap（《Gemini 3.5 Pro — July 17 Launch Specs Pricing 2026》）
  - Enterprise DNA（《Gemini 3.5 Pro July 17 Rebuild vs DeepSeek V4 2026》）
  - GSMArena（2026年7月17日，《nubia NaviX Ultra unveiled at WAIC》；7月8日，《nubia is launching an AI agent smartphone later this month》）
  - Notebookcheck（《Nubia unveils NaviX Ultra as "world's first AI agent smartphone"》）
  - BigGo Finance（《Second-Generation "Doubao Phone" Set for WAIC Debut: Can ZTE's Nubia and ByteDance Break Through Ecosystem Barriers?》）
  - KuCoin（《Nubia to Launch Second-Generation 'Dou Bao' AI Smartphone at WAIC2026》）
  - Digitimes（2026年7月9日，《China's StepFun, ZTE's Nubia vie for 'world's first AI agent smartphone' at WAIC》）
  - Memeburn（《Nubia AI Agent Smartphone Will Use Apps Without You Touching》）
  - TechCrunch（2026年7月9日，《OpenAI is shutting down Atlas, but its AI browser ambitions are still growing》）
  - The Register（2026年7月10日，《OpenAI's Atlas browser doesn't make it to its first birthday》）
  - Eastern Herald（2026年7月10日，《OpenAI Atlas browser shutdown: ChatGPT strategy》）
  - ValueAddVC（《OpenAI Launches ChatGPT Work, Retires Atlas Browser》）
  - Futurism（《OpenAI Is Shutting Down Its Browser That Was Supposed to Change Everything》）
  - The Decoder（OpenAI Sora 两阶段关闭时间线）
  - OpenAI Help Center（《What to know about the Sora discontinuation》）
  - George Chen Substack（《WAIC 2026 Full Preview》——ZTE Nubia / Huawei Atlas 950 / Xi 主旨演讲）
  - CGTN（2026年7月13日，Xi WAIC 出席公告——已于7月15日候选中覆盖，今日排除重复）
  - Al Jazeera（2026年7月13日，《Hundreds of experts warn the world must prepare now for AI's impact》——FLI 专家预警，无具体产品/公司锚点，排除）
  - Chai Discovery（$400M Series C July 14——AI药物开发，与5个主题柱契合度低，排除）
  - Neko Health $700M Series C——预防医疗，非 AI 内容柱，排除
  - Emergent $130M AI coding Series C——信息不足，无清晰角度，排除
  - SemiAnalysis Claude Code 7% GitHub 提交——已于7月16日候选中覆盖，排除
  - arXiv《Memory in the Loop: In-Process Retrieval as Extended Working Memory for Language Agents》（arXiv 2607.05690, July 8）——技术论文，无时效性企业锚点，与选出的3个候选相比信息差弱，排除
  - arXiv《AI output as representation》（July 13）——哲学框架，无具体事件锚点，排除
  - Claude Sonnet 5 发布（$2/$10 per million token pricing, "July 2026"）——无具体发布日期锚点，排除

- **Total signals found**: 约23个信号评估

- **Why these 3**:
  - **Candidate 1（Gemini 3.5 Pro, 今日 7月17日）**：**AI协作实践柱**——今日发布，0天时效性，本次扫描最高时效性事件之一；7月15日候选中以"事件尚未发生"为由排除，今日正式发布；"从零重建 + 200万 token 上下文"是架构性事件，不是版本迭代；2M token 对 AI 协作工作流的"上下文稀缺假设"构成质变（原先的 RAG/上下文压缩体系面临降级）；与 Zico 的 co-thinking 实践直接共鸣；AI协作实践柱上次入选7月16日（SemiAnalysis Claude Code 7% 贡献），今日角度完全不同（工具视角：7%贡献率 vs 协作范式：2M context 改变提问方式）；**HIGH 优先级**。
  - **Candidate 2（Nubia NaviX Ultra AI Agent 手机，今日 7月17日 WAIC 发布）**：**Agent经济柱**——今日发布，0天时效性；"全球首款量产 AI Agent 手机"是 Agent 经济进入消费硬件层的具体事件；"模型能力已到位，WeChat/支付宝不让用"是当前 Agent 经济核心瓶颈的真实案例——不是能力限制，是访问权政治；前代产品1天卖3万台即被封锁，是可核实的具体数据；中文媒体会报"全球首款 AI Agent 手机"，不会分析"App 生态对 Agent 访问权的封锁是 Agent 经济的结构性瓶颈"；Agent经济柱上次入选7月15日（中国 AI 拟人化新规），今日角度完全不同（监管切割 vs 生态壁垒）；**HIGH 优先级**。
  - **Candidate 3（OpenAI Atlas/Sora 关闭，7月9-11日）**：**组织形式变革柱**——OpenAI 在2026年九个月内关闭两个独立 AI 产品线，将所有能力收归 ChatGPT 平台；"消灭副业"指令是 AI 大公司从产品型向平台型组织转型的信号；Sora 关闭有可核实的财务数据（日均$100万成本 vs $210万总收入）；Atlas 关闭时间在7天窗口边缘（7月9-11日，6-8天前），但跟进报道持续至7月14日；与7月14日的 OpenAI Northslope FDE 收购角度完全不同（外部扩张 vs 内部整合）；组织形式变革柱上次入选7月14日，今日正好是间隔3天的最优时机；中文媒体不会建立"Sora关闭+Atlas关闭=ChatGPT平台化组织转型"的分析框架；**HIGH 优先级**。
  - 三者覆盖三个不同主题柱（AI协作实践 / Agent经济 / 组织形式变革），时效性分别为0天 / 0天 / 6-8天，与过去3天已入选/评估的候选无重叠（深层AI思考柱和AI产品战略柱今日均暂不覆盖，避免连续重复）。
