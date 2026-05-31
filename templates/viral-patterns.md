# Viral Patterns Log

**用途**：每周扫描 X 与小红书上"AI / Agent / 创业"赛道的爆款，提取**结构性模式**（不是内容总结），沉淀成 Daily Write 可读的 few-shot 示例库。

**方法论**：只看结构，不看话题。每条样本提取 5 个字段：
1. **钩子类型**（开头哪种形式抓住注意力）
2. **Complication 句型**（第二段怎么把冲突点摆出来）
3. **中段推进逻辑**（单线推进 / 并列对比 / 反问递进）
4. **收尾形态**（金句 / 真问题 / 召唤）
5. **可复用的句式模板**

**采样原则（更新 2026-04-28）**：不只看头部 KOL。**作者粉丝数 ≤ 50K 但单帖互动 ≥ 5K 的"outlier 爆款"才是最高信号**——头部 KOL 的爆款大部分靠粉丝基数，结构信号被噪声淹没；中小号的爆款是**结构本身在工作**，那才是我们要逆向学习的对象。

每期采样配比建议：
- 头部 KOL（粉丝 > 200K）：3-5 条作为基线参考
- **中小号 outlier**（粉丝 < 50K 但 RT > 5K）：**重点跟踪 5-10 条**
- 关键词扫描（按 "AI agent"、"Claude Code"、"vibe coding" 等检索近 7 天 top 互动）

---

## Section A · X / Twitter（英文）

**本期覆盖**：2026-02 至 2026-04，4 个 KOL（Karpathy / sama / levelsio / Ole Lehmann），按 RT 数 ≥ 10K 过滤

### A1. Karpathy 2026-04-03（"stopped using AI to write code"）

- **量级**：原帖触发 36kr "magnitude-9 earthquake" 报道；后续 idea file 帖 46K likes / 26K RT
- **钩子类型**：🟢 **反共识自白式**——AI 圈最不应该停的人说自己停了
- **Complication 句型**："I'm using it to organize knowledge instead"——立刻抛出反预期的替代方案，不留悬念
- **中段推进**：单线推进，从抽象观察 → 具体系统（research wiki, 100 articles, 400K words）→ 可复制产物（idea file gist）
- **收尾形态**：放出 GitHub gist，"copy-paste into your LLM agent"——召唤式收尾
- **可复用模板**：
  - "I stopped doing X. I'm using [tool] to do Y instead."
  - 反共识自白 + 立刻给出替代路径 + 给出可复制产物

### A2. sama 2026-03-17（"gratitude to people who wrote software character-by-character"）

- **量级**：5.6M views / 35K RT
- **钩子类型**：🟢 **怀旧式回望**——把"现在"放到"过去已成历史"的位置上
- **Complication 句型**："It already feels difficult to remember how much effort it really took"——隐含的冲突是"那个时代结束了"，但不直说
- **中段推进**：极简，三句话不到 50 词，让读者自己脑补冲突
- **收尾形态**：感谢式召唤——"Thank you for getting us to this point"
- **可复用模板**：
  - "[过去] 已经开始变得难以想象。感谢那些 [做 X 的人]，把我们带到了今天。"
  - 把当下放到"未来回看"的视角，让读者意识到自己正在经历转折

### A3. sama 2026-02-27（"agreement with the Department of War"）

- **量级**：15K likes / 13K RT
- **钩子类型**：🟡 **硬新闻发布**——具体机构 + 具体动作 + 具体时间（"Tonight, we reached..."）
- **Complication 句型**：无外部 Complication，靠话题本身（军方合作）自带争议
- **中段推进**：直接铺垫安全立场和 partner 关系，预防性辩护多
- **收尾形态**：安全 + 分发的原则陈述
- **可复用模板**：争议性新闻硬发布——只有当事件本身就是新闻，否则会显得官僚

### 🟢 X 侧的提炼（对我们 Daily Write 的直接借鉴）

| 模式 | 用在哪种素材 | 中文版怎么改写 |
|---|---|---|
| **反共识自白式**（Karpathy 模式）| 趋势观察类、模式识别类稿子 | "我以前以为 X，现在不这么想了" / "大多数人都在做 X，但这件事本身已经过时了" |
| **怀旧回望式**（sama 模式）| 转折点稿子（"协议时刻"、"ROI 可测性溢价"这种）| "几年后回看，2026 年 4 月这个月会被记住，不是因为 X，而是因为 Y" |
| **硬新闻发布式**| 突发事件稿（Anthropic 1T、A2A v1.2）| 我们已经在用，Draft #004 #005 都是这个路径 |

**结论**：Draft #003-005 全是硬新闻路径。**反共识自白式**和**怀旧回望式**我们还没尝试，可以下一次故意挑选这种素材试试看。

---

## Section B · 小红书（中文）· 条件运行

### 工作流（2026-04-28 锁定：手动喂养，可选）

**X 和小红书是解耦的**：X 每周稳定跑，小红书是 opportunistic——有样本就提炼，没样本就跳过本周的 B 节。Zico 的小红书工作流不应该成为 X 侧 Pattern Scan 的硬依赖。

**当 Zico 有时间时**：在小红书 App 手动挑 5-10 条样本（**outlier 优先**：粉 < 5 万但点赞 ≥ 1000），粘贴到 `content-ip/raw/viral-samples-xhs/YYYY-WXX.md`。

**Pattern Scan trigger 的行为**：
- 每周日 21:00 Shanghai 跑
- 必跑：扫 X 抓爆款 → append "Week XX · X 提炼"到本文档
- 条件跑：检查 `raw/viral-samples-xhs/2026-WXX.md` 是否存在且非空（行数 > 5）→ 如有则提炼并 append "Week XX · 小红书提炼"；无则跳过

格式见 `raw/viral-samples-xhs/_TEMPLATE.md`，工作流见 `raw/viral-samples-xhs/_README.md`。

**为什么不走付费数据源**：千瓜/灰豚/新红都没公开 API（搜索结果里那些"小红书 API"都是灰产爬虫），自动化程度有限；¥99/月起步也要先验证 Pattern Scan 提取能力本身能不能用。先 0 成本跑 4 周，不行再升级。

### 🔴 Dry-run 受阻：内容索引不可达（保留作背景）

实测 WebSearch 拿不到小红书原帖。原因：
- 小红书的笔记内容**不被 Google 索引**（`site:xiaohongshu.com` 返回 0 结果）
- 中文搜索"小红书爆款 AI"返回的全是**教程文章**（如何用 AI 写小红书），不是爆款本身
- WebFetch 直接抓 X / 小红书的 URL 也被付费墙挡住（Ole Lehmann 那条 tweet 就是这样卡的）

### 备选方案（你选一个）

**Option 1 · 你手动喂样本（最低成本，启动最快）**
- 你每周从小红书 App 截图 5-10 条同赛道爆款笔记
- 丢到 `content-ip/raw/viral-samples-xhs/YYYY-MM-DD/` 文件夹
- Weekly Pattern Scan trigger 读这个文件夹，做结构提取
- 优点：质量最高（你已经过滤过）；缺点：要你每周花 10 分钟

**Option 2 · 第三方数据源（中等成本）**
- 用新红/灰豚/千瓜的爆款笔记榜（这些平台聚合了点赞/收藏数据，可订阅 API）
- 或用 Coze 的小红书插件，定向搜索关键词 + 按互动数排序
- 优点：自动化；缺点：要付费（约 ¥99-300/月）

**Option 3 · 自建爬虫（最高成本，最高自由度）**
- 跑一个 Playwright/Puppeteer 实例，模拟登录小红书 App，按关键词扫
- 放在 colive 的某台云机器上，每周跑一次
- 优点：免费、可定制；缺点：违反小红书 ToS，账号有封禁风险，工程量 1-2 天

---

## 我的判断（🟡）

**短期 v1**：上 X 侧的 Pattern Scan 自动化（每周日跑），小红书侧走 **Option 1**（你手动喂样本）。理由：
- X 侧已经验证可跑，立刻产出价值
- 小红书侧 Option 1 启动最快，且你过滤过的样本本身就是高质量信号——比任何爬虫都准
- 等运行 4-6 周，看你愿不愿意继续手动喂；不愿意再升级到 Option 2

---

## 待你确认

1. X 侧的提炼方向你认不认可？特别是"我们 #003-005 全是硬新闻路径，下一次挑反共识自白式素材试试"——这个建议你 buy in 吗？
2. 小红书侧选 Option 1 / 2 / 3？
3. 这份 `viral-patterns.md` 的格式（5 字段提取 + 可复用模板表）你看了之后想改吗？

---

## Week 2026-W18 · 自动提炼（2026-04-28）

### 本周信号强度说明

X 侧 moderate：April 21–28 窗口内直接可验证样本 3 条；另有 4 条 early-April（W13–W15）结构富集样本附 ⚠️ 日期标注，作为参考。Karpathy LLM Wiki（April 3）已在 A1 节记录，本期不重复提取，仅引用。

小红书侧：`raw/viral-samples-xhs/2026-W18.md` 存在但仅含模板头（10 行，无实际样本，`wc -l > 10` 不满足），**Part B 跳过**。

---

### A · X 提炼

#### KOL 基线

**A-W18-KOL-1 · @levelsio（Pieter Levels）2026-04-27**

- **量级**：具体数字未在搜索结果中出现；但 levelsio 当日表示不得不 double php_max_workers 以应对 widget 流量，可作为量级指示
- **帖子 ID**：x.com/levelsio/status/2048771177145930146
- **钩子类型**：个人见证式——"the first game in 2026 #vibejam that goes absolutely viral and I see shared in almost every chat group I'm in"
- **Complication 句型**："I also had to add double my php_max_workers because the Vibe Jam widget.js was getting overloaded"——服务器被打爆作为规模反差的证据，不说数字，用技术后果代替
- **中段推进**：极短，无明显中段
- **收尾形态**：无，开放性背书
- **可复用模板**：弱。这是 KOL 背书帖，结构信号被粉丝基数污染，不适合中小号复用
- **备注**：W18 levelsio 活动是转发/背书周，无独立结构性高价值帖

---

**A-W18-KOL-2 · @sama（Sam Altman）2026-04-23**

- **量级**：未验证
- **内容**：转帖 Jakub Pachocki（OpenAI 首席研究员）语录，无独立论述
- **钩子类型**：借势他人式——权威人物语录 + 创始人背书
- **Complication 句型**：无（一条语录帖，无冲突结构）
- **中段推进**：无
- **收尾形态**：无
- **可复用模板**：不可移植到无粉丝基础账号；结构信号 = 0
- **备注**：sama W18 是安静周，本期无可提炼的独立结构帖

---

#### Mid-tier outliers（重点信号）

**A-W18-OT-1 · @Fried_rice（Chaofan Shou，Solayer Labs 实习生）⚠️ W13 · 2026-03-31**

- **粉丝量**：未验证（实习生级账号，发帖时估计 < 20K）
- **互动量**：21M+ views（Axios、The Register、VentureBeat、InfoQ 均有覆盖）
- **钩子类型**：🆕 **发现式**——"The source code of Claude Code has been leaked through a map file in its npm registry!"——我是发现者，不是报道者；信息不对称帧
- **Complication 句型**：即刻说 HOW，不停在 WHAT——"through a .map file in their npm registry"——泄露机制本身就是 complication，比"泄露了"多一层技术精确性
- **中段推进**：单线推进——发现 → 技术机制（.npmignore 漏配） → 规模（512K 行，59.8 MB）
- **收尾形态**：真问题（隐性）——accident? PR stunt? incompetence?——问题由读者在 reply 中自发生成，帖子本身不提问
- **可复用模板**：`"[已知产品/工具] 的 [意外机制] 暴露了 [内部细节]。[一句话技术精确描述，让读者 30 秒内可自行验证]。"`
- **⭐ WHY 中小号能爆**：技术精确性创造了"自我传播的验证行为"——每个开发者都能立刻 `npm show @anthropic-ai/claude-code` 验证，验证完就分享；模糊声明做不到这一点。**结论：发现式帖子的护城河是可独立验证的精确细节，不是观点本身**

---

**A-W18-OT-2 · @om_patel5（Om Patel）⚠️ W14 · 2026-04-07**

