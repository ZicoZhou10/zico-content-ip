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
