# Obsidian 同步與維護專家 (vault-obsidian-sync-automator)

本專案是一個將剪藏之法規、逐字稿或外部網頁文章，自動去除雜訊、語法重構為 Obsidian Markdown 結構，並巡檢知識庫死鏈、孤島頁的自動化工作流專案。

## 📂 目錄結構
```text
vault-obsidian-sync-automator/
├── .gitignore         隔離 input/ 與 output/，符合個資法第27條
├── README.md          本說明文件
├── AGENTS.md          給 Agent 讀的執行指令與流程
├── .agents/
│   └── skills/
│       └── vault-obsidian-sync-automator/
│           └── SKILL.md  核心知識庫重構、Wiki連結橋接與健康巡檢規則
├── input/             放置新剪藏文章（請放入 input/new_clippings/）
└── output/            產出之整理成果或 wiki-lint 巡檢報告
```

## 🛠️ 使用說明
1. **輸入材料**：將新剪藏的網頁草稿或法規公報，放入 `input/new_clippings/` 中。
2. **啟動工作流**：在對話中呼叫 `/wiki-ingest` 或 `/wiki-lint`。
3. **取得成品**：完成後，Agent 會將美化後的筆記歸檔至知識庫對應資料夾。