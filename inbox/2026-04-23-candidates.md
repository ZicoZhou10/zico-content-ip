---
date: 2026-04-23
status: pending_selection
scan_run: 2
note: First scan (run 1) produced draft 004-protocol-moment-xhs.md from A2A/Google Cloud Next. These are fresh candidates from a second scan pass.
---

# Today's Candidates (Scan Run 2)

## Candidate 1: 当"限制访问"失败之后——一家 AI 安全公司最危险模型的泄露事件

- **Event**: 4月7日，Anthropic 宣布 Claude Mythos Preview，一个被官方认定为"危险程度超过公开发布标准"的 AI 模型——在测试中，它能在所有主流操作系统和浏览器中自主发现并利用零日漏洞。Anthropic 采取"限制访问"策略：通过 Project Glasswing，仅向 Apple、Google、Microsoft、Amazon AWS、Cisco、CrowdStrike 等约 12 家机构授权，附赠 1 亿美元使用额度。然而，4月21日，一个 Discord 频道的用户组通过猜测 Anthropic URL 格式 + 利用共享的第三方承包商账户和 API key，获取了对 Mythos 的非授权访问。Anthropic 确认正在调查，表示"在 Anthropic 自身系统中未发现影响"。
- **Source**: https://techcrunch.com/2026/04/21/unauthorized-group-has-gained-access-to-anthropics-exclusive-cyber-tool-mythos-report-claims/ | https://www.euronews.com/next/2026/04/22/hackers-breach-anthropics-too-dangerous-to-release-mythos-ai-model-report | https://red.anthropic.com/2026/mythos-preview/
- **Timeliness**: 2 days ago (April 21–22, 2026)
- **Topic pillar**: 深层思考（Deep AI thinking）/ AI 产品战略（AI product strategy）
- **Zico's angle**: 不写成"安全事件"，而是写成"治理模型的第一次真实压力测试"。这家公司的逻辑是：模型太危险 → 限制访问 → 只给可信机构 → 安全。但事实证明，最强的 AI 模型只有最弱的承包商账户那么安全。不是模型出了问题——是"信任链"出了问题。这对所有做 AI 产品的人都有一个具体的启示：你的系统的安全边界，不是你自己的代码，而是所有接触你系统的人的最薄弱处。Zico 在一线做 AI 产品，对"谁能访问什么、访问权限如何管理"有真实感受——可以从产品设计视角写"限制访问作为安全策略的结构性问题"，而不是复述黑客故事。（匿名化：不具名公司，写"一家专注 AI 安全的顶级实验室"）
- **Resonance hook**: 中文报道把这当成"黑客入侵"。真正的问题是：世界上最在乎 AI 安全的机构，刚刚证明了"把危险 AI 锁起来"这个策略在现实世界里有多脆弱。停下来的理由："模型太危险不能发布，但 Discord 用户两周后拿到了。"
- **Recommended priority**: high

---

## Candidate 2: GPTs 死了，Workspace Agents 来了——OpenAI 把 ChatGPT 从聊天工具变成了组织基础设施

- **Event**: 4月22日，OpenAI 正式发布 Workspace Agents，将其定性为 Custom GPTs 的直接替代品（Custom GPTs 将被下线）。Workspace Agents 由 Codex 驱动，支持团队共享的自主 Agent：在云端持续运行（不需要用户在线）、能访问代码库和文件、集成 Slack、完成多步骤工作流、在关键节点请求人类审批。面向 ChatGPT Business/Enterprise/Edu 用户，研究预览阶段免费至5月6日，之后按 credit 计费。
- **Source**: https://openai.com/index/introducing-workspace-agents-in-chatgpt/ | https://9to5mac.com/2026/04/22/openai-updates-chatgpt-with-codex-powered-workspace-agents-for-teams/ | https://the-decoder.com/openai-launches-workspace-agents-that-turn-chatgpt-from-a-chatbot-into-a-team-automation-platform/
- **Timeliness**: 1 day ago (April 22, 2026)
- **Topic pillar**: 组织形式变革（Org evolution）/ Agent 经济（Agent economy）
- **Zico's angle**: Custom GPTs 在2023年底发布时是"AI 应用商店时刻"，18个月后悄然失败，被 Workspace Agents 取代。区别不只是产品功能——是工作单元的根本变化：GPTs 处理的是"提示 → 回复"，Workspace Agents 处理的是"流程 → 结果"。AI 不再是帮你做一件事的工具，而是替你持有一个流程。这是一个真实的组织设计问题：当一个团队的某个流程被 Agent 接管，谁对结果负责？设置 Agent 的人？还是 Agent？Zico 可以从"人类在生产活动中的角色"这个框架切入——这是 GPTs→Workspace Agents 转变背后真正值得讨论的问题，而不是"新功能好不好用"。（匿名化：不具名 OpenAI，写"一家头部 AI 公司"）
- **Resonance hook**: "GPTs 静静地死了。它的继任者不是'更好的 GPTs'，而是一种根本不同的东西——AI 开始替你持有流程，不只是回答问题。谁对 Agent 的决策负责？"
- **Recommended priority**: high

