# Common Dev Prompt

Claude Code 開發工作流的通用 Prompt 集，幫助團隊快速建立 AI 協作規範。

## 這是什麼？

一系列可複用的 Prompt，用來教 Claude Code「怎麼幫你做事」。
直接複製 Prompt 到任何專案中貼上執行，AI 會自動掃描專案結構並產生：

- **指引文件**（CLAUDE.md）— 讓 AI 理解你的專案架構與開發慣例
- **Agent Skill**（.claude/skills/）— 讓 AI 學會專案特有的協作技能
- **Spec-before-Code 工作流** — 強制 AI 先寫規格、確認後才寫程式碼

## 文件說明

| 文件 | 用途 | 使用方式 |
| --- | --- | --- |
| [1.依據過去的程式脈絡產生指引文件及AgentSkill.md](1.依據過去的程式脈絡產生指引文件及AgentSkill.md) | 掃描現有程式碼，自動產生 CLAUDE.md 與 Agent Skill | 整段貼到 Claude Code 執行 |
| [2.多專案Spec-before-Code工作流與AgentSkill導入指南.md](2.多專案Spec-before-Code工作流與AgentSkill導入指南.md) | 一鍵建立 Spec-before-Code 完整工作流（含目錄結構、範本、指令） | 複製「一鍵導入」區塊，改一行描述即可 |

## 涵蓋的 Prompt

### 初始建立（挑一個執行即可）

| Prompt | 說明 |
| --- | --- |
| 一鍵導入 Spec-before-Code 工作流 | 自動掃描專案 → 產生 CLAUDE.md、rules、skills、commands、templates，只需改一行專案描述 |
| 產生 CLAUDE.md 指引文件 | 掃描專案結構與技術棧，產生 AI 指引文件 |
| 產生 Agent Skill | 掃描程式碼脈絡，建立 AI 協作技能文件 |

### 日常開發

| Prompt | 說明 |
| --- | --- |
| 跨子專案功能開發 | 自動判斷影響範圍 → 建 Spec → 確認後開發 |
| Bug 修復 | 分析根因 → 建 Spec → 確認後修復 → 記錄 Bug Log |
| 分析程式碼建立慣例 | 分析命名、結構、pattern，在 rules/ 建立慣例規則 |

### 文件同步

| Prompt | 說明 |
| --- | --- |
| 新增 command 後更新文件 | 同步更新 README.md、CLAUDE.md、skills |
| sync-docs（`/sync-docs`） | 掃描專案，補齊 README 與 CLAUDE.md 中缺少的內容 |
| sync-skill（`/sync-skill`） | 掃描專案，補齊 skills/ 中缺少的技能描述 |

## 如何使用

1. 到目標專案根目錄開啟 Claude Code
2. 選擇適合的 Prompt，複製貼上
3. AI 自動掃描專案結構並產生所有檔案

不需要手動填入資料夾名稱或技術棧，AI 會自動偵測。

## 適用對象

任何使用 Claude Code 的開發團隊，無論是單一專案或多專案結構皆適用。
