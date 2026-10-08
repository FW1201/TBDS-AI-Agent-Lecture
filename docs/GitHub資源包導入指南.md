# GitHub 資源包導入指南

## 目的

將講師提供的 GitHub skills/context 資源下載到課程 workspace，檢查來源和內容後，讓 Codex Agent 在案例專案中依流程編輯文件、簡報大綱和試算表。課程資料目前未指定上游資源庫 URL；下方命令中的 `<RESOURCE_REPO_URL>` 和 `<RESOURCE_COMMIT>` 是待講師填入的佔位符，不可直接當成實際網址或版本。

## 匯入步驟

1. 確認 repo URL、可存取性、授權、適用對象及是否允許課堂重分發。
2. 以 HTTPS clone 或下載 ZIP 取得資源，固定到講師確認的 commit/tag；不要把 GitHub token 寫進命令、文件或 shell history。
3. 將原始副本放入 `resources/inbox/<resource-name>/`，記錄來源、commit、日期和下載人員角色。
4. 盤點 README、SKILL.md、context 文件、範本、程式和外部依賴；先閱讀，再決定哪些內容適用。
5. 檢查授權、外部網路需求、檔案操作範圍、命令副作用和資料處理要求。沒有審閱的腳本不執行。
6. 把核准供課堂使用的 skills 放入 `skills/upstream/`，context 文件放入 `context/`；不修改上游原始來源，課程調整另存為 local 版本並註明差異。
7. 在一份合成案例上測試 Agent 是否照 skill 步驟執行、是否產生預期格式、是否保留人工檢查點。
8. 填寫 `resources/manifest.md`，之後更新資源時記錄差異並重新檢查。

## Agent 任務指派範例

```text
請先只盤點 projects/teaching/T1/input/、context/teaching/ 與 skills/upstream/。
先回報你讀到的檔案、使用的 skill/context、來源日期、相互矛盾處、缺漏及建議步驟；暫時不要修改任何檔案。
我確認後，才在 projects/teaching/T1/output/ 建立新教案草稿和來源清單。
不得覆寫 input、不得新增課程事實；不確定處標成「待教師確認」。完成後列出新增檔案及驗收清單。
```

## 資源清單模板

| 名稱 | 類型 | 上游 URL／路徑 | Commit／版本 | 授權 | 用途 | 依賴／網路 | 審閱狀態 |
|---|---|---|---|---|---|---|---|
| 待填 | skill/context | 待填 | 待填 | 待確認 | 待填 | 待填 | 未審閱 |

## GitHub 存取問題

先用目前環境的既有 Git HTTPS proxy 執行唯讀讀取；token 變數不存在不代表 GitHub 不可用。只有在具體操作被拒絕且排除網路與 repo 權限問題後，才記錄需由管理者處理的存取事項。不要索取或保存使用者的秘密值。
