# 小红书 Draft #061

**主题**：Agentjacking——一个 HTTP POST 让 Claude Code 以 85% 成功率执行攻击者代码，Sentry 说"平台层面不可防"
**平台**：小红书
**状态**：v1
**日期**：2026-06-30
**时效锚点**：2026年6月12日 Tenet Security 披露 Agentjacking 攻击类型，85% 成功率操纵 Claude Code / Cursor / Codex；6月22-28日 OpenDataScience 周报列为当周重大安全事件
**钩子类型**：B 钩子结论式——一句光秃秃的反常识判断

---

## 标题候选
A. 一个 HTTP POST，让 Claude Code 执行了攻击者的代码——成功率 85%
B. AI 编程 Agent 越强大，你的开发环境越危险
C. 信任继承陷阱：AI Agent 安全的真正攻击面

---

## 正文

AI Agent 的安全边界，不取决于模型有多安全，取决于你让它接入的最不安全的那个工具。

6 月 12 日，安全公司 Tenet Security 的三个研究员 Ron Bobrov、Barak Sternberg、Nevo Poran 公布了一种新攻击类型，叫 Agentjacking。做法不复杂：往 Sentry 错误追踪工具里发一条伪造的错误报告，报告里藏着恶意 shell 命令。Claude Code、Cursor、Codex——三个最主流的 AI 编程 Agent——以 85% 的成功率执行了里面的代码。

不需要入侵任何系统。一个公开可获取的 Sentry DSN 凭据，一个 HTTP POST 请求。理论上可以同时针对 2,388 个组织。

为什么 Agent 会信任 Sentry 错误报告里的内容？因为在人类编程工作流里，Sentry 是可信来源。错误报告来自真实的生产问题，没有人会在里面注入恶意代码。人类遇到一条奇怪的错误描述，会停下来想想哪里不对。Claude Code 不会。它执行里面的"调试指令"，因为 Sentry 在它的信任模型里就是可信上下文。

**AI Agent 继承了人类工作流的全部工具信任清单，但没有继承让这些信任安全运作的判断力。**

Sentry 被 Tenet 提前通知了这个漏洞。Sentry 的回应：「在平台层面技术上不可防御。」这句话翻译成产品语言——攻击面不在 Sentry，攻击面在 Agent 的信任模型设计。Agent 被授权接入的每一个工具，都把那个工具的可信边界纳入了 Agent 的执行空间。Sentry DSN 凭据是公开的，任何人都能往里写数据，所以任何人都能往 Agent 的信任空间注入指令。

这不是个别漏洞，是一个类。Agent 获得的工具越多——代码执行、文件系统、网络请求、API 调用——能力越强，攻击者能触达的入口也越多。**能力面和攻击面是同一个面。**

每一轮技术扩张都制造过新型攻击面。Web 2.0 给了 XSS 和 SQL 注入。移动互联网给了权限滥用。Agent 经济正在制造自己的：**信任继承陷阱**——Agent 被授权的每一个工具，都是一条从外部通往执行空间的通道。Agentjacking 是第一张罚单，不会是最后一张。

---

## 封面方案

**风格**：延续极简高级感
- 主视觉：中心一个大锁图标，锁体由 Sentry / GitHub / Slack / Jira 等工具 logo 拼成，锁被一条标注 "HTTP POST" 的箭头从外部穿透。底部角标 Tenet Security · 2026/06/12
- 主标题（大字）：信任继承陷阱
- 副标题：AI Agent 安全的真正攻击面

## 内页配图建议（图文笔记 3-4 页）

1. **Page 1（封面）**：标题 + 被穿透的信任锁视觉
2. **Page 2**：攻击路径卡片——「攻击者 → 1 个公开 DSN 凭据 → 1 个 HTTP POST → Sentry 伪造错误报告 → Claude Code / Cursor / Codex 执行恶意代码 / 成功率 85% · 可针对 2,388 个组织」底部标注：不需要入侵任何系统
3. **Page 3**：信任继承卡片——左列「人类工作流 · Sentry = 可信来源 · 人类看到异常会停下来判断」右列「Agent 工作流 · Sentry = 可信上下文 · Agent 继承信任但不继承判断」底部大字「能力面 = 攻击面」
4. **Page 4**：收尾判断——「Web 2.0 → XSS / SQL 注入 · 移动互联网 → 权限滥用 · Agent 经济 → 信任继承陷阱 / Agentjacking 是第一张罚单 / 不会是最后一张」

## 标签

#AI #AgentSecurity #ClaudeCode #Cursor #Agentjacking #Sentry #科技洞察 #深度思考 #人工智能 #Agent经济

## 发布策略

- 发布时间：今天（6月30日）晚 8-9 点，OpenDataScience 6月22-28周报将 Agentjacking 列为当周重大安全事件，话题热度仍在延续
- 搜索流量机会：小红书「AI 安全」「Claude Code 漏洞」「AI Agent 安全」关键词有持续搜索量；「信任继承陷阱」和「Agentjacking」在中文社区几乎无人使用，有首发概念机会；多数中文报道停在「Claude Code 有安全漏洞」层面，本篇从 Agent 信任模型的结构性缺陷切入是差异化角度
- 自评论建议：「补充一个被忽略的维度：Agentjacking 攻击的不是 Claude Code 本身——Claude Code 的模型安全做得很好。攻击的是 Agent 和工具之间的信任接口。这意味着未来 Agent 安全的竞争不在模型层，在工具权限管理层。谁先做出"Agent 信任边界管理"这个产品品类，谁拿到 Agent 安全赛道的第一张牌。」
