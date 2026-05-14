---
date: 2026-05-14
status: written
selected: candidate 2 → drafts/018-ai-molecule-trial-xhs.md
---

# Today's Candidates

## Candidate 1: OpenAI Deployment Company 发布——McKinsey 和 Bain 同时当这家公司的投资人和被颠覆对象

- **Event**: 2026年5月11日（3天前），OpenAI 正式发布 **OpenAI Deployment Company**（内部代号 DeployCo），完成 **$40 亿融资，估值 $140 亿**，OpenAI 持有多数股权并保留运营控制权（其中 OpenAI 自己注入 $5 亿现金 + $10 亿期权）。投资方阵容：**TPG**（领投）、Advent、Bain Capital、Brookfield、Goldman Sachs，以及咨询公司 **McKinsey & Company、Bain & Company、Capgemini**——三家全球最大咨询公司既是本轮投资者，又将直接面对 DeployCo 在企业 AI 改造市场的竞争。同日，OpenAI 宣布收购应用 AI 咨询公司 **Tomoro**，从第一天起引入约 **150 名 Forward Deployed Engineers（FDE，前向部署工程师）**。FDE 模式：OpenAI 自己的工程师嵌入企业客户内部，在客户的安全模型、合规要求、遗留基础设施内直接构建和部署 AI 生产系统。三家咨询伙伴合计年营收超 **$490 亿**，合计员工约 **424,000 人**（其中大量参与企业 AI 项目）。Axios（5月11日）报道 DeployCo 估值 $140 亿；SiliconANGLE、The Register、CIO Dive（5月11日）同日覆盖。背景：**2026年5月4日**，Anthropic 也与 Blackstone、Hellman & Friedman、Goldman Sachs 发布 **$15 亿** AI 咨询合资公司，目标是向中型企业嵌入 Claude 工程师，与 OpenAI DeployCo 模式几乎相同，相隔一周先后发布。
- **Source**: https://openai.com/index/openai-launches-the-deployment-company/ | https://www.axios.com/2026/05/11/openai-deployco-private-equity | https://thenextweb.com/news/tomoro-openai-deployment-company-consulting | https://www.bain.com/about/media-center/press-releases/2026/bain-company-openai-a-new-venture-to-deploy-ai-at-enterprise-stage/ | https://siliconangle.com/2026/05/11/openai-launches-professional-services-business-4b-investment/
- **Timeliness**: 3 days ago（2026年5月11日）
- **Topic pillar**: 组织形式变革
- **Zico's angle**: 中文媒体把这件事报道成"OpenAI 进军咨询行业"，配一张和麦肯锡、埃森哲的市场份额对比图，结束。这个叙事框架恰好遮住了最值得注意的地方：**McKinsey 和 Bain 是 DeployCo 的股东——他们在给一家要替代他们核心业务的公司出钱。** 传统咨询公司最难被替代的业务是"组织变革顾问"——懂行的合伙人带团队进驻客户公司，帮它重构流程。DeployCo 的 FDE 做的是一模一样的事，只是把人换成了 OpenAI 工程师：进客户的内部，在它的合规体系和遗留 IT 里搭 AI 系统。这个模式是 **Palantir** 十年前发明的——Palantir 不卖软件许可，他们把工程师嵌进五角大楼和 CIA。OpenAI 现在做的是 AI 时代的 Palantir 化。McKinsey 和 Bain 选择成为 DeployCo 的股东而不是纯粹竞争对手，不是认输，是换一种方式继续分到企业 AI 改造的钱。但这个逻辑还有下一层：麦肯锡的人完成同等任务收多少，OpenAI 的 FDE 完成同等任务收多少——这个价差决定了传统咨询利润空间还能维持多久。同一周 Anthropic 也做了同一件事（$15 亿，Blackstone + Goldman），不是巧合：**"模型公司 → 嵌入式工程师 → 重构企业工作流"这条垂直整合路径，在一周之内被 OpenAI 和 Anthropic 双重验证**。对做 B2B AI 产品的人，这有一个直接的含义：不卖产品，卖嵌入本身。
- **Resonance hook**: 2026年5月11日，OpenAI 发布了一家新公司专门帮企业部署 AI，融资 $40 亿，估值 $140 亿。最荒诞的细节：McKinsey 和 Bain 同时是这家公司的投资人，也是它最直接的竞争对手。七天前，Anthropic 用同一套逻辑跟 Blackstone 和 Goldman Sachs 发了 $15 亿的版本。AI 模型公司开始垂直整合进咨询：不是卖软件，而是把自己的工程师嵌进企业内部重构工作流。
- **Recommended priority**: high

---