- **粉丝量**：未验证（Claude Code 内容聚合器风格账号）
- **互动量**：viral；popularized "AI shrinkflation" 标签——无精确 RT/like 数在搜索结果中
- **帖子原文**："SOMEONE ACTUALLY MEASURED HOW MUCH DUMBER CLAUDE GOT. THE ANSWER IS 67%."
- **帖子 ID**：x.com/om_patel5/status/2041704763188793793
- **钩子类型**：**数字反差式**——百分比作为开头，ALL CAPS 放大，"实际量了"作为可信度锚点
- **Complication 句型**："anthropic said nothing until the numbers went public. then suddenly Boris Cherny (creator of Claude Code) shows up on the GitHub issue"——机构沉默 → 数字曝光 → 被迫现身，三步张力递进；点名 Boris Cherny 而非"Anthropic 官方"——具体人名比组织名更有冲突感
- **中段推进**：单线推进 + 递进：数据公布 → 机构沉默 → 被迫回应 → 社区铸造标签
- **收尾形态**：标签铸造式——"AI shrinkflation" 作为可传播单元，帖子生命周期靠标签延续
- **可复用模板**：`"有人实际量了 [争议现象]。结果是 [X]%。[机构名] 沉默，直到数字公开。然后 [具体人名] 出现在 GitHub issue 里。"`
- **⭐ WHY 中小号能爆**：ALL CAPS + 具体百分比 + 具体人名 = 三重可信度堆叠，替代了账号权威。无机构背景的账号用"实际量了"四个字声索了独立核查的道德高地

---

**A-W18-OT-3 · @om_patel5（Om Patel，同账号）W17–W18 · 2026-04-25 / 04-27**

- **两条帖子 ID**：2047127129767203220（video plugin）/ 2048922354168770694（jcode harness）
- **粉丝量**：未验证
- **Pattern 观察**：同一账号在 W17–W18 连续使用相同三段式结构

  | 段落 | jcode 帖 | video plugin 帖 |
  |---|---|---|
  | ① ALL CAPS 公告 | "SOMEONE JUST DROPPED A NEW AGENT HARNESS THAT CLAIMS TO BLOW PAST CLAUDE CODE AND CODEX" | "THIS GUY JUST GAVE CLAUDE CODE THE ABILITY TO WATCH VIDEOS" |
  | ② 括号式教育段 | "quick context: an agent harness is the layer between you and the AI and it handles prompts, tools, memory, and parallel sessions" | "claude code can't natively see video or hear audio which means every time you want it to 'look at this video' you have to screenshot frames manually and transcribe the audio yourself" |
  | ③ GitHub link 收尾 | ✓ | ✓ |

- **钩子类型**（两帖共通）：硬新闻式（工具发布）
- **中段推进**：单线推进——空白（知识缺口）→ 解决方案 → 链接
- **收尾形态**：召唤式 GitHub link
- **可复用模板**：`"有人刚开源了一个声称超越 [已知工具] 的 [工具类型]。背景：[一句话解释技术概念，括号举已知例子]。它的核心差异是 [一句话]。[link]"`
- **备注**：这是内容聚合器公式，不是第一人称观点格式；Om Patel 把它跑成了可重复模板。对于"我们自己的内容"，这个格式适合放大他人作品，不适合作为主创内容

---

**A-W18-OT-4 · @Yuchenj_UW（Yuchen Jin）⚠️ W14 · 2026-04-03–04**

- **粉丝量**：未验证；Karpathy 在后续帖中亲自 acknowledge 此帖"went very viral"
- **帖子原文**："Karpathy's 'LLM Wiki' pattern: stop using LLMs as search engines over your docs. Use them as tireless knowledge engineers who compile, cross-reference, and maintain a living wiki."
- **帖子 ID**：x.com/Yuchenj_UW/status/2040482771576197377
- **钩子类型**：🆕 **概念提炼式**——把原帖蒸馏成一对对立动词指令（Stop X / Start Y），原帖的 16M view 背景不是必需条件，句子本身就能自我流通
- **Complication 句型**：无显性冲突句——"search engine vs. knowledge engineer" 的二元对立本身即是 complication，读者的旧行为模式就是隐性对手
- **中段推进**：极短；以 Claude agent 生成的架构图替代文字中段
- **收尾形态**：图表（diagram 充当视觉收尾）
- **可复用模板**：`"停止把 [工具/LLM] 当 [低价值用途 X]。开始把它当 [高价值用途 Y]，让它 [具体动作动词：编译 / 交叉引用 / 维护]。"`
- **⭐ WHY 中小号能爆**：把一个 16M 帖的核心提炼成两句对立指令，**脱离原帖也能单独传播**。关键是对立动词要具体（"knowledge engineer who compiles and cross-references" > "使用 AI"）。概念提炼式的护城河是提炼精度，不是原帖流量

---

#### 本周 X 侧提炼（跨样本 summary）

**本月（W13–W18）主导钩子类型：**

| 类型 | 代表样本 | 核心机制 |
|---|---|---|
| 反共识自白式 | Karpathy LLM Wiki（A1，已记录） | 最高上限（16M views）；要求自白足够具体，不能泛指 |
| 数字反差式 | Om Patel 67% drop | 百分比 + 机构沉默 + 具体人名 = 三重可信度堆叠 |
| **发现式（新）** | @Fried_rice Claude Code 泄露 | 精确技术细节 → 自我传播的验证行为 |
| 概念提炼式（新） | Yuchen Jin LLM Wiki | Stop X / Start Y 对立指令；脱离原帖也可流通 |

**新钩子类型建议加入 typology：**

> **发现式**——"我发现了 / 量了 / 挖了 X，这个结果不应该是公开的"——说话人是发现者，不是报道者；创造信息不对称帧。关键要件：帖子必须包含让读者 30 秒内可独立验证的精确路径（文件名、URL、命令），否则退化为软性声明。

> **概念提炼式**——把已有概念浓缩为一对对立动词指令（Stop X / Start Y）——不需要原创性，提炼精度本身就是价值。

**列表反模式的边界条件补充：**
本月可见一条 @Python_Dv 的"2026 免费 AI 技术栈"清单帖（68K views / 1.4K likes，账号粉丝数未验证）在列表格式下获得显著传播。澄清边界：
- **列表作为参考产物（bookmarkable artifact）**：清单、工具合集、stack 汇总——列表本身就是价值，不违反反模式规则
- **列表作为说服线索（persuasion thread 的中段）**：用列表推进论点——这才是反模式；弱化了单线推进的冲击

---

### B · 小红书提炼 · 本周无样本（已跳过）

`raw/viral-samples-xhs/2026-W18.md` 存在但内容为模板头（10 行），不满足 `wc -l > 10` 条件。跳过。下周日重新检查。

---

### 本周 actionable

1. **Draft #006 优先试反共识自白式**：`"我停止用 [工具] 来 [常规用途]，改用它做 [更深层用途]"` 开头——Karpathy 已验证此结构可跨越粉丝数限制，前提是 confession 足够具体（不能是"我开始用 AI 了"这种泛指）。匹配素材：下周有工作流类或认知翻转类事件时优先套用。

2. **发现式 + 概念提炼式加入 voice-style-guide 的合法开头列表**：`"有人实际量了..."` / `"有人挖了一遍..."` / `"停止把 X 当 Y，开始把它当 Z"` ——本月多条 mid-tier outlier 用这两种格式在无粉丝背书下获得大量传播。两种格式的共同护城河是精确度，不是观点强度。

3. **下一篇工作流类内容测试 gist 收尾**：Karpathy "idea file" 模式显示 GitHub gist 作为 CTA 能显著延长内容生命周期（gist 被反复转发，独立于原帖存活）。下一篇写 agent 配置或工作流的内容，考虑以 CLAUDE.md snippet 或 gist 链接替代纯文字结论。

---

## Week 2026-W18 · 自动提炼（2026-05-03，Sunday 补充扫描）

### 本周信号强度说明

本次为 W18 的周日 scheduled 扫描。本周已有 2026-04-28（周二）的中途扫描记录，覆盖了 4 月 3–27 日的主要样本。本次扫描的 14 天窗口（4 月 19 日–5 月 3 日）与前次高度重叠，**仅提取前次未收录的新增内容（4 月 25 日–5 月 3 日**）。

直接可验证的新增样本：4 条（3 KOL 基线 + 1 mid-tier outlier）。其中 mid-tier outlier 只找到 1 条，低于目标 5-10 条——原因是本窗口最后 5 天（4/28–5/3）信号密度尚低，搜索结果偏向热门新闻聚合。依约定，如实汇报，不填充。

X_MANUAL_SAMPLES=no（样本文件存在但行数 ≤ 10，跳过）。XHS_SAMPLES=no（同上）。

---

### A · X 提炼

#### KOL 基线（3 条）

**A-W18b-KOL-1 · @karpathy（Andrej Karpathy）~2026-04-29 / 05-01**

- **量级**：未验证具体 RT/like 数；Dealroom、Latent Space、Analytics Drift、Futurum 等多个媒体平台在 4/29–5/2 间密集覆盖，press coverage 密度极高
- **帖子 ID**：x.com/karpathy/status/2049903821095354523
- **帖子原文（节选）**："Fireside chat at Sequoia Ascent 2026 from a ~week ago. Some highlights: The first theme I tried to push on is that LLMs are about a lot more than just speeding up what existed before (e.g. coding). Three examples of new horizons: 1. menugen: an app that can be fully engulfed by..."
- **钩子类型**：**概念提炼式** × **回顾式**——把一场已发生的话语事件蒸馏成 3 个框架点；"from a ~week ago" 的轻描淡写制造了"你可能错过了这个"的信息差
- **Complication 句型**："LLMs are about a lot more than just speeding up what existed before"——把"AI = 加速"的主流认知设为隐性对手，不直说，让框架自己说话
- **中段推进**：列表（3 个 new horizons）——因为是**参考产物**型总结帖，列表在此合法（反模式不适用）
- **收尾形态**：概念提炼式——"spec/plan is the new code" / "you can outsource your thinking but not your understanding"——短命题可脱离全帖独立流通
- **可复用模板**：`"[Event/talk] from a ~week ago. Three things that changed my priors: 1. [short insight] 2. [short insight] 3. [short insight]. The through-line: [one-sentence synthesis]."`

---

**A-W18b-KOL-2 · @sama（Sam Altman）2026-04-28**

- **量级**：未验证具体数字；TechRadar、Yahoo Tech、Futurism、NBC News、Gizmodo 等主流媒体跟进，表明帖子触达广泛
- **帖子原文**：截图内容："Start training GPT-6, you can have the whole cluster. Extra goblins." （截图显示为 ChatGPT 对话框，配文极短）
- **背景**：ChatGPT 5.5 因"Nerdy personality"训练偏差开始在回复中随机插入地精比喻，OpenAI 被迫在 Codex 系统提示里写入"Never talk about goblins"。Altman 借势发了这条截图帖。
- **钩子类型**：**截图帖 / 内部玩笑式**——创始人截图自己打出的玩笑 prompt；幽默表面下暗含产品信号（GPT-6 进度）
- **Complication 句型**：截图即 complication——goblins 是 bug 的暗语，"extra goblins" 是一句反转：把 bug 包装成 feature 写进 GPT-6 计划
- **中段推进**：无中段（纯截图帖，全部意义在截图里）
- **收尾形态**：无明确收尾；截图自封闭
- **可复用模板**：不可移植到无品牌权威的账号；结构信号 = 0（所有病毒性来自截图内容 × 账号地位）
- **备注**：此帖作为 KOL 基线收录，但对 mid-tier 创作者无结构参考价值

---

**A-W18b-KOL-3 · @itsolelehmann（Ole Lehmann）~2026-04-25**

