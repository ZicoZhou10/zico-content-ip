# 小红书爆款样本 · 手动喂养工作流

**目的**：你每周手动从小红书 App 里挑 5-10 条同赛道爆款笔记（AI / Agent / 创业 / 科技洞察），扔到这个文件夹。Weekly Pattern Scan trigger 读完后做结构提取，append 到 `templates/viral-patterns.md`。

---

## 工作流（每周日晚或周一早各 5-10 分钟）

1. 在小红书 App 搜关键词："AI"、"Claude"、"AI 创业"、"Anthropic"、"科技洞察"、"AI Agent"
2. 按"近期热门"排序，挑出**点赞 ≥ 1000 但博主粉丝 < 5 万**的笔记（outlier 优先）
3. 每条笔记复制：**标题 + 正文 + 链接 + 点赞数 + 博主粉丝数**
4. 粘贴到本周对应的 `2026-WXX.md` 文件里，用 `---` 分隔每条样本
5. 保存（Obsidian 会自动 push 到 github）
6. 周日晚 21:00 Pattern Scan trigger 自动跑，结构提炼会出现在 `templates/viral-patterns.md`

---

## 每条样本的格式

```
---
url: 小红书笔记链接（可空）
likes: 点赞数
saves: 收藏数（可空）
follower_tier: small / medium / large（small=粉<5万，medium=5-20万，large=>20万）
---

【标题原文】

【正文原文，保留 emoji 和原始排版】
```

样本之间用 `---` 单独一行隔开。

## 示例文件

见 `_TEMPLATE.md`。

## 目录约定

- `2026-W18.md` = 2026 年第 18 周（4/27 - 5/3）
- 一周一个文件，文件名格式 `YYYY-WXX.md`
- 旧周文件保留，作为长期模式数据库