## Candidate 2: Isomorphic Labs 完成 $21 亿 B 轮——AlphaFold 的下一步是把 AI 设计的分子送进人体

- **Event**: 2026年5月12日（2天前），**Isomorphic Labs** 宣布完成 **$21 亿 B 轮融资**，由 **Thrive Capital** 领投，现有股东 Alphabet（Google 母公司）和 GV 跟投，新增投资方包括 **MGX**（阿联酋主权基金）、**Temasek**（新加坡主权基金）、**CapitalG** 和 **英国主权 AI 基金（UK Sovereign AI Fund）**。Isomorphic Labs 2021 年由 **Demis Hassabis** 从 Google DeepMind 分拆创立，建立在 AlphaFold 蛋白质结构预测技术之上，核心产品是 AI 药物设计引擎 **IsoDDE**（Isomorphic Drug Design Engine）。公司目前维持与 **Novartis、Eli Lilly、Johnson & Johnson** 的付费战略合作管线。新资金用于继续开发 IsoDDE 并将治疗项目推进至临床：公司预计将于 **2026 年底启动首批人体 I 期临床试验**（此前 Hassabis 目标为 2025 年底，延迟约一年）。Bloomberg（5月12日）、PR Newswire（5月12日官方新闻稿）、Yahoo Finance（5月12日）同日多媒体覆盖。
- **Source**: https://www.isomorphiclabs.com/articles/isomorphic-labs-announces-series-b-investment-round | https://www.bloomberg.com/news/articles/2026-05-12/deepmind-spinout-isomorphic-labs-raises-2-1-billion-to-design-drugs-with-ai | https://www.prnewswire.com/news-releases/isomorphic-labs-secures-2-1-billion-funding-to-scale-its-ai-drug-design-engine-302769674.html | https://finance.yahoo.com/sectors/healthcare/articles/google-backed-isomorphic-raises-2-152155056.html
- **Timeliness**: 2 days ago（2026年5月12日）
- **Topic pillar**: 深层思考
- **Zico's angle**: AlphaFold 改变了科学家理解蛋白质的方式——它解决了人类用实验方法研究了五十年的问题。但"预测蛋白质如何折叠"和"设计一个可以进入人体的药物分子"之间是两件不同的事。**Isomorphic Labs 在跨这个跳跃**。IsoDDE 不是在帮化学家更快地验证假设，而是在生成化学家原本无法系统搜索的分子空间里的候选物——因为这个空间的维度太高，人类直觉无法导航。$21 亿融资的投资方结构很能说明问题：两个主权基金（英国 + 新加坡）、Thrive Capital 和 Alphabet 同时押注，意味着这不是科研赌注，是主权级别的"AI 工业化制药"竞争。Novartis 和 Lilly 为 Isomorphic Labs 的化合物**付钱**——不是为咨询付钱，而是为 AI 生成的候选物付钱——意味着 AI 的输出已经进入了制药公司风险评估体系认可的质量级别。2026 年底首批人体试验，是 AI 从"分析工具"变成"创造者"在科学领域的第一个公开时钟：**AI 设计的分子将第一次进入人体**。这是 Zico 的"AI 是新物种"框架在科学领域的最具体案例。
- **Resonance hook**: AlphaFold 解决了蛋白质折叠——一个科学家研究了五十年的问题。Isomorphic Labs 的下一步：用 AI 从头设计药物分子，2026 年底送进人体 I 期临床。$21 亿 B 轮，Thrive Capital 领投，英国和新加坡两国主权基金跟投，Novartis 和 Lilly 已经在为 AI 生成的化合物付钱。AI 第一次不是在加速科学家的工作，而是在提交自己的候选分子进入临床管线。
- **Recommended priority**: high

---

## Candidate 3: 18 位顶级研究者联合发布 survey——"没有 World Model，VLA 机器人走不到复杂场景"