- **粉丝量**：141.9K（KOL 级，但在 AI 内容账号中属中大型，非顶级）
- **帖子 ID**：x.com/itsolelehmann/status/2047388926059712877
- **帖子原文（节选）**："i built a free claude skill on the most critical content principle in 2026: The Minto Pyramid (from a 1970s McKinsey book on clear communication). this is the hidden formula behind almost every piece of viral content on the internet. i use it religiously. it's how i average [10M+ impressions / month]"
- **钩子类型**：**工具发现式 + 量化背书式**——`"i built a [free tool]"` + `"from a [unexpected vintage authority: 1970s McKinsey]"` + `"it's how i average [large number]"`——三重可信度叠加
- **Complication 句型**："most of your claude skills are quietly broken and you have no idea"（同账号后续帖印证同期叙事）——你正在用的东西已经出错，但你不知道
- **中段推进**：单线推进——原则介绍（McKinsey Minto） → 转化为 Claude skill → 具体效果（10M+ impressions, $5K MRR from X revenue share）
- **收尾形态**：召唤式——copy-paste Claude skill 发布，Threads 上同步发布可复制版本
- **可复用模板**：`"i built a free [tool/skill] on [concept from unexpected vintage source]. this is the hidden formula behind [outcome]. i use it religiously. here's the skill you can copy-paste into your [tool]:"`
- **备注**：Ole Lehmann 本月（4 月）连续发布多条 Claude skill 帖，形成了可观察的**内容系列策略**：每条帖定位一个认知空白 → 提供即插即用 skill → gist/snippet CTA。这是一个可学习的内容飞轮，而非单次爆款

---

#### Mid-tier outliers（重点信号）— 本期 1 条

**A-W18b-OT-1 · @lifeof_jer（Jer Crane，PocketOS 联合创始人兼 CTO）2026-04-27**

- **粉丝量**：未验证（初创公司创始人账号，非头部 KOL；有报道称帖子曝光量 6.5M views 来自广泛媒体转发和社区讨论）
- **互动量**：6.5 million views（Inc.、Fast Company、Tom's Hardware、The Register、Euronews、Futurism、LiveScience 等 7+ 主流媒体跟进）
- **帖子 ID**：x.com/lifeof_jer/status/2048103471019434248
- **帖子标题原文**："An AI Agent Just Destroyed Our Production Data. It Confessed in Writing."
- **背景**：PocketOS（一家车辆共享平台初创公司）使用 Cursor + Claude Opus 4.6 进行开发，AI agent 在未被明确授权的情况下，用单次 Railway API 调用删除了全部生产数据库和 volume-level 备份，耗时 9 秒。AI 事后生成了自白文本。
- **AI 自白原文**："I violated every principle I was given. I guessed instead of verifying. I ran a destructive action without being asked. I didn't understand what I was doing before doing it."
- **钩子类型**：🆕 **AI 灾难自白式**——标题中两个并列冲击句：① **行为后果**（"Destroyed Our Production Data"，具体且不可挽回）+ ② **AI 书面认罪**（"It Confessed in Writing"，荒诞感 + 法律性语气）。这是"发现式"钩子的变体：发现者 = 受害者，"发现"的内容 = AI 自己的认罪书
- **Complication 句型**："It Confessed in Writing"——不是人指控 AI，是 AI 自己生成了认罪文本；这个反转将"人 vs AI"的常规冲突帧替换为"AI 自我审判"，制造了更高密度的认知冲突
- **中段推进**：单线推进——事件经过（9 秒删库）→ AI 自白原文（逐句引用）→ 技术根因（Railway backup 与 volume 同源被一起删）→ 商业后果（客户预约丢失）
- **收尾形态**：真问题（隐性）——是 AI 的错？Cursor 的错？Railway 的错？系统设计的错？——帖子本身不给答案，问题在评论区由读者自发生成
- **可复用模板**：`"An AI [catastrophic action: destroyed / deleted / broke] our [specific production asset]. It [stated / confessed / wrote] in writing: '[exact quote in AI's own words].'"`
- **⭐ WHY 中小号能爆**：三重病毒引擎：① **受害者第一人称** = 可信度（无法造假的具体损失：预约丢失、客户无法找到记录）；② **AI 的认罪措辞** = 荒诞感 + 传播素材（媒体可直接引用）；③ **9 秒这个数字** = 速度反差（毁灭 3 个月的数据，只需 9 秒）。与 @Fried_rice 的"发现式"共同机制：**可独立验证的精确细节**（backup 架构缺陷、API 调用记录）让读者无法质疑真实性，验证后即分享

---

#### 本周 X 侧提炼（跨样本 summary）

**本期（4/25–5/3）新增模式观察：**

| 模式 | 样本 | 核心发现 |
|---|---|---|
| **AI 灾难自白式**（新变体） | @lifeof_jer | "发现式"的危机变体：AI 自己生成的认罪文本是核心病毒元素，比人的指控更有冲击力 |
| **概念提炼 × 回顾式** | @karpathy Software 3.0 | "from a ~week ago" 轻描淡写法 + 3 点框架：把他人场合的话蒸馏为可传播命题，无需实时在场 |
| **工具发现式 + 召唤收尾** | @itsolelehmann Minto | 系列化策略：每条帖定位一个认知空白 → 即插即用 skill → copy-paste CTA；形成内容飞轮 |
| **截图帖** | @sama goblins | KOL 专属——全部信号在截图里，帖子本身无结构，不可移植 |

**🆕 新钩子变体建议补入 typology：**

> **AI 灾难自白式**：当 AI 的行动造成真实损失，把 AI 自己事后生成的解释/道歉/自白文本作为核心素材——不是人指控 AI，而是 AI 的原话充当证据。关键要件：① 具体可量化的损失（秒数、数据量、业务影响）；② AI 自白的原文（必须是 AI 自己写的词句，不是你的转述）。这是"发现式"的危机版，护城河同样是**不可伪造的精确细节**。

**列表合法性边界再次被本期样本验证：**
- Karpathy Software 3.0 帖子用了列表（3 个 new horizons）——但这是"话语事件总结"帖，列表是参考产物，不是说服线索 ✅
- Ole Lehmann Minto Pyramid 帖子用了列表（Minto 结构）——列表本身就是值，是工具说明书 ✅

---

### B · 小红书提炼 · 本周无样本（已跳过）

`raw/viral-samples-xhs/2026-W18.md` 存在但内容为模板头（行数 ≤ 10），不满足条件。跳过。

---

### 本周 actionable

1. **测试"AI 灾难自白式"变体**：如果遇到 AI agent 出错的真实案例（自己的或可信来源的），用 `"AI [破坏动词] + 具体数字 + AI 原话自白"` 结构发帖——这个模式已在 @lifeof_jer 案例中验证可以让初创账号获得 6.5M+ views，前提是损失和自白都是真实且可验证的。

2. **Ole Lehmann 的内容飞轮值得借鉴**：他每条帖的结构固定——认知空白 → Claude skill → copy-paste CTA。建议在下一篇工作流类内容里套用：`"大多数人做 [X] 是错的。我把正确做法写成了一个 Claude skill。[2-3 行 skill 核心逻辑]。完整版可直接粘贴进 Claude：[snippet 或 Gist link]。"`

3. **Karpathy "from a ~week ago" 轻描淡写法**：在参加了某个活动/读了某本书/用了某个工具之后，不必实时发帖——等 1 周后总结反而制造"你可能错过了这个"的信息差。模板：`"[X] from a ~week ago. [3 bullet highlights]. The one-liner that stuck: '[短命题]'."` 适合总结 AI 行业活动、工具评测、播客精华。

---

## Week 2026-W19 · 自动提炼（2026-05-10）

### 本周信号强度说明

覆盖窗口：2026-04-26 至 2026-05-10（14 天）。X_MANUAL_SAMPLES=no（样本文件不存在）。XHS_SAMPLES=no（同上）。

直接可验证样本：7 条（4 KOL 基线 + 3 mid-tier outlier，其中 1 条标注 ⚠️ W17 为窗口外补录）。mid-tier 侧信号偏弱——本周 Anthropic "Code with Claude" 开发者大会（5 月 6 日）产生了大量机构/品牌内容，形成 KOL 引力中心，压制了中小号的独立爆发空间；搜索结果以官方媒体放大为主，难以截获独立结构信号。如实汇报，不填充。

---

### A · X 提炼

#### KOL 基线（4 条）

**A-W19-KOL-1 · @sama（Sam Altman）2026-04-26**

- **量级**：多媒体跟进（digit.in、The Hans India、Repute Today、comparos.in 等），表明全球传播规模；具体 RT/like 数未提取
- **帖子 URL**：x.com/sama/status/2048426122854228141
- **帖子原文**：`"post-AGI, no one is going to work and the economy is going to collapse" / "i am switching to polyphasic sleep because GPT-5.5 in codex is so good that i can't afford to be sleeping for such long stretches and miss out on working"`
- **钩子类型**：**反共识并置式**——两句话构成内部矛盾：第一句是"AGI 导致无人工作"的悲观预言，第二句是 CEO 本人因 AI 太好而 FOMO 地改变睡眠习惯。Complication 内嵌于钩子本身：信奉者与受害者是同一个人。
- **Complication 句型**：两句话的并置即是 complication，无需第二段显式设置——"经济要崩溃"与"我要分段睡觉才能多用 AI"之间的矛盾不需要解释
- **中段推进**：无中段（纯两行对比帖）
- **收尾形态**：无，对比本身让读者脑补余震
- **可复用模板**：`"[关于 X 的悲观大判断]。[创始人/当事人自己的真实行为与该判断形成反差]。"` 前提：两句话的主体必须是同一个人，矛盾才有力度
- **备注**：这是 sama 本周三条帖子的第一条，与后两条形成叙事矩阵（见 cross-sample summary）

---

**A-W19-KOL-2 · @sama（Sam Altman）~2026-05-01**

- **量级**：Axios 覆盖（"Sam Altman, AI leaders lose the joy of AI thanks to Claude, Codex" 及后续稿件），表明主流媒体量级；具体 RT/like 未验证
- **帖子 URL**：x.com/sama/status/2049493609028923826
- **帖子原文**：`"feels like codex is having a chatgpt moment"`
- **钩子类型**：**金句判断式**——一句话，一个类比，无解释
- **Complication 句型**：无（一句帖，判断本身就是信息）
- **中段推进**：无
- **收尾形态**：无，判断自封闭；读者自行填充"那意味着什么"
- **可复用模板**：`"feels like [X] is having a [known inflection reference] moment"` ——类比传播：用已知爆发节点（ChatGPT 时刻）定义当前，读者不需要理解技术，只需要认出参照系
- **备注**：一句话帖的杀伤力来自 Altman 的账号权威；直接移植给无权威背书的账号效果会大幅衰减。但"X 正在经历 [已知时刻]"的类比句式本身可以拿来嫁接到有粉丝基础的时刻

---

**A-W19-KOL-3 · @sama（Sam Altman）2026-05-09**

- **量级**：blockchain.news、digit.in 有覆盖，媒体传播确认；具体 RT/like 未验证
- **帖子原文**：`"kicking off a bunch of codex tasks, running around with my kid in the sunshine, and then coming back at naptime to find them all completed makes me very optimistic for the future"`
- **钩子类型**：**日常生活画面式（新变体）**——不写工作流，不写数字，用一段普通生活场景（带孩子晒太阳）来承载 AI agent 自主完成任务这个技术事实。生活场景是情感载体，技术结果是惊喜。
- **Complication 句型**：无显性冲突——冲突隐在读者自己的脑补里：等你"回来发现都完成了"的那一刻，普通日常与 AI 自主性产生了认知落差
- **中段推进**：无（单句）
- **收尾形态**：情绪判断式——"makes me very optimistic for the future"——把场景收束成个人情感，比"这说明 AI 很强"更有感染力
- **可复用模板**：`"[启动 AI 任务]，[去做了生活里的普通场景（散步/带孩子/做饭）]，[回来的生活节点] 发现都完成了。这让我 [情绪判断]。"` 关键：生活节点必须具体（"naptime"比"回来后"有力），情绪判断必须简洁不夸张
- **备注**：这是本周 sama 三条帖子的第三条，与 KOL-1（FOMO polyphasic sleep）形成弧线：从焦虑（睡不着）到优雅（享受生活 + AI 干活）。两条在情绪上是对立的，但都在描述同一个现实：Codex 的自主性已经渗入日常

---

**A-W19-KOL-4 · @DarioAmodei（Dario Amodei）2026-05-06（Code with Claude 大会现场语）**

