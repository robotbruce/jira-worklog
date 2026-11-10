# jira-worklog

Claude Code skill **jira-worklog**：每日或每週整理、補登本人 Jira worklog。以一天約 7 小時（含會議與學習）為參考，扣除會議（會議本身不登錄），其餘時間依本人名下當期處理的議題粗略分配，並避免重複登錄。

- Skill 原始碼：`jira-worklog/`，複製到 `~/.claude/skills/jira-worklog`（Claude Code）或 Codex 的 skills 目錄即可使用
- 相依：Claude Code 或 Codex + Atlassian MCP 連接器（可選：行事曆連接器取得會議時數）

## 使用

在 Claude Code 中：

```
/jira-worklog 幫我補本週工時
記今天的工時，先給草稿
```

## 結構

```
jira-worklog/
├── SKILL.md              # 時數分配原則、查既有工時、草稿與寫入流程
└── agents/openai.yaml    # Codex 介面設定（顯示名稱、說明、預設 prompt）
```
