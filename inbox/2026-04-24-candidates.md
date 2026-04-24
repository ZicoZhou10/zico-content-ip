---
date: 2026-04-24
status: written
selected: candidate 1 → drafts/005-workflow-embedding-xhs.md
---

# Today's Candidates

## Candidate 1: 某 AI 公司用一个开发者工具超越了行业老大——但这才是真正有意思的事

- **Event**: Anthropic 在 4 月初 ARR 突破 300 亿美元，首次超过 OpenAI（约 250 亿美元）；4 月 23 日，Anthropic 在二级市场估值达到 1 万亿美元，超越 OpenAI（约 8800 亿）。驱动这次超越的核心产品：Claude Code——2025 年中公开发布，6 个月内 ARR 达 10 亿美元以上，客户结构 80% 为企业，年消费超过 100 万美元的企业客户在不到 2 个月内从 500 家增至 1000 家以上。Anthropic 同期训练成本是 OpenAI 的四分之一。
- **Source**: https://www.saastr.com/anthropic-just-passed-openai-in-revenue-while-spending-4x-less-to-train-their-models/ | https://finance.yahoo.com/markets/stocks/articles/anthropic-just-overtook-openai-1-155312239.html | https://www.the-ai-corner.com/p/anthropic-30b-arr-passed-openai-revenue-2026
- **Timeliness**: 1 day ago（估值超越：4 月 23 日；收入超越：4 月 7 日，17 天前）
- **Topic pillar**: AI 产品战略
- **Zico's angle**: 大家讨论这件事都在说"谁更厉害"。但真正值得拆解的是：某 AI 公司靠什么超越对手的——是一个开发者编码工具，6 个月做到 10 亿美元 ARR，80% 来自企业，客户留存极高。这不是 toC 产品逻辑，是基础设施逻辑。开发者用了 6 个月，肌肉记忆就形成了。更反直觉的是：这家公司的训练成本是对手四分之一，却做出了更快的增长——意味着它不是靠算力堆出来的，是靠产品形态赢的。一个编码工具成为历史上增长最快的企业软件，这背后的产品策略值得仔细看。
- **Resonance hook**: 中文媒体大量报道"估值超越"，但几乎没有人认真分析"为什么是一个代码工具，而不是旗舰大模型，成了真正的增长引擎"。这个角度在中文圈是空白。
- **Recommended priority**: high

---

## Candidate 2: Agent 之间的互联网正在形成——一个协议悄悄连接了 150 家公司的生产系统

- **Event**: Google Cloud Next 2026 在拉斯维加斯举行（4 月 22-24 日），Google 展示了 Agent2Agent（A2A）协议 v1.2 的最新进展：已有 150+ 家组织在生产环境中运行（非试点），协议治理权移交 Linux Foundation 旗下的 Agentic AI Foundation。微软、AWS、Salesforce、SAP、ServiceNow 均已接入。核心能力：Salesforce 上的 Agent 可以把任务转交给 Google Vertex 上的 Agent，再由后者查询 ServiceNow 的 IT Agent——三套系统之间无需任何定制集成代码。同期 Google 还发布了 Workspace Studio（企业 Agent 定制平台）和 ADK（Agent Development Kit，已获 8200+ stars）。A2A 与 Anthropic 的 MCP 互补：MCP 解决 Agent-to-Tool，A2A 解决 Agent-to-Agent。
- **Source**: https://thenextweb.com/news/google-cloud-next-ai-agents-agentic-era | https://cloud.google.com/blog/products/ai-machine-learning/agent2agent-protocol-is-getting-an-upgrade | https://stellagent.ai/insights/a2a-protocol-google-agent-to-agent
- **Timeliness**: 2 days ago（Google Cloud Next 会议：4 月 22-24 日，正在进行中）
- **Topic pillar**: Agent 经济
- **Zico's angle**: 大多数人讨论 Agent 的时候，焦点还在单个 Agent 能做什么。但当前更重要的变化是另一层：Agent 之间怎么协作。某大厂年度开发者大会上展示的协议，实质上在做一件事：搭建"Agent 之间的互联网"。HTTP 解决了人类的网页互访，这个协议解决的是不同公司系统里的 Agent 之间的任务流转。当 150 家公司的生产系统都跑在同一个协议上，这不再是实验——这是基础设施的形成时刻。更有意思的是：两家竞争关系明显的公司，一家负责 Agent-to-Tool 协议，另一家负责 Agent-to-Agent 协议，两者被迫变成互补关系。Agent 经济的基础设施层，正在以一种没人提前预测到的合作-竞争方式形成。
- **Resonance hook**: 中文 AI 圈热议"Agent 能干什么"，但 Agent 之间怎么互通、哪家公司在主导基础设施标准——这个层面几乎没有中文内容在追踪。
- **Recommended priority**: high