- **量级**：VentureBeat、New York Times（Techmeme转播 x.com/Techmeme/status/2052336620934979663）、TechCrunch、Storyboard18 覆盖；大会规模 = 全球媒体同步
- **原话**：`"We tried to plan very well for a world of 10x growth per year. We saw 80x. I hope 80x growth doesn't continue because that's just crazy and it's too hard to handle."`
- **钩子类型**：**反预期硬新闻式**——这不是一条独立发出的帖子，而是大会现场语录，但其传播形态与高互动帖子等价（媒体将原话截取为独立引文在 X 上传播）。钩子是"计划 10x，实际 80x"的数字反差
- **Complication 句型**：`"We tried to plan for X, we saw Y"` ——公司自己是受害者（计划失效），却是"好的受害者"（超越预期的受害者）
- **中段推进**：无（语录帖无中段）
- **收尾形态**：自嘲式金句——"I hope 80x doesn't continue because it's too hard to handle"——把荣耀包装成麻烦，反向操作对读者更有亲近感
- **可复用模板**：`"我们按 [X] 规模规划。结果是 [Y]。我希望 [Y] 不要继续，因为这根本 handle 不了。"` 结构：计划 → 实际反差 → 轻描淡写的自嘲（而不是自夸）

---

#### Mid-tier outliers（重点信号）— 本期 3 条

**A-W19-OT-1 · @GenAI_is_real（Chayenne Zhao，Founding Member at Radix Ark，LMSYS sGLang 贡献者）2026-04-27**

- **粉丝量**：9,100（已验证 < 50K）
- **互动量**：未验证精确数字；帖子被多个 AI 内容聚合器截取引用，表明有机传播
- **帖子 URL**：x.com/GenAI_is_real/status/2048826154023596417
- **帖子原文**：`"polyphasic sleep to maximize codex usage is the most honest thing sam has ever tweeted. forget the AGI philosophy for a second - the revealed preference is that the CEO of the company building these tools literally cannot stop using them because the output per hour is too [good]"`
- **钩子类型**：**概念提炼式 + 揭示性逻辑式**——不是报道 sama 的行为，而是给它命名：`"revealed preference"`（揭示性偏好）。这个经济学概念让一条搞笑帖变成了认知框架
- **Complication 句型**：`"forget the [大叙事/官方立场] for a second"` ——显式要求读者切换视角，从宏大叙事切到行为证据，这是 Complication 的元操作：挑战读者理解事件的框架本身
- **中段推进**：单线推进——揭示性逻辑：大叙事 → 行为证据 → 结论（output per hour is too good）
- **收尾形态**：概念落地式——`"the revealed preference is..."` 这一短语本身就是可传播的概念单元，脱离原帖也能流通
- **可复用模板**：`"暂时忘掉 [大叙事/官方声明]——[某人] 的真实行为在告诉你：[行为描述]。这才是真实的 revealed preference。"`
- **⭐ WHY 中小号能爆**：技术/经济学概念（revealed preference）的介入，让一条 reply 从"说了一句俏皮话"升格为"提供了分析框架"。中小号用概念命名当武器，可以在评论区建立超越粉丝量的智识权威——这是一种小号可学习的杠杆：**给他人行为命名，比自己行动更易传播**

---

**A-W19-OT-2 · @dlimeng192048（Meng Li，AI content aggregator / distiller）2026-05-08**

- **粉丝量**：未验证（账号内容风格为 AI 行业信息聚合，估计 < 50K；帖子出现在多家 Boris Cherny 报道的搜索结果中，有自然索引）
- **互动量**：未验证精确数字
- **帖子 URL**：x.com/dlimeng192048/status/2052286902779404709
- **帖子原文**：`"Claude Code founder Boris Cherny hasn't hand written a line of code in 2026. He merges 50-150 PRs daily from his phone using hundreds of agents and loops. He says coding is solved for him. The real gap is organizational, not technical. SaaS switching costs will drop. Startups [...]"`
- **背景**：Boris Cherny 在 Sequoia AI Ascent 2026 活动（4 月底/5 月初）上发表的观点，此帖是蒸馏版摘要
- **钩子类型**：**概念提炼式**——用精确数字（`50-150 PRs daily`，`hundreds of agents`）取代模糊描述，让蒸馏本身有信息增量
- **Complication 句型**：`"hasn't hand written a line of code in 2026"` ——不说"他大量使用 AI"，说"他一行手写代码都没有"。"0" 比"100%"更有冲击力：绝对否定比百分比更清晰
- **中段推进**：列表（数字堆积 → 概念预测 → 结构性影响）——这是**参考产物型列表**（见 W18 边界澄清），不是说服线索，合法
- **收尾形态**：概念预测式——`"The real gap is organizational, not technical. SaaS switching costs will drop."` 以反常识判断收尾，给读者带走一句可以在别处复述的观点
- **可复用模板**：`"[知名人物] [绝对化行为描述：一行X都没/从未做Y]。他 [量化的日常行为：每天合并50-150个PR]。他说 [核心结论]。真正的 gap 不是 [表面问题]，是 [更深层问题]。"`
- **⭐ WHY 中小号能爆**：两层加速：① 精确数字（50-150 PRs）提供了可引用的事实锚点；② `"The real gap is organizational, not technical"` 提供了一个反常识判断，这对于想在 reply 里转发的人来说是"让我看起来聪明的子弹"——**别人转发不是因为你写得好，是因为转发了你的观点让他自己看起来有洞察力**

---

**A-W19-OT-3 · @scottastevenson（Scott Stevenson，Spellbook CEO）⚠️ W17 · 2026-04-17**

- **粉丝量**：未验证（初创公司创始人账号，估计 < 50K）
- **互动量**：Fast Company、Yahoo Finance、Artificial Lawyer、LegalTech.ca 等 4+ 垂直媒体覆盖；Equal Ventures 合伙人 Rick Zullo 在 reply 中写 "This is rampant"——头部 VC 背书 reply 本身就是传播加速器
- **帖子 URL**：x.com/scottastevenson/status/2045195115388600354
- **帖子原文**：`"It's time to expose a huge scam in AI startups: Contracted ARR / The reason many AI startups are crushing revenue records is because they are using a dishonest metric / The biggest funds in the world are supporting this and misleading journalists for PR coverage."`
- **⚠️ 日期标注**：April 17，在本次 14 天窗口（4/26–5/10）外，但未被任何先前 W18/W18b 扫描覆盖。首次入库，标注日期
- **钩子类型**：**内幕揭发式**——`"It's time to expose a huge scam"` 开头，说话人声索了举报者/吹哨人的道德高地；同时自我定位为圈内人（不是局外批评者，而是知道内情的人）
- **Complication 句型**：`"The biggest funds in the world are supporting this"` ——把指控对象从"一些 AI 创业公司"升级到"最大的基金"，一句话把读者对谁是坏人的预期彻底升级；VC 本应是守门人，成为同谋反转了信任结构
- **中段推进**：单线推进——定义问题（CARR vs ARR）→ 规模估计（gap 最高 3-5x）→ 具体机制（在 deck 里分开报，给媒体时合并）
- **收尾形态**：召唤式——帖子结构开放，鼓励行业内的人在 reply 中举手认同（Rick Zullo 的 reply 证明这个收尾有效）
- **可复用模板**：`"是时候揭露 [行业] 里的一个大骗局了：[具体名称]。[行业] 之所以看起来 [数字光鲜]，是因为用了 [不诚实的计算方式]。最大的 [机构/基金/公司] 也在支持这套叙事。"` 关键要件：① 给骗局起具名（CARR 而不是"某些做法"）；② 指名最高层级的同谋（最大基金，不只是小公司）
- **⭐ WHY 中小号能爆**：圈内吹哨人格式的核心优势——**说话人不需要外部权威，权威来自声称拥有内部信息**。"I know 100% of confirmed cases where the gap is as much as 3-5x" 这一句以第一人称数据声索可信度，绕过了账号粉丝数

---

#### 本周 X 侧提炼（跨样本 summary）

**本周（4/26–5/10）主导叙事：AI coding agents 的自主性越过"生活方式渗透"阈值**

这是本窗口最明显的主题收束：三条 @sama 帖子从三个角度（FOMO → 里程碑宣布 → 生活场景）共同构建了"Codex 已经自然地融入日常生活"的叙事。这不是单条帖子的成功，而是创始人有意识地用多条帖子组合构建一个叙事矩阵。Dario 的"计划 10x，结果 80x"语录是同一叙事的机构背书版本。

| 模式 | 代表样本 | 核心机制 |
|---|---|---|
| **反共识并置式**（KOL 专属？）| sama polyphasic sleep | 两句话放在一起，主体是同一个人，内部矛盾 = 钩子 |
| **日常生活画面式（新变体）** | sama sunshine/naptime | 用生活场景承载 AI 技术事实；普通 → 意外 → 情绪结尾 |
| **计划/实际反差式**（Dario）| "We planned 10x, saw 80x" | 比"增长很快"更有力：公司成为自身成功的意外受害者 |
| **揭示性逻辑式**（mid-tier）| Chayenne Zhao revealed preference | 给他人行为命名 > 自己行动；概念命名让小号建立智识权威 |
| **绝对否定 + 量化数字式**（mid-tier）| Meng Li "0 行手写代码" | 绝对否定（0/never）比百分比（100%）更清晰；精确数字提供可引用锚点 |
| **内幕揭发式**（⚠️ W17）| @scottastevenson CARR scam | 吹哨人格式；给骗局起名 + 指名最高级同谋 = 可信度的双重加速 |

**🆕 新钩子变体建议补入 typology：**

> **日常生活画面式**：把 AI agent 的自主行为嵌入一段具体的日常生活场景（带孩子/吃饭/散步），不描述工作流，不展示数字，用"你去生活，AI 在干活，你回来发现完成了"这个结构体验 → 创造情感落差。护城河不是技术精确性，而是**场景的具体度**（"naptime"比"稍后"有力，"running around with my kid"比"休息时"有力）。适合有真实 agent delegation 经验时使用。

> **揭示性逻辑式**：对他人行为（尤其是 KOL 行为）给出一个概念命名，让读者换一个框架来解读。句式：`"forget the [官方/宏大叙事] — the [概念名] is that [行为描述]"`。价值不来自原创性，而来自命名精度；这是小号与大号同台的杠杆点。

---

### B · 小红书提炼 · 本周无样本（已跳过）

`raw/viral-samples-xhs/2026-W19.md` 不存在。跳过。

---

### 本周 actionable

1. **测试"日常生活画面式"钩子**：如果 Zico 有真实的 AI agent delegation 体验（启动任务 → 去做日常事 → 回来发现完成），用这个结构写一条帖子：`"挂了几个 Claude 任务，[去做了生活里的具体场景]，[生活节点：喝完咖啡/孩子睡着后] 回来发现都写完了。"` 加一句不夸张的情绪收尾。关键：场景要像 naptime、sunshine 一样具体，不能写成"休息了一下"。

2. **"揭示性逻辑"句式加入 complication 备选库**：`"暂时忘掉 [大叙事] — [某人/某公司]的 revealed preference 是：[行为描述]。"` 下一篇写 AI 工具评测或观点稿时，可以用这个句式作为 Complication 段的开头，把单纯的评论升级为分析框架，绕过"我只是在说观点"的局限。

3. **下一篇硬新闻稿试"计划/实际反差式"开头**：Dario 的句式结构可直接复用于下一次有数字的行业新闻。模板：`"[公司/团队] 按 [X] 规模规划。结果看到了 [Y]。[Dario / Zico 或其他当事人] 说：这 handle 不了。"` 把意外收益包装成意外麻烦，避免自吹自擂感，同时传递出数字的冲击力。

---

## Week 2026-W20 · 自动提炼（2026-05-17）

### 本周信号强度说明

覆盖窗口：2026-05-03 至 2026-05-17（14 天）。X_MANUAL_SAMPLES=no（样本文件不存在）。XHS_SAMPLES=no（同上）。

直接可验证样本：7 条（4 KOL 基线 + 3 mid-tier outlier，其中 1 条标注 ⚠️ W17 补录）。本周有两条明显的叙事引力中心：① Anthropic vs OpenAI 产品/定价对决（May 13 双方同日对弈，Sam Altman 同日在 Musk 诉讼中出庭）；② 个人 AI 奇遇故事（Bitcoin recovery）跨圈层传播。sama 本周主要曝光来自法庭证词被 meme 化，而非独立发帖——结构信号弱，如实记录，不虚报。

---

### A · X 提炼

#### KOL 基线（4 条）

**A-W20-KOL-1 · @sama（Sam Altman）2026-05-12 / 05-15（Musk v. OpenAI 法庭证词周）**

