# 小红书 Draft #035

**主题**：微软在 Build 2026 自研模型替换 GPT-4 Turbo，并点名 Claude Code 为对手——AI 编程工具的真正护城河不在产品层，在模型主权
**平台**：小红书
**状态**：v1
**日期**：2026-06-02
**时效锚点**：2026年6月2日 Microsoft Build 2026 开幕，Satya Nadella 宣布 Project Polaris 自研 AI 编程模型从8月起替换 GitHub Copilot 中的 GPT-4 Turbo，发布会上点名 Claude Code 为竞争对手
**钩子类型**：C 反共识自白式——"我以前以为 X，今天改了看法"，认知翻转驱动

---

## 标题候选
A. 微软点名要干掉 Claude Code——但真正的信号不是竞争
B. AI 编程工具的护城河不在产品层，微软今天证明了
C. 你用的 AI 工具，模型是谁的？

---

## 正文

我以前以为 AI 编程工具的护城河在产品层——上下文窗口多大、Agent 模式多聪明、IDE 集成多丝滑。今天改了看法。

不是因为 Project Polaris 的 benchmark 数字好看。是因为 Satya Nadella 在 Build 2026 发布会上点名了 Claude Code——这是主流 AI 工具厂商第一次在产品发布会上公开指定一个创业公司的产品为"要干掉的对手"。万亿市值的公司不会在自己年度大会上无端命名竞争者。除非数据已经很难看。

6 月 2 日，Microsoft Build 2026 开幕。Polaris 是微软自研 AI 编程模型，混合专家架构（Mixture-of-Experts），HumanEval 和 MBPP benchmark 优于 GPT-4 Turbo，运行在 Azure 自研 Maia 加速器上，8 月起替换 GitHub Copilot 的默认推理引擎。

但替换 GPT-4 Turbo 的原因不只是性能。

两周前的一个细节：微软 Experiences & Devices 部门——管 Windows、Office、Teams、Surface 的——因为工程师用 Claude Code 用量超标，取消了大量 Claude Code 许可证。做 Copilot 的公司，自己的工程师在 Copilot 旁边用竞品完成工作。

这是 revealed preference。不需要看 benchmark，看人用脚投票就够了。

GitHub Copilot 在 OpenAI 模型上构建了四年。今天这个替换是微软主动做的。但如果 OpenAI 先动——调价、改接口、收回授权？四年的 Copilot 生态被架空。Polaris 首先解决的不是 Claude Code 的威胁，是对 OpenAI 的模型依赖。

很多 AI 产品团队还没意识到这个问题的本质：**当你的产品建在别人的模型上，你不是在做产品决策——你是在别人的产品决策之外活着。**

这就是**模型寄生**。Cursor 寄生在 Anthropic 和 OpenAI 上。Copilot 过去四年寄生在 OpenAI 上。Windsurf 寄生在多家上。表面是产品竞争——上下文窗口、Agent 模式、IDE 集成。底层问题是：你用谁的大脑？大脑的主人一个电话就能改写你的 roadmap。

微软的选择是：不再寄生。自研模型 + 自研芯片，训练到推理全链路可控。同场宣布的 Windows Agent Store 给开发者 85% 分成——App Store 是 30%。不是慷慨，是在 Agent 生态最早的窗口用分成倒贴卡住分发入口。

**微软今天做了一个判断：在别人模型上包产品不是长期策略。开发者工具的战争已经输了一局，需要自研模型才能扳回来。**

这个判断对所有正在做 AI 产品的人都成立。你现在用的 AI 工具，它的模型是谁的？**如果你的核心能力建在一个 API call 上，你的护城河就是一个 API key。**

---

## 封面方案

**风格**：延续极简高级感
- 主视觉：左侧 GitHub Copilot logo 上方标注 "GPT-4 Turbo" 被一条红色删除线划掉，右侧 Project Polaris logo 标注 "自研模型"。下方一行小字："同一天，微软点名了 Claude Code。" 背景深色
- 主标题（大字）：模型寄生
- 副标题：你的 AI 工具，用的是谁的大脑？
- 角标小字：Microsoft Build 2026 · 2026/06/02

## 内页配图建议（图文笔记 3-4 页）

1. **Page 1（封面）**：标题 + 替换视觉
2. **Page 2**：核心事实卡片——「6月2日 Build 2026 / Project Polaris：自研 AI 编程模型 / 8月起替换 GPT-4 Turbo / 发布会点名 Claude Code 为竞争对手 / 两周前：微软自己的工程师因 Claude Code 用量超标被取消许可证」
3. **Page 3**：模型寄生结构图——上方「产品层竞争（表面）：上下文窗口 / Agent 模式 / IDE 集成」下方「模型层依赖（底层）：Cursor → Anthropic+OpenAI / Copilot → OpenAI（→ Polaris）/ Windsurf → 多家」中间标注：「大脑的主人一个电话就能改写你的 roadmap」
4. **Page 4**：结尾金句——「在别人模型上包产品不是长期策略。/ 如果你的核心能力建在一个 API call 上，/ 你的护城河就是一个 API key。」

## 标签

#AI #Microsoft #Build2026 #Copilot #ClaudeCode #AI编程 #科技洞察 #深度思考 #人工智能 #模型寄生 #AI产品

## 发布策略

- 发布时间：今天（6月2日）晚 8-9 点，Build 2026 开幕当天，时效性最强窗口
- 搜索流量机会：小红书「Microsoft Build」「GitHub Copilot」「AI 编程」「Claude Code」关键词因今日发布会有搜索增量；「模型寄生」为原创概念标签，有长尾搜索占位价值
- 自评论建议：「补充一个角度：微软同场宣布的 Windows Agent Store 也值得注意。85% 开发者分成，Adobe 和 Zoom 已签约。App Store 用 30% 分成花了 15 年成为基础设施。微软今天在 Agent 生态最早的窗口里用分成倒贴——不是因为 Agent 生态现在能赚钱，是因为谁先建立 Agent 分发渠道，谁就拿到接下来五年的流量入口。这和 Polaris 的逻辑一样：先卡位，再收割。」
