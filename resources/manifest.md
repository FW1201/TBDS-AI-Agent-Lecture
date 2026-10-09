# GitHub 課程資源 Manifest

本表記錄課程內的外部及本地資源。上游版本以精確 commit 為準；有更新時新增版本紀錄，不覆蓋舊來源。

| 資源 | 類型 | 來源 | 版本／日期 | 授權／狀態 | 適用課堂 |
|---|---|---|---|---|---|
| `tw-edu-skills` | 上游 skills 與課綱參考快照 | [FW1201/tw-edu-skills](https://github.com/FW1201/tw-edu-skills) | v5.0.1；`420afdf58d913b6d240c4a6b41ef55bb7d0a66ec`；匯入 2026-10-09 | MIT；保留原始 `LICENSE`、README、CITATIONS 與文件；35 skills 已複製至 `skills/upstream/tw-edu-skills/` | T1–T3、A1–A6 |
| tw-edu 課綱資料快照 | 上游共同參考資料 | `skills/upstream/tw-edu-skills/shared/curriculum/references/curriculum/` | 上游 snapshot manifest 標示 2026-09-08；隨上述 commit 匯入 | 含每檔來源與 SHA256 manifest；屬上游封存快照，正式引用前須核對官方現行版本 | T1、T2 |
| 課程簡報大綱 3 份 | 教材 | 本 repo `slides outline/` | 2026-10-08 | 已編寫，待 Claude 生成投影片及講師核對 | 全部 |
| 學生資料包 | 合成練習資料 | `scripts/build_synthetic_pack.py` 生成 | 2026-10-08 | 已生成；內容皆為模擬資料 | 全部 |
| 教學情境 Context | 專案脈絡 | 本 repo `context/teaching/` | 2026-10-08 | 已編寫；非課綱原文，含現行課綱核對要求 | 教學 |
| 行政流程 Context | 專案脈絡 | 本 repo `context/administration/` | 2026-10-08 | 已編寫；非校內規則 | 行政 |

複製方式為來源 commit 的 Git archive，未包含 `.git`、未執行安裝器、未改寫上游 skill 檔案。課堂使用時先依 [`../skills/README.md`](../skills/README.md) 選取 skill，檢查其 `SKILL.md`、manifest、schema、範例、依賴與限制，再指派 Agent；學生案例只能使用合成資料。上游套件中若有 scripts 或依賴，不代表課堂需要執行它們。