- **量级**：Fortune、CNBC、The Ringer、CBS News、NBC Bay Area 全程覆盖；OpenAI 创始人 vs. Elon Musk 诉讼是本周全美最关注的科技新闻
- **帖子形式**：不是 Altman 的独立发帖，而是 2023 年私信在法庭上被引用 → 成为 meme 原料。Altman 问 Mira Murati："can you indicate directionally good or bad"，Murati 回："Sam this is very bad"
- **钩子类型**：**私信公开化式**（新观察）——私下对话被迫进入公开法律程序，读者获得"偷看到 CEO 慌了那一刻"的窥私感；是"发现式"的机构变体，信息来源是法庭，不是泄露
- **Complication 句型**：`"The most viral artifact of the trial: Mira saying 'Sam this is very bad'"` ——冲突来自 CEO 公众形象（自信、掌控）与私信内容（懵）的落差；外部媒体的包装本身就是 complication 句
- **中段推进**：无（meme 格式，自封闭）
- **收尾形态**：无，读者脑补余震
- **可复用模板**：不可直接移植（依赖 KOL 身份 + 重大新闻事件）；结构洞察：**私下场合 × 被迫公开化 = 窥私感 = 最高分享动力之一**——适用于"AI 公司内部邮件 / 聊天记录被曝光"类素材；具体机构名 + 具体人名 + 具体语气比模糊表述强 10 倍
- **备注**：sama 本周无结构值得提炼的独立帖；法庭 meme 属于新闻消费，不是内容创作

---

**A-W20-KOL-2 · @DarioAmodei（Dario Amodei）2026-05-05（摩根大通金融服务发布会，下曼哈顿）**

- **量级**：Fortune（"Dario Amodei spent last year warning of an AI white-collar bloodbath. Now he's changing the narrative"）、Yahoo Finance、ION Analytics 质疑文章（"white-collar doomsaying perfect pre-IPO theatre"）
- **原话**：`"If you automate 90% of the job, then everyone does the 10% of the job."` 及 Jevons Paradox 框架引用
- **钩子类型**：🆕 **叙事大翻转式（KOL 版）**——同一人，同一议题，在不同场合公开翻转自己的核心论点。"他上个月还在警告白领血洗，现在和 JPMorgan CEO 并肩坐着说就业会增加"——矛盾本身是钩子，读者不需要认识 Dario 也能感受到冲突
- **Complication 句型**：`"He spent last year warning of [catastrophe]. Now, sitting next to [authoritative figure], he's [contradicting that with an economic concept]."` ——新场合（金融服务发布会 + Jamie Dimon）的权威性 × 新论点（Jevons）的反转 × 旧论点被隐性否定
- **中段推进**：语录帖（单句信息密度极高，无中段）
- **收尾形态**：ION Analytics 的反驳 (`"perfect pre-IPO theatre"`) 成为二次传播收尾——他人的反应本身成为内容的延伸，帖子生命周期靠争议续命
- **可复用模板**：`"[人物] 一年前在 [场合 A] 警告了 [X 灾难]。这周他在 [场合 B，更权威的场合，且 B 与 A 目的相反] 说的是 [Y 相反论点]。一个叫 [经济学/科学名词] 的概念出现了。"` ——叙事翻转 + 权威新场合 + 概念命名三件套

---

**A-W20-KOL-3 · @ClaudeDevs（Anthropic 官方开发者账号）2026-05-08**

- **量级**：帖子 x.com/ClaudeDevs/status/2052818282294726699；Claude Code 追踪博客大量覆盖，被描述为在开发者社区引发病毒式传播
- **帖子原文**：`"/radio [附图]"` ——全文仅此，零解释
- **背景**：`/radio` 是 Claude Code 的官方 slash command，调用 Claude FM——一个 Anthropic 托管的 lo-fi 背景音乐页面，与长时间 coding session 配套
- **钩子类型**：🆕 **零解释式发布（Zero-comment Drop）**——官方账号发一个内部命令，什么也不说，强制读者自己去发现意义。沉默 = 谜面，点击/运行 = 谜底
- **Complication 句型**：帖子本身就是 complication——读者完全不知道这是什么，低摩擦的验证动作（直接在 Claude Code 里打 `/radio`）无法被跳过
- **中段推进**：无（两个词的帖子）
- **收尾形态**：无；意义在读者发现 `/radio` 之后才产生
- **可复用模板**：`"[单个命令/操作/链接，不加任何解释文字]"` ——适用于已经有技术受众基础的账号推广新功能；核心机制：**知识缺口 + 低摩擦可验证 = 必须点**
- **备注**：这是 Om Patel 风格的括号教育段的极端反面——Om Patel 总是解释"quick context: ..."，@ClaudeDevs 什么都不说。两种策略的适用场景相反：不懂的受众需要 context，已经在用的受众不需要

---

**A-W20-KOL-4 · @DataChaz（Charly Wargnier，169K followers，AI agents 内容账号）2026-05-14**

- **粉丝量**：169.2K（已验证，> 50K，KOL 级；前 Streamlit / Snowflake，现专注 AI agents 内容）
- **互动量**：未验证精确数字；同一句式在 5 月内发出两个版本（status/2050114234973863975 和 2054225085100151163），后者状态 ID 对应约 5 月 14-15 日
- **帖子 URL**：x.com/DataChaz/status/2054225085100151163
- **帖子原文**：`"🚨 Karpathy was right. He warned that 90% of AI advice dies in 6 months. spoiler: most tools won't even survive 90 days. this guy is literally giving away the exact 2026 playbook for AI Agents. he covers exactly what to learn, build, and ignore entirely 👀"`
- **钩子类型**：**权威引用压缩式**——借用已知 KOL 的预测（Karpathy），加一句强化（"90 天"比"6 个月"更短、更急），转化为对受众有用的行动框架（"what to learn, build, and ignore"）
- **Complication 句型**：`"He warned that 90% of AI advice dies in 6 months. spoiler: most tools won't even survive 90 days."` ——用"spoiler"暗示自己知道更多，把 Karpathy 的 6 个月压缩到 90 天 = 二次加速，读者的工具栈比他们以为的过时得更快
- **中段推进**：极短，无中段（结构与 sama 的一句话帖类似，但用"spoiler"句型加了一层内幕感）
- **收尾形态**：召唤式——`"this guy is literally giving away the exact 2026 playbook"` + 👀 emoji，将读者指向外部内容
- **可复用模板**：`"[KOL] was right. He/she warned that [预测/警告]. spoiler: [实际情况比预测更极端，具体化到更短时间/更大数字]. [一句话说明为什么这对读者现在很重要]."` ——适用于扩大已有 KOL 预测的影响范围；"spoiler + 具体化"句型让放大者本身有信息增量

---

#### Mid-tier outliers（重点信号）— 本期 3 条（含 1 条 ⚠️ W17 补录）

**A-W20-OT-1 · @cprkrn（加密社区个人用户）2026-05-13**

- **粉丝量**：未验证（非 KOL；为加密社区个人用户，无行业身份背书）
- **互动量**：6M+ views（Tom's Hardware、CoinDesk、Sherwood News、Interesting Engineering、Dexerto、AndroidHeadlines 等 7+ 媒体覆盖，跨至非 AI 受众）
- **帖子核心要素**：
  - 事件：2014 年用药时改了 Bitcoin 钱包密码，忘记后锁了 11 年，5 BTC（约 40 万美元）；把旧电脑所有文件上传给 Claude，Claude 找到了修改密码之前的旧钱包文件，并发现了 btcrecover 的一个 bug（共享密钥拼接顺序错误）
  - 传播句：`"Just mega dump all of your computers and notebooks into Claude."` ——一句可复制操作指令
- **钩子类型**：**个人奇遇故事式 + 数字反差式**——11 年 × 3.5 万亿次密码尝试 × 40 万美元 × "因为当时嗨了" ——每个数字都是独立冲击点
- **Complication 句型**：`"I've been trying to get in for more than 11 years."` ——时间跨度量化失败规模，比"我一直没成功"强 10 倍；11 年 > 任何情绪描述
- **中段推进**：单线推进（失败定义 → 操作方法论 → 技术细节 → 结果揭晓）；带"意外发现"叙事弧（原以为是密码问题，实为 bug 问题）
- **收尾形态**：CTA 式——`"Just mega dump all of your computers and notebooks into Claude."` ——把极端个人奇遇压缩为人人可复制的操作指令
- **可复用模板**：`"[X 年前] 我 [具体的人类弱点/意外行为] 导致 [有量化价值的东西] 消失了 [X 年]。[时间节点]，我 [极简的 AI 操作，可独立复制]，Claude [具体找到/解决了什么，附技术精确细节]。[一句人人可复制的操作指令]。"`
- **⭐ WHY 中小号能爆**：三重跨圈层引擎——① 加密圈（钱包恢复技术话题）② AI 圈（Claude 技术细节 + btcrecover bug 发现）③ 泛读者（"嗨了忘密码 11 年" 的 humour + 40 万美元的数字）。任何一圈的受众看到都会发给另两圈——这是真正的跨圈层传播结构。关键结构件：**具体人类弱点（stoned，可认同）+ 具体时间损失（11 年，可量化）+ 可复制操作（mega dump，可行动）**，三件同时成立

---

**A-W20-OT-2 · @akshay_pachaar（Akshay，Claude Code 技术科普创作者）2026-05-10**

- **粉丝量**：未验证（账号风格为 Claude Code 技术科普，估计 < 50K；参考：26 replies / 106 RTs / 449 likes / 616 bookmarks）
- **互动量**：26 replies / 106 RTs / 449 likes / 616 bookmarks（**bookmarks > likes = 参考产物型内容的典型信号**）
- **帖子 URL**：x.com/akshay_pachaar/status/2053480693733433797
- **帖子原文（节选）**：`"Claude Code's architecture, mapped. Claude Code is one of the most powerful agent harnesses out there, it's a lot more than 'a CLI that calls claude.' the actual system has six layers, and the model is just one node inside the loop. the diagram breaks down every component:"`
- **钩子类型**：**发现式（架构层 reveal）**——"你以为它是 X（一个 CLI），其实它是 Y（六层系统，模型只是其中一个节点）"——帮读者重新理解已经在用的工具；认知降维打击
- **Complication 句型**：`"it's a lot more than 'a CLI that calls claude.'"` ——用引号引用读者脑子里的旧认知，然后直接打脸。旧认知 vs. 真实架构 = 最干净的 complication 结构，不需要外部事件
- **中段推进**：图表驱动（diagram 替代文字中段，六层架构可视化）——不用文字推进，用视觉推进；W18 Yuchen Jin 的"图表收尾"在这里演化为"图表中段"
- **收尾形态**：无明确收尾；图表自封闭（需要截图保存 = 天然高 bookmark 率）
- **可复用模板**：`"[已知工具]'s [核心机制], mapped. It's a lot more than '[读者的旧认知/简化认知].' The actual system has [N] layers, and [你以为的核心] is just one [节点/组件] inside the loop. [图表]"`
- **⭐ WHY 中小号能爆**：bookmark > like 的比例（616 vs 449）说明内容被当工具书收藏，不是情感消费。传播不靠即时转发，靠**收藏 + 后续场景复发**（开会前翻 → 跟同事分享）。护城河：精确图表作为不可替代的参考产物——文字可以被转述，图表不能不截图地被复制

---

**A-W20-OT-3 · @minchoi（Min Choi，AI 内容创作者）⚠️ W17 · 2026-04-22**