- **Event**: 2026年5月初（arXiv 2605.00080），来自 **Stanford、UC Berkeley、ETH Zurich、Oxford、Harvard、INRIA** 的 18 位研究者联合发布综述论文《**World Model for Robot Learning: A Comprehensive Survey**》。通讯作者包括：**Jiajun Wu**（Stanford AI Lab）、**Pieter Abbeel**（UC Berkeley，深度 RL 奠基人之一）、**Jitendra Malik**（UC Berkeley，计算机视觉先驱）、**Marc Pollefeys**（ETH Zurich，3D 视觉与 NeRF/3DGS 领域核心人物）、**Oier Mees**（UC Berkeley）、**Zhuang Liu**（Meta AI Research）、**Yilun Du**（Harvard）。论文核心论点：**"纯反应式 VLA（Vision-Language-Action）策略在复杂物理环境中的上限，根源在于缺乏对'agent 行动后环境如何演化'的显式预测结构"**。综述梳理 world model 在机器人学习中的四大角色，覆盖代表工作从 TD-MPC2、LeWorldModel 到 GROOT、UniSim。配套 GitHub 仓库 NTUMARS/Awesome-World-Model-for-Robotics-Policy 收录 200+ 篇论文并持续更新。
- **Source**: https://arxiv.org/abs/2605.00080 | https://ntumars.github.io/wm-robot-survey/ | https://www.alphaxiv.org/overview/2605.00080 | https://github.com/NTUMARS/Awesome-World-Model-for-Robotics-Policy
- **Timeliness**: ~14 days ago（2026年5月初，在30天可接受窗口内；中文圈覆盖率接近零）
- **Topic pillar**: 深层思考（空间智能前沿）
- **Zico's angle**: 做 3DGS 产品的人有一个独特位置来读这篇 survey。**Marc Pollefeys 同时是 3DGS 领域的核心人物，也是这篇论文的通讯作者之一**——空间理解（3DGS 解决的问题）和空间预测（world model 要解决的问题）正在合流。3DGS 给了机器人"看到当前世界是什么"的能力；world model 给机器人"预测如果我做这个动作世界会变成什么"的能力。两者叠加才是真正的 Physical AI 所需要的东西。这篇 survey 说的"VLA 在复杂场景里有系统性上限"对 NVIDIA GR00T（Jim Fan 在做的）、Figure AI、1X 和 Boston Dynamics 都是一个检验框架。Pieter Abbeel 和 Jitendra Malik 同时出现在通讯作者列表，意味着这是整个 embodied AI 社区对"下一个要解决的核心问题"的集体标定。
- **Resonance hook**: UC Berkeley、Stanford、ETH Zurich 的 18 位机器人研究者今年发了一篇 survey，核心结论是：VLA 机器人的系统性上限来自一件它做不到的事：预测"我的行动之后世界会是什么样"。这不是算力不够，是架构缺了一层。Pieter Abbeel 和 Jitendra Malik 同时在通讯作者列表，说明这不是边缘意见——是整个领域在标定下一个要解决的问题。
- **Recommended priority**: medium

---

## Scan summary

- **Sources scanned**: OpenAI 官方博客（5月11日 DeployCo）、Isomorphic Labs 官方（5月12日 Series B）、PR Newswire（5月12日）、Bloomberg（5月12日）、Axios（5月11日）、The Next Web（5月11日）、SiliconANGLE（5月11日）、Bain & Company 官方（5月11日）、CIO Dive（5月11日）、Yahoo Finance / BioPharm / BioSpace（5月12日）、arXiv cs.AI（2605.00080）、alphaXiv、NTUMARS GitHub、Fortune（5月4日 Anthropic JV 背景）、X/Twitter（Altman DeployCo 确认；Demis Hassabis Isomorphic B 轮 X 帖；Karpathy/Jim Fan/LeCun/Swyx/Nat Friedman 无5月12-14日独立新信号）、HN（DeployCo 上榜；Isomorphic Labs 上榜）、GitHub Trending（NTUMARS/Awesome-World-Model-for-Robotics-Policy 新上榜）
- **Total signals found**: 22 evaluated
- **Why these 3**:
  - **Candidate 1（OpenAI DeployCo）**：时效3天（5月11日），近7天 candidates 完全未覆盖；McKinsey + Bain 同时当投资人和被颠覆对象；Palantir 映射中文圈无人点名；组织形式变革柱近期空缺。
  - **Candidate 2（Isomorphic Labs）**：时效最强（2天，5月12日）；"AI 设计分子首次进人体"时效锚点中文圈零深度覆盖；AI 是新物种框架天然对接；深层思考柱角度与5月13日 NLA 完全不同。
  - **Candidate 3（World Model survey）**：时效14天（30天窗口内）；Marc Pollefeys 的 3DGS+world model 双重身份给 Zico 独有视角；Pieter Abbeel + Jitendra Malik 赋予领域共识地位；空间智能前沿柱本周空缺。

---

**Excluded signals**:
- Googlebooks（5月12日，同 Android Show 事件，已在5月13日 candidates 覆盖为 Gemini Intelligence）
- OpenAI-Microsoft $380 亿上限（原始协议4月27日，17天前）
- GPT-Realtime-2（发布日期无法独立确认为5月12日后）
- Claude Mythos 未授权访问（来源单一，无官方日期）
- DeepSeek 模型预览（4月24日，20天前，国内已全覆盖）
- Anthropic 咨询 JV（5月4日，作为 Candidate 1 背景锚点使用）
