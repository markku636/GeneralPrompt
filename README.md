# Common Dev Prompt

Claude Code 開發工作流的通用 Prompt 範例集，幫助團隊快速建立 AI 協作規範。

## 這是什麼？

這個專案收錄了一系列可複用的 Prompt 範本，用來教 Claude Code「怎麼幫你做事」。
你可以直接複製這些 Prompt 到任何專案中使用，快速建立：

- **指引文件**（CLAUDE.md）— 讓 AI 理解你的專案架構與開發慣例
- **Agent Skill**（.claude/skills/）— 讓 AI 學會專案特有的協作技能
- **Spec-before-Code 工作流** — 強制 AI 先寫規格、確認後才寫程式碼

## 文件說明

| 文件 | 內容 |
| --- | --- |
| [1.依據過去的程式脈絡產生指引文件及AgentSkill.md](1.依據過去的程式脈絡產生指引文件及AgentSkill.md) | 依據現有程式碼脈絡，自動產生 CLAUDE.md 指引文件與 Agent Skill 的 Prompt 範例 |
| [2.多專案Spec-before-Code工作流與AgentSkill導入指南.md](2.多專案Spec-before-Code工作流與AgentSkill導入指南.md) | 多專案結構下的 Spec-before-Code 完整導入指南，含目錄結構、範本、Prompt 範例 |

## 涵蓋的 Prompt 範例

### 文件同步類
- 依據新增 command 更新 README 及 CLAUDE.md
- 依據新增 command 更新 Agent Skill
- 同步掃描專案結構，自動補齊文件（sync-docs / sync-skill）

### 工作流建立類
- 一鍵導入 Spec-before-Code 工作流（含完整目錄結構與範本）
- 為現有專案產生 CLAUDE.md 指引文件
- 為現有專案產生 Agent Skill

### 開發流程類
- 跨子專案功能開發（全端聯動）
- 分析現有程式碼建立開發慣例
- Bug 修復標準化流程

## 如何使用

1. 選擇適合你專案的 Prompt 範例
2. 將範例中的佔位符替換為你的專案資訊
3. 在 Claude Code 中執行 Prompt
4. AI 會依據你的專案結構自動產生對應的文件與設定

## 適用對象

任何使用 Claude Code 的開發團隊，無論是單一專案或多專案結構皆適用。