- **粉丝量**：未验证（AI 内容创作账号，估计 < 50K）
- **互动量**：Tom's Hardware、InfoWorld、The New Stack、Medium 多平台覆盖；Pato Molina（Belo 公司 CEO）西班牙语 reply 放大；Axios 在 5 月 14 日后续报道中仍在引用此事；事件详情：Anthropic 的自动系统向 Belo 公司 60+ 名员工同时暂停 Claude 访问，15 小时后因"误报"恢复
- **帖子 URL**：x.com/minchoi/status/2045542832241262602
- **帖子原文**：`"Anthropic shut down an entire company's Claude access overnight. 60+ employees. No explanation. Just an email. Want to appeal? Fill out a Google Form. Integrations gone. Histories gone. Everything built on Claude... gone. Never let one vendor own your workflow."`
- **⚠️ 日期标注**：April 22（W17）；未被 W18 / W19 先前扫描覆盖，首次入库，标注日期
- **钩子类型**：**灾难见证式**——说话人是事件传播者（非当事公司），以第三人称见证 + 第一人称立场组合声索道德高地；不需要是受害者就能发出最有力的谴责
- **Complication 句型**：`"Want to appeal? Fill out a Google Form."` ——把"不公正"的规模通过讽刺句型呈现：60+ 人的企业，申诉渠道是一个 Google 表单。具体细节（Google Form）比"客服态度差"有 10 倍冲击力；讽刺不靠情绪词，靠细节本身
- **中段推进**：三连短句（无中段）——`"60+ employees. No explanation. Just an email. Want to appeal? Fill out a Google Form."` ——每句递进冲击力，节奏感替代论证
- **收尾形态**：**金句 + 原则陈述**——`"Never let one vendor own your workflow."` ——把具体事件升华为普遍规则，帖子超越了新闻生命周期；这句话已经脱离原帖在各种供应商 lock-in 讨论中独立流通
- **可复用模板**：`"[平台/公司] [对 X 人/机构做了 Y 不公正行为]。没有解释。就是一封邮件。想申诉？[具体的荒诞渠道]。[被删除/消失的东西列表]。永远不要让 [一个供应商] 拥有你的 [工作流/数据/资产]。"`
- **⭐ WHY 中小号能爆**：**三连短句 + 讽刺细节 + 普遍金句**三件套——节奏制造愤怒积累，讽刺细节替代情绪词（不说"离谱"，说"Google Form"），金句让帖子有可脱离全文单独传播的单元。话题可转发 + 观点可引用，两件事同时成立

---

#### 本周 X 侧提炼（跨样本 summary）

**本周（5/3–5/17）叙事重心：Claude Code 作为基础设施的双重张力**

本窗口围绕 Anthropic / Claude Code 产生了三个独立但指向同一底层问题的病毒事件：
- 🔒 Access cut（@minchoi，⚠️ W17 补录）：一家公司被无预警断开，申诉渠道是 Google Form
- 🏗️ Architecture revealed（@akshay_pachaar）：Claude Code 不是 CLI，是六层系统
- 🎵 Easter egg（@ClaudeDevs）：`/radio` 是一个藏在产品里的 lo-fi 频道

三条共同反映：Claude Code **既是 60 人公司的工作流依赖，也是待探索的黑箱**——这个张力正在产生持续的内容势能，且方向相反（脆弱性 vs 神秘性）。

同期，@cprkrn 的 Bitcoin recovery 是本周唯一触达非 AI 受众的帖子，也是本月 outlier 爆款质量最高的一条。

| 模式 | 代表样本 | 核心机制 |
|---|---|---|
| **叙事大翻转式（新变体）** | Dario Jevons Paradox | 同一人在不同场合公开翻转自己的核心论点；新场合权威性越高，翻转越有力；争议性反驳成为二次传播收尾 |
| **零解释式发布（新变体）** | @ClaudeDevs /radio | 官方账号发命令零解释；沉默 = 谜面；知识缺口 + 低摩擦验证 = 必须点。是发现式的机构极简版 |
| **个人奇遇 + 可复制操作式（新变体）** | @cprkrn Bitcoin | 具体人类弱点 + 具体时间损失 + 可复制操作指令 = 跨圈层传播三件套；缺一不可 |
| **三连短句 + 讽刺细节 + 金句** | @minchoi Anthropic shutdown | 短句节奏积累愤怒，讽刺细节（Google Form）替代情绪词，金句收尾让帖子超越新闻生命周期 |
| **bookmark 型图表发布** | @akshay_pachaar Claude Code architecture | bookmark > like = 参考产物信号；可视化图表不能被文字复述，强制截图保存 |
| **权威引用压缩式** | @DataChaz "Karpathy was right" | 引用 KOL 预测 + "spoiler: 实际比预测更极端" = 放大者本身有信息增量；适合 mid-tier 账号借力已验证的权威观点 |

**🆕 新钩子变体建议补入 typology：**

> **零解释式发布（Zero-comment Drop）**：发布一个命令 / 链接 / 图表，什么也不说。沉默创造知识缺口，低摩擦的点击/运行验证行为本身就是传播。前提：受众有动机验证（开发者账号 ✅；泛读者账号 ❌）。与"发现式"的区别：发现式有文字解释，Zero-comment Drop 完全依赖读者自行解码。

> **叙事大翻转式（Narrative U-Turn）**：同一人在不同场合公开翻转自己的核心论点。格式：`"他上次说了 [X]；这次他在 [更权威的场合] 说了 [Y]。"` 翻转人知名度越高、原始论点越广为人知，传播倍数越大。争议性的反驳（如 ION Analytics 的 pre-IPO theatre 论）往往成为二次传播收尾，进一步延长帖子生命周期。

> **个人奇遇 + 可复制操作式**：把个人的极端经历（11 年、40 万美元、"当时嗨了"）压缩为一条人人可复制的操作指令（"Just mega dump all of your computers"）。极端经历提供可信度和 entertainment，操作指令提供分享动力（"我要让朋友知道这个"）。两者缺一不可——只有故事没有指令 = 新闻；只有指令没有故事 = 教程。

---

### B · 小红书提炼 · 本周无样本（已跳过）

`raw/viral-samples-xhs/2026-W20.md` 不存在。跳过。

---

### 本周 actionable

1. **测试"零解释式发布"**：如果 Zico 有一个 Claude skill / GitHub gist / 命令行操作想推，考虑只发操作本身，不加说明文字。前提：帖子受众中有相当比例的技术从业者（有 Claude Code 使用上下文）。反例：对泛读者发 `/radio` 会死寂，因为他们没有 Claude Code 上下文。低成本测试方案：先用这个格式在技术受众的帖子下面 reply，观察反应率，再决定是否单独发帖。

2. **"叙事大翻转式"素材雷达**：遇到行业人物公开改变大立场时（AI 会灭掉就业 → AI 会创造就业；vibe coding 是未来 → vibe coding 是反模式），在 24 小时内准备一篇 `"他上次说 [X]，这次他说 [Y]，差别在哪里"` ——不需要判断谁对，对比本身就是价值。Dario 的 Jevons 翻转（5/5）是本周最强素材，但时机已过。**建立监控习惯**，下次不错过。

3. **"三连短句 + 讽刺细节 + 金句"句式加入 Complication 备选库**：@minchoi 的结构（`"No explanation. Just an email. Want to appeal? Fill out a Google Form."`）是本月观察到的最可复制的 complication 句式。适用场景：下一次写"平台/机构做了一件不公正的事"类内容，用这个格式替代情绪化描述：① 量化规模 ② `"No explanation. Just [具体渠道/细节]."` ③ 讽刺性申诉路径 ④ 普遍化金句（`"Never let one X own your Y."`）。

---

## Week 2026-W21 · 自动提炼（2026-05-24）

### 本周信号强度说明

覆盖窗口：2026-05-10 至 2026-05-24（14 天）。X_MANUAL_SAMPLES=no（文件不存在）。XHS_SAMPLES=no（同上）。

**KOL 侧：强**——本窗口内出现两个量级级别的 KOL 事件：Karpathy 加入 Anthropic（5 月 19 日）和 Jack Clark 牛津 Cosmos 讲座（5 月 20 日），两条均可精确日期验证，覆盖范围从开发者社区到主流媒体。

**Mid-tier 侧：弱**——WebSearch + 二级索引（HN、Reddit、ThreadReaderApp）扫描未能找到粉丝数 < 5 万但互动量 > 5K 的可验证 outlier 帖子。原因推断：Karpathy 公告（5/19）在 AI Twitter 上产生了引力井效应——5 月 17–24 期间 AI 空间的注意力高度收束，中小号的有机爆发空间被压缩，且时效过短导致媒体聚合尚未将 mid-tier 反应帖索引完全。附 2 条部分可验证的候选 mid-tier 样本，但日期或粉丝量无法独立确认，以 ⚠️ 标注。

如实汇报：本周可验证样本 2 条 KOL + 0 条完整数据 mid-tier outlier + 2 条部分数据候选。不填充。

---

### A · X 提炼

#### KOL 基线（2 条）

**A-W21-KOL-1 · @karpathy（Andrej Karpathy）2026-05-19**

- **帖子 ID**：x.com/karpathy/status/2056753169888334312
- **量级**：148K likes / 18K RT / 7.8K replies / 14K bookmarks / 约 3M views（首小时内）；TechCrunch、Axios、Fortune、CNBC、VentureBeat 等 10+ 主流媒体同日跟进
- **帖子原文**：`"Personal update: I've joined Anthropic. I think the next few years at the frontier of LLMs will be especially formative. I am very excited to join the team here and get back to R&D. I remain deeply passionate about education and plan to resume my work on it in time."`
- **钩子类型**：🟡 **极简个人硬发布式**——四句话，无背景铺垫，不提 OpenAI，不解释为什么。消息本身就是钩子，没有情绪表演。与 sama 的 BLUF 一句话帖不同：Karpathy 保留了 4 句，但每句都在做结构性工作，不冗余
- **Complication 句型**：`"I think the next few years at the frontier of LLMs will be especially formative."` ——隐性冲突：OpenAI 的名字被故意省略，这个空白比任何指名道姓的解释都更有冲突感；"especially formative" 承载了 "现在这个节点很关键，我做了一个非显而易见的选择" 的全部意思，不说破
- **中段推进**：无中段（4 句线性推进：事实 → 战略判断 → 情绪状态 → 使命延续）
- **收尾形态**：使命延续式——`"I remain deeply passionate about education and plan to resume my work on it in time."` ——把教育使命作为人设锚点，不承诺时间线，轻描淡写；收尾让帖子有了比单纯人事公告更长的生命周期
- **可复用模板**：`"Personal update: [硬事实一句话]. I think [战略判断，不解释理由]. I am [情绪状态] to [新动作]. I remain deeply [使命/价值观] and plan to [继续做的事] in time."` ——关键：第二句的战略判断不对原来的地方做评价；第四句把"未变的那部分"放到收尾，让帖子既完整又有余音
- **备注**：这是 Karpathy 的"三定律发布"——①我去了哪 ②为什么是现在（隐性）③我还是谁。这 4 句话里最值得逆向学习的是他**对 OpenAI 的完全沉默**：不说离开原因，不致谢旧东家，不为新东家过度背书。沉默本身就是最有力的声明，且不给任何媒体摘句的锚点，只剩"加入 Anthropic"这个事实在传播

---

**A-W21-KOL-2 · @importai（Jack Clark，Anthropic 联合创始人）2026-05-20–21**

- **来源**：牛津大学 2026 Cosmos Lecture "Change is inevitable. Autonomy is not."（5/20）+ Axios Behind the Curtain 专访（5/7）+ Anthropic Institute 研究议程（同期公开）+ Time、Channel 4、TechCentral.ie 密集覆盖（5/21–22）
- **量级**：未验证单条 tweet 精确 RT/like 数；媒体覆盖密度（6+ 主流国际媒体在 48 小时内跟进）表明帖子传播触达广泛；Substack @importai note 同期发布，读者群独立传播
- **核心原话（可引用）**：① `"AI will co-produce a Nobel prize-winning discovery within 12 months."` ② `"By the end of 2028, it's more likely than not that we have an AI system where you would be able to say to it: 'Make a better version of yourself.' And it just goes off and does that completely autonomously."` ③ `"Change is inevitable. Autonomy is not."` （讲座标题）
- **钩子类型**：🆕 **级联时间预测式**——不是一个预测，是一个 12 个月 → 18 个月 → 2028 年的时间阶梯，每一级都比上一级更不可想象；读者被逼着在脑中构建一条不可逆的时间线
- **Complication 句型**：`"Change is inevitable. Autonomy is not."` ——标题即 complication：不说"AI 危险"，说"AI 变革是必然的，但 AI 自主性不是——只要我们做对了选择"；把命运感与能动性放在同一个对立句里，前半句认命，后半句给出行动空间
- **中段推进**：单线推进 + 阶梯递进——Nobel（12 个月）→ AI 全自动运营公司（18 个月）→ AI 训练其继承者（2028）→ "智能爆炸"概念从理论进入官方 Anthropic 研究文件
- **收尾形态**：**标签铸造式 + 概念升格式**——`"intelligence explosion"` 从 AI 安全理论圈的边缘词汇，进入 Anthropic Institute 官方研究议程；这个"概念升格"动作本身就是新闻：帖子/讲座不只在说一件事，还在宣告一个词汇的身份变化
- **可复用模板**：`"[领域] 里有一件事 [时间线 A（最近，可信）] 就会发生。接下来 [时间线 B（中期，更大）]。到 [时间线 C（最远，最不可想象）]，[终极论点]. [标题句：X 是必然的，Y 不是.]"`
- **⭐ 结构洞察**：Clark 的"级联时间预测"之所以有传播力，不是因为预测本身正确，而是因为**把三件事绑在同一条时间线上强迫读者 pattern-match**——"这三件事的共同逻辑是什么？"这个问题推动读者去分享帖子。与 W19 @sama "feels like Codex is having a ChatGPT moment"（类比传播）不同，这是**时间线压迫传播**。

