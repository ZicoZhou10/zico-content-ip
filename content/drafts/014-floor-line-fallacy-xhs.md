# 小红书 Draft #014

**主题**：Karpathy 在 Sequoia Ascent 给了一个时间刻度，中文报道全部跳过了——Vibe Coding 是地板，不是天花板
**平台**：小红书
**状态**：v1
**日期**：2026-05-05
**时效锚点**：2026年4月29日 Karpathy 在 Sequoia Capital 主办的 AI Ascent 2026 炉边对话，4月30日发布博客回顾（karpathy.bearblog.dev）并在 X 推文宣传
**钩子类型**：D 发现式——博客稿中藏着一个中文报道跳过的精确时间刻度，读者可自行验证

---

## 标题候选
A. Karpathy 给了一个时间刻度，中文媒体全部跳过了
B. Vibe Coding 是地板，不是天花板
C. 你以为 Vibe Coding 就是 AI 开发？Karpathy 说那只是入门级

---

## 正文

Karpathy 4 月 30 日在 karpathy.bearblog.dev 发了 Sequoia Ascent 2026 演讲回顾。你自己去读。里面有一个中文报道全部跳过的时间刻度：**2025 年 12 月**。在那个月之前，AI 编码 Agent "basically didn't work"。在那之后，成了他的默认专业工作方式。这是 Karpathy 第一次给 AI 编码能力画出一条精确的时间分割线。

中文媒体的标题都在写"Karpathy 宣布 Vibe Coding 已死"。他说的不是这件事。Karpathy 做了一个更精确的区分：Vibe Coding 提高了地板——任何人都能构建原型。Agentic Engineering 拉高了天花板——专业人员协调多个易错 AI Agent 完成系统工程。**地板和天花板之间的距离，比大多数人以为的要大得多。**

他给了 Agentic Engineer 的具体画像：设计规格说明，监督执行计划，检视 diff，编写测试，创建评估循环，管理权限隔离。注意这些动词。没有一个是"写代码"。

Agentic Engineering 不是"更高级的编程"。是管理一群极快但不可靠的执行者。代码由 Agent 写，但正确性、安全性、品味——Karpathy 的原词——由人负责。

然后他举了自己的例子。menugen：拍餐厅菜单生成食物图片的 App。上线几周后被 Gemini 的原生多模态能力直接吃掉。不是竞品打败了他。是这个 App 品类本身消失了。Karpathy 管这叫 Software 3.0——LLM 把上下文窗口变成程序运行环境，传统 App 的存在理由被釜底抽薪。

我每天用 Claude Code 做产品。写 CLAUDE.md 约束 AI 行为，在多个并行 worktree 里做决策仲裁，设计评估循环验证 Agent 产出——Karpathy 描述的那套，就是我的日常。但我之前没给这件事起过名字，因为我以为这已经是共识了。

他的博客告诉我不是。大多数人还停在 Vibe Coding——对着 AI 说"帮我写个 XX"，接受结果，部署。

我给这个认知差起个名字：**地板线谬误**。

看到 Vibe Coding 让人人都能做 App，就以为 AI 辅助开发的能力边界也在这附近。Vibe Coding 是地板。Agentic Engineering 是天花板。中间隔的不是更多编程技巧，是一整套系统工程思维——管理对象从代码变成 Agent，从确定性执行变成概率性协调。

Karpathy 还说了一句话："You can outsource your thinking, but you can't outsource your understanding。"

**你现在用 AI 的方式，是在地板上，还是在往天花板走？**

---

## 封面方案

**风格**：延续极简高级感
- 主视觉：一栋建筑的剖面图，底层标注"Vibe Coding / 地板"（颜色浅、密度高），顶层标注"Agentic Engineering / 天花板"（颜色深、人少），中间巨大的空白层用虚线标注距离
- 主标题（大字）：地板线谬误
- 副标题：Vibe Coding 是地板，不是天花板
- 角标小字：Karpathy · Sequoia Ascent 2026 · 2026/04/29

## 内页配图建议（图文笔记 3-4 页）

1. **Page 1（封面）**：标题 + 楼层剖面视觉
2. **Page 2**：核心发现卡片——"Karpathy 的时间分割线：2025年12月。之前 AI 编码 Agent 'basically didn't work'。之后成为默认专业工作方式。你去 karpathy.bearblog.dev 自己看。"
3. **Page 3**：对比卡片——左栏"Vibe Coding（地板）：对 AI 说'帮我写个 XX' / 接受生成结果 / 部署"，右栏"Agentic Engineering（天花板）：设计规格说明 / 检视 diff / 编写测试 / 评估循环 / 权限隔离 / 保留正确性、安全性、品味"
4. **Page 4**：结尾金句——"You can outsource your thinking, but you can't outsource your understanding. —— Karpathy" + "你在地板上，还是在往天花板走？"

## 标签

#Karpathy #AI #VibeCoding #AgenticEngineering #地板线谬误 #Software3 #科技洞察 #深度思考 #ClaudeCode #人工智能

## 发布策略

- 发布时间：今天（5月5日）晚 8-9 点，Karpathy 博客发布后 5 天窗口内，中文深度拆解仍为空白
- 搜索流量机会：小红书"Karpathy"、"Vibe Coding"、"AI 编程"关键词有持续搜索量；"Agentic Engineering" 中文搜索近乎空白，有首发定义权；"地板线谬误"为原创概念，可建立搜索锚点
- 自评论建议："补充一个细节：Karpathy 还举了招聘的例子——未来面试不是考算法题，是让候选人现场用 AI Agent 构建完整项目、部署、做安全加固，还要抵御对抗性 Agent 的攻击测试。这就是 Agentic Engineering 的验证标准：不是你能不能让 AI 写出代码，是你能不能在 AI 出错时保住系统。"
