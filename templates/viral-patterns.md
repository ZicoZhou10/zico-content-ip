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
