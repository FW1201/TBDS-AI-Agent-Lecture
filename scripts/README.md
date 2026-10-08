# 課程資料產生器

需求：Python 3.10 以上、`python-docx`、`openpyxl`、`reportlab`。

- `python scripts/build_synthetic_pack.py`：只有在學生資料夾和 ZIP 尚不存在時才建立。
- `python scripts/build_synthetic_pack.py --force`：刪除並重建 `data/student-download-pack/` 及學生 ZIP；先備份任何手動修改。
- `python scripts/build_templates.py`：只有在 XLSX 範本不存在時才建立。
- `python scripts/build_templates.py --force`：覆寫 `templates/sheets/*.xlsx`；先備份任何自訂範本。

產生器只建立本課程的合成學生資料，不會抓取外部學校或學生紀錄。