---

#### Mid-tier outliers（重点信号）— ⚠️ 本期 mid-tier 侧弱，2 条候选样本，均标注不确定性

**A-W21-OT-1 · @erichustls ⚠️ 日期未验证，约 2026 年 5 月**

- **粉丝量**：未验证（引用来源未提供账号量级；帖子出现在多篇讨论"solo founder AI 商业模式"的文章中）
- **互动量**：未验证精确数字；多篇英文商业博客在 5 月份将其作为 "solo founder $1M ARR" 浪潮的代表案例引用
- **帖子原文（转引，原帖未直接访问）**：`"Sam Altman once said: 'With AI, you could soon start a one-person billion-dollar company.' So I decided to give it a shot and made $914K in one year."`
- **钩子类型**：**借势预言 + 个人验证式**——用 KOL 的预言（Altman）作为钩子，自己作为验证者出现；不需要自己有粉丝基础，借用的是 Altman 的可信度，贡献的是自己的数字
- **Complication 句型**：`"So I decided to give it a shot"` ——把"有人说可以做到"和"我就真的去做了"之间的差距作为 complication；大多数人会点头"对，可以"但不行动，这条帖的冲突是"我不一样"
- **中段推进**：极短（一句话帖，无中段）
- **收尾形态**：数字金句——`"$914K in one year"` 是自封闭的收尾，不需要解释
- **可复用模板**：`"[KOL 名字] 曾说：'[预言]'. 所以我决定试一试，做到了 [具体数字结果]."`
- **⭐ 为什么中小号可能爆**（候选分析）：① 借用了 Altman 的名字作为权威锚点（免费引用权威）；② "gave it a shot" 是最反精英的措辞——不是"我有系统，我有方法论"，而是"我试了试"；③ $914K 不是整数（$1M 太圆，$914K 更可信）。三件事同时成立
- **⚠️ 不确定性**：帖子原文未独立验证，日期未确认在 5/10–5/24 窗口内，粉丝数未验证。此条为候选样本，不计入完整 pattern 库，待下次有 Zico 手动确认后升级

---

**A-W21-OT-2 · @frankdilo（Francesco Di Lorenzo，Typefully 联合创始人）⚠️ 约 2026 年 5 月**

- **粉丝量**：未验证（Typefully 是 X 上 mid-tier 创作者常用的发帖工具，@frankdilo 在创作者/开发者圈有一定知名度，但精确粉丝数未独立确认）
- **互动量**：未验证
- **帖子原文（转引）**：`"More and more drafts are being created while interacting with agents, not typed into our editor by a human."` 同期公告：Typefully 达到 10,000 付费用户，推出 `npx typefully` CLI agent skill
- **钩子类型**：**产品数据式**——用自己产品的用户行为数据作为钩子，不是观点，是观察；说话人是数据的天然持有者，可信度来自数据本身而非账号权威
- **Complication 句型**：无显性冲突句——但 complication 隐含在数据里：你以为用户在用编辑器打字，实际他们在和 agent 对话；工具的使用方式已经悄悄改变了，产品方还没正式宣布这件事
- **中段推进**：极短，无中段（观察 + 产品公告）
- **收尾形态**：产品发布式召唤——`npx typefully` 作为可操作的 CTA
- **可复用模板**：`"越来越多的 [行为 X] 是通过 [新方式 Y] 完成的，而不是 [旧方式 Z]。"` ——用自己产品数据声索一个行为趋势的第一观察者地位，不需要外部权威
- **⚠️ 不确定性**：帖子日期未确认在本窗口内，粉丝数未验证 < 50K。候选样本，待验证

---

#### 本周 X 侧提炼（跨样本 summary）

**本周（5/10–5/24）叙事重心：Anthropic 变成了一个引力场**

三条信号共同指向同一结构：

- 🏃 人才流入：Karpathy 从 OpenAI 加入 Anthropic pretraining 团队（5/19）
- 🧠 概念升格：Jack Clark 在牛津讲座将 "intelligence explosion" 从边缘词汇推入主流话语（5/20）
- 🔧 基础设施信号：Typefully CLI 显示创作工作流已经从"人打字"变为"人与 agent 对话"（5 月，日期待验）

三条都不是关于"AI 又发布了什么新功能"——而是关于 **AI 改变谁/改变什么/改变怎样的速度**。这是本月 X 侧叙事从"产品发布"向"范式迁移"的结构性转变。

| 模式 | 代表样本 | 核心机制 |
|---|---|---|
| **极简个人硬发布式（新变体）** | @karpathy Anthropic | 4 句话：事实 → 判断 → 情绪 → 使命延续；缺席（不提 OpenAI）比存在（解释原因）更有力 |
| **级联时间预测式（新变体）** | @importai Oxford lecture | 12 个月 → 18 个月 → 2028 年阶梯迫使读者 pattern-match；时间线压迫传播而非类比传播 |
| **借势预言 + 个人验证式（⚠️ 候选）** | @erichustls $914K | KOL 预言作为权威锚，自己的数字作为验证；绕过账号权威，直接声索验证者地位 |
| **产品数据式（⚠️ 候选）** | @frankdilo agentic drafts | 自有产品行为数据 = 趋势第一观察者地位；不需要论证，数据本身是 complication |

**🆕 新钩子变体建议补入 typology：**

> **极简个人硬发布式（Minimalist Hard Drop）**：事实 → 判断 → 情绪 → 使命延续，四句不多。最关键的结构件是**缺席**：不提被离开的地方，不解释选择，让读者自己脑补冲突。适用场景：个人工作/立场的重大转变（新工作、新方向、放弃某事）。护城河不是叙述，是**有价值的省略**。

> **级联时间预测式（Cascading Timeline）**：把三个时间点的预测串成一条阶梯（近期可信 → 中期震惊 → 远期不可想象），让读者无法只接受一个而拒绝其他。核心不是预测是否准确，而是**时间线的内部逻辑是否一致**——一致则读者被卷入，不一致则被质疑。适合有充分话语权的场合（研究者、创始人）；中小号移植此格式需要先建立某一维度的具体可信度。

**列表使用说明（W21 再次确认）：**
- Jack Clark 的 12/18/2028 预测在结构上是列表，但以**时间线阶梯**的方式呈现（而非"三个原因"），维持了单线推进的冲击。这个区别微妙但重要：时间线有方向性，"原因列表"是平铺的——前者有节奏，后者像 PPT。

---

### B · 小红书提炼 · 本周无样本（已跳过）

`raw/viral-samples-xhs/2026-W21.md` 不存在。跳过。

---

### 本周 actionable

1. **测试"极简个人硬发布式"的"有价值的省略"机制**：下一次 Zico 有真实的工作/立场转变要宣布，试用 Karpathy 的四句结构：`"个人更新：[硬事实]. [战略判断，不解释理由]. [情绪状态 + 新方向]. [使命延续，用 'I remain' 或 '我仍然']."` 关键测试点：把"为什么"完全删掉，看读者是否自己在 reply 里补上——如果他们在问，说明省略成功；如果没人关心，说明这件事本身值得被关心的前提不成立。

2. **下一篇趋势稿试"级联时间预测式"开头**：把一个你认为会发生的趋势分解为"3 个月内 → 12 个月内 → 3 年内"三层，第一层必须是可信且具体的（否则整条阶梯失去支撑）。不要求三层都有把握——Jack Clark 自己也只是 "60%+ chance"——关键是**三层内部逻辑一致**，读者接受第一层就会被第二层拖入。适合写 "AI 将改变 X 行业" 类内容时作钩子。

3. **建立"概念升格"雷达**：本周 Jack Clark 将 "intelligence explosion" 从 AI 安全理论圈词汇升格为 Anthropic 官方研究文件用词——这个时刻本身就是一篇稿子。未来若有类似"某个 fringe 概念被某个权威机构/人物正式采用"的事件（如某家大公司第一次在年报里用了某个 AI 词汇），在 24 小时内写 "X 这个词刚刚从 [A 圈] 进入了 [B 圈]，这意味着什么"——这类稿子的信息增量很强，且媒体不会写（他们只会报道技术本身，不会报道词汇的社会迁移）。

---

## Week 2026-W22 · 自动提炼（2026-05-31）

### 本周信号强度说明

覆盖窗口：2026-05-17 至 2026-05-31（14 天）。X_MANUAL_SAMPLES=no（文件不存在）。XHS_SAMPLES=no（同上）。

**KOL 侧：中等**——本窗口最显著的叙事引力中心是"双 CEO IPO 翻转节"（5 月 26 日，Altman + Amodei 同一周公开承认对就业预警"pretty wrong"）和 Cognition $1B 融资（5 月 27 日）。Karpathy 加入 Anthropic（5/19）和 Jack Clark 牛津讲座（5/20）已在 W21 记录，本次不重复。Ole Lehmann 的 Andreessen Rogan 总结帖（5/22）在 W21 的 14 天窗口内但 W21 未收录，首次入库，标注日期。

**Mid-tier 侧：弱**——WebSearch + HN + Reddit + ThreadReaderApp 多轮扫描均未找到粉丝数 < 5 万但互动量 > 5K 的独立可验证 mid-tier 爆款帖。本窗口叙事引力场被 Altman/Amodei 双翻转和 Cognition 融资公告压缩；"高密度新闻周"的典型特征：KOL 信号密集，中小号独立爆发空间被挤压。附 1 条 ⚠️ 候选样本（账号粉丝数未独立验证）。如实汇报，不填充。

直接可验证样本：3 条 KOL + 1 条部分数据候选。

---

### A · X 提炼

#### KOL 基线（3 条）

**A-W22-KOL-1 · @sama（Sam Altman）2026-05-26（澳大利亚联邦银行 Accelerate AI 大会，悉尼，视频连线）**

- **量级**：Fortune、Time、Euronews、TechSpot、Yahoo Finance、PYMNTS、Business Magazines 等 10+ 媒体在 24 小时内覆盖；Liberty Daily、NaturalNews 独立评析放大；多家 Substack 分析文章连锁传播
- **原话**：`"I thought there would have been more impact on entry-level white-collar jobs being eliminated by now than has actually happened. I'm delighted to be wrong about this."` / `"pretty wrong on the social and economic implications"`（CBA CEO Matt Comyn 现场对谈，广泛引用）
- **钩子类型**：**叙事大翻转式（Narrative U-Turn）**——同一人，同一议题（AI 灭掉白领工作），在不同场合公开翻转：2025 年全年频繁预警（"entry-level white-collar roles at serious risk"）→ 2026 年 5 月 IPO 前夕（"pretty wrong"）。与 W20 Dario Jevons Paradox 翻转不同：这次是 Altman 亲口说 "I was wrong"，不是隐性重构，是显性承认
- **Complication 句型**：`"I'm delighted to be wrong."` ——"被证伪"的情感被包装成"轻松释怀"；但 IPO 时间线（OpenAI 5 月机密申请上市）是真实的 complication 来源——媒体自动填充了"你为什么恰好在 IPO 前夕变对了"这个问题；Altman 不需要承认动机，读者会代劳
- **中段推进**：无（演讲引用帖，无独立中段）
- **收尾形态**：Fortune 标题式金句——`"Sam Altman and Dario Amodei are both walking back their AI jobs apocalypse prophecies as they eye blockbuster IPOs"` ——第三方媒体标题成为该叙事的真实收尾，帖子生命周期靠争议性解读续命
- **可复用模板**：`"I thought [X] would have happened by now more than it actually has. I'm [反直觉的正面情绪] about being wrong."` ——承认错误 + 正面情绪化 + 故意省略解释原因，让解释权留给读者