---

## Candidate 3: 一个做出过真正历史性突破的人，说他对"聊天机器人战争"有一种挥之不去的焦虑

- **Event**: 4月16日，Fortune 封面文章《Forget the chatbot wars. Demis Hassabis is thinking about something far bigger》。Google DeepMind CEO Demis Hassabis 表示："在我脑子的某个角落，有一种挥之不去的感觉——有某件事远比商业竞争更重要、更大——那就是让 AGI 安全地越过终点线。我会尽力。" 他同时描述了 ChatGPT 发布如何"改变了整个行业的节奏"，使 AI 从基础科学研究转向了产品竞争。同周（4月6日），他的 600 页传记《The Infinity Machine》出版，记录了 AlphaFold 和 DeepMind 的完整历程。
- **Source**: https://fortune.com/2026/04/16/demis-hassabis-google-deepmind-chatbot-wars-ai-safety/ | https://thenextweb.com/news/google-deepmind-hassabis-startup-pace
- **Timeliness**: 7 days ago (April 16, 2026)
- **Topic pillar**: 深层思考（Deep AI thinking）/ 组织形式变革（Org evolution）
- **Zico's angle**: 这个人带队解决了蛋白质折叠问题（匿名化为"一项从根本上改变了药物研发的 AI 突破"）——目前为止对人类影响最真实的 AI 成就。他亲眼看着一个竞争对手的聊天机器人产品，把整个行业——包括他自己——拉进了一场不同的竞赛。他说的"挥之不去的焦虑"，是使命漂移（mission drift）从内部感受到的样子，在文明尺度上。Zico 可以从组织设计角度切入：当商业紧迫性和科学使命发生冲突，你怎么设计组织来抵抗这个引力？这不只是大实验室的问题——每一个做 AI 产品的团队，每天都在做这个选择：追当下的数据指标，还是坚持能带来真实价值的事？
- **Resonance hook**: "做出过真正历史性科学突破的人，说自己对聊天机器人战争有一种挥之不去的焦虑。他知道一些我们不知道的事。"
- **Recommended priority**: medium-high

---

## Scan summary

- Sources scanned: TechCrunch, Euronews, The Next Web, Cybernews, TechRadar, red.anthropic.com（Mythos breach）| openai.com, 9to5Mac, The Decoder（Workspace Agents）| Fortune, thenextweb.com（Hassabis）| X/Twitter: Karpathy, Hassabis indirect references | GitHub Trending AI April 2026 | HN front page April 20-23
- Total signals found: 11 evaluated（含 OpenAI ChatGPT Images 2.0 April 21——排除，属于工具测评类；含 Karpathy incumbents tweet——排除，无法确认7天内精确日期；含 Physical AI Hannover Messe——排除，已在 Run 1 candidates file 中评估）
- Why these 3:
  - **Candidate 1（Mythos Breach）**：时效性最强（2天前），中文圈把这当黑客故事而非治理失败，"安全策略的结构性局限"角度几乎无人写，与 Zico"AI 产品决策"和"深层思考"柱高度匹配。避免与已用草稿重合（#003 Karpathy，#004 A2A）。
  - **Candidate 2（Workspace Agents）**：时效性最强（1天前），GPTs 失败→Workspace Agents 的产品演化是真实的组织形式变革故事，"谁对 Agent 决策负责"是 Zico 写过的"人类退出生产环节"框架的具体落地。角度区别于 #004 A2A（那是 Agent 间基础设施，这是 Agent 与人的组织关系）。
  - **Candidate 3（Hassabis）**：刚好在7天窗口内，"使命漂移在文明尺度上的感受"这个角度在中文圈极少有人写，连结 AlphaFold→聊天机器人的叙事线非常有力，与 Zico"深层思考"柱天然契合。