---

## Candidate 3: 有一种 Agent 在悄悄进化——每解决一个任务，它就变得更强

- **Event**: 4 月 21 日，arXiv 发布论文"GenericAgent: A Token-Efficient Self-Evolving LLM Agent via Contextual Information Density Maximization"（作者 lsdefine 等）。GitHub 仓库 lsdefine/GenericAgent 在 4 月 22 日 GitHub Trending 周榜中进入头部。核心机制：Agent 从 3300 行种子代码出发，每次成功解决任务后，将执行路径"结晶"为一个可复用技能，持续积累形成个人技能树。实测：消耗 token 数量仅为基线的六分之一，同时实现完整系统控制能力。与此同时，同期 GitHub Trending 还有 NousResearch 的 hermes-agent-self-evolution（DSPy + GEPA 框架做 Agent 自我优化）和 sentient-agi 的 EvoSkill（从失败轨迹中提炼可复用技能），形成"自进化 Agent"的整体趋势。
- **Source**: https://github.com/lsdefine/GenericAgent | https://www.shareuhack.com/en/posts/github-trending-weekly-2026-04-22 | https://pyshine.com/GenericAgent-Self-Evolving-AI-Agent/
- **Timeliness**: 3 days ago（arXiv 论文：4 月 21 日；GitHub Trending：4 月 22 日）
- **Topic pillar**: 深层思考（与 Agent 经济交叉）
- **Zico's angle**: 我们现在用的绝大多数 Agent 是无状态的——每次调用从零开始，用完即忘。GenericAgent 的设计哲学不同：它每解决一个新任务，就把执行路径结晶成一个技能，下次遇到类似情境直接调用。它在积累。这和"工具"的本质区别是：工具不会因为被用而变得更好用。但这种 Agent 会。更准确的说法不是"AI 工具进化了"，而是：某类系统开始表现出生命体才有的特征——经验积累带来能力增长。这正在从论文阶段变成可 clone 的开源项目。
- **Resonance hook**: "AI Agent"这个词在中文圈被用烂了，但 99% 讨论的都是无状态 Agent。有状态、自进化的 Agent 是一个完全不同的范式，背后的设计哲学值得单独拆一篇。
- **Recommended priority**: medium

---

## Scan summary

**Sources scanned**:
- X/Twitter: Karpathy, Altman 相关 4 月推文动态
- GitHub Trending: 2026-04-22 周报（shareuhack.com 汇总）
- Hacker News: 4 月前页热帖
- 官方博客: Anthropic, Google Cloud Blog, Google Developers Blog
- 新闻报道: Yahoo Finance, The Next Web, SaaStr, TechCrunch 等
- arXiv: 自进化 Agent 领域近期论文
- 会议动态: Google Cloud Next 2026（4 月 22-24 日）

**Total signals found**: 12+（Anthropic 估值/收入突破、Google Cloud Next A2A、GenericAgent arXiv、EvoSkill、Hermes Agent、Google ADK、Claude Design HN、Skills ecosystem explosion、CaP-Agent0、Multica 平台等）

**Why these 3**:
- Candidate 1（Anthropic 超越 OpenAI）：时效最强（1 天前）+ 中文圈大量报道但全在表面，Zico 的产品策略视角是空白。
- Candidate 2（A2A 协议）：时效强（2 天，正在进行中的会议）+ 直接命中 Agent 经济主题柱 + 中文圈几乎无深度分析。
- Candidate 3（GenericAgent）：时效良好（3 天）+ 命中"AI 作为新物种"深层思考柱 + 技术社区热议但中文圈尚未有好的解读。

**Excluded signals**:
- Karpathy second brain / LLM Wiki：已在 draft 003 中使用，排除。
- Claude Opus 4.7 HN 讨论（4 月 16 日）：超过 7 天窗口，且模型发布讨论竞争激烈，排除。
- AI 安全漏洞（Moltbook token 泄露等）：不符合 Zico 主题柱，排除。