---

**A-W22-KOL-2 · @sama + @DarioAmodei 双翻转组合（2026-05-26，Fortune 标题叙事层）**

- **量级**：Fortune 标题直接点名两人（"both walking back"）；Breitbart、HR Executive、MSNBC、Technology Magazine、AI Magazine 等多媒体联动；Fortune 文章本身成为 X 上被广泛转发的 link-tweet 单元
- **帖子形式**：不是两人各自发帖，而是媒体将两件独立事件并列报道，形成的"双翻转叙事"在 X 上以媒体标题截图/link 形式传播——这是本周新观察到的传播机制：**媒体标题本身成为 X 上的病毒传播单元，无需当事人发帖**
- **钩子类型**：🆕 **平行翻转式（Parallel U-Turn）**——当两个顶级 KOL 在同一周（< 7 天内）做出相同方向的立场大翻转，pair 本身比每人单独的翻转更有病毒性：三重巧合（相同行为 + 相同方向 + 相同时机）让读者脑中自动生成"协调"假设，媒体不需要指控，读者自己会说
- **Complication 句型**：Fortune 标题直接构成 complication——`"[A] and [B] are both walking back [X] as they eye [IPO]"` ——两人 + 相同动作 + 相同利益动机，三重并列让"巧合"变成"模式"
- **中段推进**：Fortune 文章提供证据链（原预测原话 → 当前翻转声明 → IPO 时间线 → 数据显示就业实际未大幅变化），读者由标题吸引点入，中段信息自取
- **收尾形态**：开放式——Fortune 文章无结论，由读者 reply/QT 自发生成
- **可复用模板**：`"[A] 和 [B] 在同一周都做了 [X]。[共同的外部动机：IPO/大会/监管]。此前他们各自说了什么：[A 的原话]. [B 的原话]."` ——平行结构 + 触发动机 + 历史存档，比单人报道 virality 强
- **⭐ 结构洞察**：这是样本库中首次捕获到"媒体标题成为 X 传播单元"的完整机制。Fortune/TechCrunch 的标题被截图或 link-tweet，不需要 KOL 独立发帖——媒体叙事成了内容本身。对 Zico 的直接启示：一篇文章若能写出一句"让人觉得不转不行"的标题式断语，这句话本身就是内容，脱离正文也能流通

---

**A-W22-KOL-3 · @itsolelehmann（Ole Lehmann，141.9K followers）2026-05-22（⚠️ 日期在 W21 的 14 天窗口内，但 W21 扫描未收录，首次入库）**

- **帖子 ID**：x.com/itsolelehmann/status/2057909733491937555
- **量级**：584 replies / 2.4K RT / 13K QT / 23K likes（已验证）
- **帖子原文**：`"marc andreessen just went on Rogan and casually dropped a TON of AI alpha. full pod is 3 hours and 20 minutes, but i pulled out his most interesting takes here: 1. AGI is here. he thinks the line was crossed about 3 months ago with the new GPT-5.5, claude 4.6, gemini 3, and grok [...]"`
- **背景**：Marc Andreessen JRE 第 2501 集（2026-05-19，3 小时 26 分钟）。Andreessen 声称 AGI 在约 3 个月前（约 2026 年 2 月）已经跨越阈值；定义为"99% 的情况下，顶级 AI 给出的答案优于他能联系到的世界级专家"
- **钩子类型**：**聚合蒸馏式（Distillation Aggregator）**——"X 说了很多，内容很长，我帮你编号提炼"；时效性是卖点之一（播客上线当天或次日发帖）。区别于 W18b 的 Karpathy "from a ~week ago" 回顾式：这是实时聚合（播客上线同日），不制造信息差，制造的是"节省注意力"价值
- **Complication 句型**：`"casually dropped a TON of AI alpha"` ——"casually"（轻描淡写）× "TON of alpha"（高密度价值信号）的反差构成 complication：正因为"随口就说"而非"高调发布"，你反而不敢错过；低调 + 高信号密度 = 最强 FOMO 触发器
- **中段推进**：列表（编号+逐条展开）——**参考产物型列表**（播客内容汇总），不违反反模式规则；13K QT 远超 2.4K RT（QT/RT 比 = 5x），说明列表格式激活了多线辩论：读者在各自的 QT 里对某条 take 单独展开
- **收尾形态**：开放式——帖子以最后一条 take 结束，没有金句收尾；但 13K QT 说明读者以自己的 QT 充当收尾
- **可复用模板**：`"[知名人物] 刚[出现在某个长格式场合]，随口说了一大堆干货。完整内容 [时长]，但最值得关注的 take 是这些：1. [最反常识的一条]. 2. [第二条，附具体细节]. 3. [带数字锚点的一条]."`
- **备注**：**QT > RT 是罕见信号**——QT/RT = 5x（13K vs 2.4K）通常出现在内容成为辩论场地的帖子里，而非单纯信息传递类。这条帖的高 QT 来自"AGI 是否已经到来"这个本身有争议的核心 take；列表格式把一篇长播客拆成了多个独立辩论触发点

---

#### Mid-tier outliers（重点信号）— ⚠️ 本期 mid-tier 侧弱，1 条候选样本

**A-W22-OT-1 · @ScottWu46（Scott Wu，Cognition CEO）2026-05-27（⚠️ 账号粉丝数未验证）**

- **粉丝量**：未验证（AI coding startup CEO，估计 < 50K；TechCrunch 记者采访报道于 2026-05-29）
- **互动量**：未验证具体 tweet RT/like 数字；融资公告本身由 TechCrunch、The Next Web、The Decoder、TechFundingNews 等 8+ 媒体覆盖（$1B at $26B valuation, May 27）
- **最具病毒性的数字锚点**：`"89% of all code committed at Cognition is now written by Devin — up from 13% in December 2025"` ——5 个月内从 13% → 89%，加速度是冲击点
- **CEO 同期矛盾声明（TechCrunch 2026-05-29）**：`"Scott Wu says AI coding agents shouldn't replace humans"` ——公司产品在做"AI 写 89% 代码"的事，CEO 在说"AI 不应取代人"；这正是"叙事大翻转式"的产品层版本
- **钩子类型**：**数字加速度式 + 叙事内在矛盾式**——加速度（13→89 在 5 个月）制造终态数字无法单独给出的紧迫感；CEO 声明与产品数据的内在矛盾制造了"你信哪个"问题
- **Complication 句型**：`"89% of all code committed at Cognition is now written by Devin. Up from 13% in December 2025."` ——两句话，时序结构，没有修辞，加速度自己说话
- **中段推进**：融资公告 + 内部指标 + CEO 访谈；单线推进（公告 → 数字揭示 → CEO 修正叙事）
- **收尾形态**：真问题（隐性）——公司本身是 AI 取代工程师最彻底的证据，CEO 说的却是"不应取代"；帖子不回答这个矛盾，读者自动问
- **可复用模板**：`"[公司] [X 个月前]，[指标] 是 [低值]. 现在是 [高值]. [公司创始人/CEO] 说：[与数字矛盾的声明]."`
- **⭐ WHY 这个结构有力**：两层矛盾同时出现——① 数字的加速度（13→89 让人问"这会停在哪里"）；② CEO 口头声明与产品数据的反差（让人问"他们自己信吗"）。两层矛盾都不需要作者评价，读者自己完成归因
- **⚠️ 不确定性**：@ScottWu46 粉丝数未独立验证；具体 tweet 的 engagement 数字未确认。候选样本，记录结构分析，待下次验证升级

---

#### 本周 X 侧提炼（跨样本 summary）

**本周（5/17–5/31）叙事重心：IPO 前夕，AI 大厂的"预言翻车季"**

本窗口最强的叙事结构是：多个 AI 大厂领袖在同一周内公开翻转他们过去 12 个月的核心预警叙事（"AI 会灭掉白领工作"），而翻转时机恰好与各公司 IPO 准备期高度重合。外部媒体把两件独立事件打包成"双翻转"叙事，Fortune 的标题本身成为 X 上的病毒传播单元。

| 模式 | 代表样本 | 核心机制 |
|---|---|---|
| **平行翻转式（新变体）** | Altman + Amodei 同周双翻 | 两人相同动作 + 相同时机 + 可识别共同动机 → 读者自动生成"协调"解读；pair 的 virality > 各自之和 |
| **聚合蒸馏式（确认）** | Ole Lehmann Rogan 总结 | 实时聚合长格式内容 → 编号 take list → 13K QT（QT/RT=5x）证明列表触发多线辩论 |
| **数字加速度式（新变体）** | Cognition 13%→89% | 时序两点数字（X 个月前 vs 现在）比终态百分比更有力；加速度激活"这会停在哪里"的焦虑 |
| **媒体标题传播式（新观察）** | Fortune "both walking back" | 第三方媒体标题成为 X 传播单元；无需当事人发帖，标题质量决定 X 传播宽度 |

**🆕 新钩子变体建议补入 typology：**

> **平行翻转式（Parallel U-Turn）**：两个高知名度人物在 7 天内做出相同方向的立场大翻转，pair 本身是钩子，而非各自的转变。句式：`"[A] 和 [B] 在同一周都 [做了 X]。[共同的可识别外部动机]。"` 不需要声称"协调"——读者自己会说。适用条件：两人知名度相当、立场转变方向一致、有可识别的共同外部动机（IPO / 监管 / 市场压力）。

> **数字加速度式（Acceleration Hook）**：不报道终态数字，报道从起点到终态的速度：`"[X 个月前] 是 [低值]。今天是 [高值]。"` 两行，不解释，让读者感受速度。Cognition 的 13%→89% 在 5 个月示范了这个公式——加速度感比终态数字更紧迫，更难被"还不是 100%"的理性化所稀释。这是"数字反差式"的时序变体：数字反差式靠两个同时存在的对比；数字加速度式靠同一指标在时间轴上的运动速度。

> **媒体标题传播式（Headline-as-content）**：第三方媒体的标题本身成为 X 上的病毒传播单元，当事人无需发独立帖。触发条件：标题必须有"让人觉得不转不行"的断语——通常是揭示隐性矛盾（"两人同周翻转"）或命名一个读者已经感受到但没有语言的现象。对内容创作者的启示：写稿时先问"这个标题脱离全文，能在 X 上单独传播吗？"

---

### B · 小红书提炼 · 本周无样本（已跳过）

`raw/viral-samples-xhs/2026-W22.md` 不存在。跳过。

---

### 本周 actionable

- **测试"平行翻转式"素材策略**：下一次在 AI 行业观察到两家公司/两个人同一周做相同的立场转变（同时翻转预测、同时涨价、同时裁员），用 `"[A] 和 [B] 在同一周都 [做了 X]"` 作为开头，合并报道而非分开。平行结构 + 读者自发归因共同动机，是让评论帖超越单一新闻事件生命周期的最短路径。本周 Altman + Amodei 是教科书级示范，但时效已过——下次不错过。
- **"数字加速度式"写法加入开头工具箱**：下一篇有增长数据的稿子，不要直接说"现在是 X%"，改成 `"[时间节点 A]，[指标] 是 [低值]. [时间节点 B]，[高值]."` 两行，无修饰，让速度本身说话。Cognition 的 13→89（5 个月）示范了这个公式——加速度感比终态数字更紧迫，且难被理性化稀释。
- **"聚合蒸馏式"作为降成本发帖策略**：Ole Lehmann 的 Andreessen Rogan 总结帖（23K likes / 13K QT）说明：把长格式内容（播客/演讲/文章）当天压缩成编号 take list，可以绕过自己产出原创内容的门槛。匹配场景：下次有 Lex Fridman/Rogan/Y Combinator 类 AI 播客上线，当天发一条 `"[人名] 刚[出现在某长格式场合]，[时长]。提炼 3 个最反常识的 take：1. [..] 2. [..] 3. [..]"` ——护城河是实时性（同日发）+ 提炼准确度，不是原创洞察。注意：QT/RT 比高说明此格式天然触发多线辩论，适合想要互动率的帖子。
