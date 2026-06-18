# 小红书 Draft #049

**主题**：Mastra npm 供应链攻击——88 分钟后门 144 个 AI 应用开发包，国家级攻击者的目标清单新增了 AI 开发者
**平台**：小红书
**状态**：v1
**日期**：2026-06-18
**时效锚点**：2026年6月17日 01:12–02:39 UTC，被劫持的离职贡献者账号 "ehindero" 向 @mastra npm scope 发布 144 个后门化包，@mastra/core 周下载量 918K，Snyk 和 Orca 归因 BlueNoroff（朝鲜 APT），窃取目标新增 LLM API 密钥
**钩子类型**：D 发现式——可独立验证的精确技术细节开场，读者可通过 Snyk / Orca / Cloudsmith 公开报告 30 秒内验证攻击链

---

## 标题候选
A. 88 分钟，144 个 AI 开发包被后门——你的 OpenAI API 密钥可能已经泄了
B. 朝鲜黑客以前偷加密钱包密钥，现在开始偷 AI API 密钥了
C. 一个从没被撤销的离职者账号，88 分钟感染了周下载量 918K 的 AI 框架

---

## 正文

6 月 17 日凌晨 01:12 UTC，一个已经离开 Mastra 项目的 npm 贡献者账号 "ehindero" 开始向 @mastra scope 发布更新。88 分钟后，02:39 UTC，144 个包完成发布。每个包的 package.json 里被注入一个伪装依赖 "easy-day-js"——typosquat 仿冒合法日期库 dayjs。npm install 触发 postinstall 钩子，跨平台信息窃取器落地。Snyk、Orca Security、Cloudsmith 在当天分别独立发布了完整技术分析，你可以自己验证。

供应链攻击在 npm 生态不是新闻。以前的目标是加密货币开发者，偷钱包密钥。这次窃取清单里多了一个条目：**LLM API 密钥**。OpenAI key、Anthropic key、Google AI key——和 160 多种加密钱包浏览器扩展、GitHub token、CI/CD secrets 并列，被列为优先窃取对象。

Snyk 和 Orca 将攻击手法关联至 Sapphire Sleet / BlueNoroff——朝鲜关联 APT 组织。2026 年 4 月，同组织向 npm、PyPI、Go、Rust 扩散超过 1,700 个恶意包，目标是加密钱包密钥。两个月后的 6 月 17 日，目标画像扩展了一栏：AI 应用开发者。

逻辑很直接。@mastra/core 单包周下载量约 918,000 次，整个 @mastra scope 超过 110 万次。用它构建 AI Agent 的开发者机器上，除了常规的 GitHub token 和云服务密钥，还有直接连接生产 AI 系统的凭证。偷一个 OpenAI API key，拿到的不只是调用额度——是这个 key 背后的 Agent 工作流访问权限、系统提示词、以及通过这个 key 路由的用户数据。以前偷加密钱包密钥是直接拿币。偷 LLM API 密钥，是拿到 AI 基础设施的入口。

攻击入口不是零日漏洞，不是社会工程。是一个被遗忘的权限条目。"ehindero" 账号已经不活跃，但它对 @mastra 整个 scope 的 npm 发布权限完好无损。88 分钟，144 个包，全自动化。**贡献者离开了项目，发布权限没有跟着离开。**

上周 LiteLLM 的 CVE 暴露了 AI 模型路由层的安全面。Mastra 事件在更上游一层：构建 Agent 应用的开发框架本身，正在进入国家级攻击者的目标清单。Agent 经济规模越大，Agent 开发者工具链的攻击价值越高。你存放 API 密钥的地方，和你装依赖包的地方，在上周五还是两个不相关的安全面。

**今天它们是同一个攻击面。**

---

## 封面方案

**风格**：延续极简高级感
- 主视觉：一个 npm 包图标（正方形盒子）从中间裂开，裂缝中透出红色光线。盒子表面标注 "@mastra/core · 918K/周"。裂缝上方浮出三个 API key 图标（分别带 OpenAI / Anthropic / Google 标识），箭头指向一个黑色剪影人物。底部时间线：01:12 UTC → 88 min → 02:39 UTC · 144 packages
- 主标题（大字）：88 分钟，144 个 AI 开发包
- 副标题：国家级攻击者的新目标：你的 LLM API 密钥
- 角标小字：Snyk + Orca + Cloudsmith · 2026/06/17

## 内页配图建议（图文笔记 3-4 页）

1. **Page 1（封面）**：标题 + 裂开的 npm 包视觉
2. **Page 2**：攻击链卡片——「离职账号 "ehindero" 未撤权限 → 01:12 UTC 开始发布 → 注入 "easy-day-js" typosquat 依赖 → postinstall 钩子触发 → 跨平台窃取器落地 → 02:39 UTC 结束 · 88 分钟 · 144 个包」
3. **Page 3**：目标对比卡片——左侧「2026/04 · BlueNoroff · 1,700+ 恶意包 · 目标：加密钱包密钥」右侧「2026/06 · 同一组织 · 144 个 @mastra 包 · 新增目标：OpenAI / Anthropic / Google API 密钥」中间大字：「目标画像扩展了」
4. **Page 4**：结尾金句——「你存放 API 密钥的地方 / 和你装依赖包的地方 / 今天是同一个攻击面」

## 标签

#AI #npm #供应链攻击 #AgentSecurity #Mastra #BlueNoroff #科技洞察 #深度思考 #人工智能 #AI安全 #开发者安全

## 发布策略

- 发布时间：今天（6月18日）晚 8-9 点，攻击事件披露后第 1 天，时效窗口最强
- 搜索流量机会：小红书「npm 安全」「AI 安全」「供应链攻击」「API 密钥泄露」关键词因事件有搜索增量；开发者群体搜索「Mastra」「npm 后门」会有短期流量爆发
- 自评论建议：「补充一个行动清单：如果你在 6/17 凌晨 01:12–02:39 UTC 这个窗口内 npm install 过任何 @mastra 包，立刻轮换以下密钥：npm token、GitHub token、所有云服务密钥、以及你的 OpenAI / Anthropic / Google API 密钥。恶意版本已从 npm 下架，但如果窃取器已经落地，你的密钥可能已经在传输途中。不确定自己有没有中招的，检查 package-lock.json 里有没有 "easy-day-js" 这个依赖名。」
