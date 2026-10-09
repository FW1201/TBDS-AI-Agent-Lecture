# 課程 Skills

`local/` 放本 repo 為課程示例撰寫的 skills；`upstream/tw-edu-skills/` 保留教師提供的上游原件。匯入來源、版本、授權和更新方式見 [`upstream/README.md`](upstream/README.md)。上游技能不等於已安裝或自動啟用；課堂依案例明確指定對應的 `SKILL.md`，讓 Codex Agent 閱讀後整理輸入、編輯案例專案並建立輸出。

## 課程案例對照

| 案例 | 建議上游 skill | 操作重點 |
|---|---|---|
| T1 九年級社會通學探究 | `tw-edu-lesson-plan-108`、`tw-edu-rubric-designer`、`tw-edu-material-reviewer` | 從目標與來源建立教案、規準，再檢查隱私和資料品質 |
| T2 高一地理微氣候 | `tw-edu-interdisciplinary`、`tw-edu-differentiated`、`tw-edu-worksheet-creator` | 將同一合成資料轉為探究活動及不同支架 |
| T3 高中國文形成性回饋 | `tw-edu-feedback-writer`、`tw-edu-formative-assessment` | 根據匿名作品證據撰寫回饋，不代替正式評分 |
| A1 課發會提案與意向調查 | `tw-edu-school-curriculum-plan`、`tw-edu-school-document` | 區分意向與正式選課，草擬提案摘要及通知 |
| A2 會議紀錄與行動追蹤 | `tw-edu-meeting-facilitator`、`tw-edu-official-document` | 保留討論、決議、未決事項的差異和來源 |
| A3 成果交流日 | `tw-edu-school-document`、`tw-edu-parent-communication` | 依核定資料整理計畫和通知草稿，標出待確認事項 |
| A4 回饋問卷分析 | `tw-edu-learning-evidence-analyzer`、`tw-edu-research-viz` | 先核定清理規則，再分析合成問卷並說明限制 |
| A5 設備盤點 | `tw-edu-school-document` | 將表格差異整理為可追查的盤點說明和待辦 |
| A6 月報與主管簡報 | `tw-edu-school-document`、`tw-edu-slides-creator`、`tw-edu-meeting-facilitator` | 從追蹤表生成多格式草稿，狀態附來源和日期 |

上表是課堂選用建議，不代表只可使用這些技能。每次操作仍要先查看 skill 的適用邊界、所需輸入、依賴和產出驗證方法；所有案例資料是合成資料，正式教學、行政決策和對外發送由教師／承辦人覆核。

## 本地課程示例

本地示例提供一套教案草擬、校務文件整理、試算表品質檢查和簡報摘要流程。是否能由 Codex 自動載入，取決於實際 workspace 的 skill 安裝位置和 Codex 版本；課堂可先將 `SKILL.md` 當作 Agent 參考文件明確指定。
