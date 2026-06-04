# 教育備課與 NotebookLM 研究指引專家 (ai-learning-curator)

本專案是一個將警政教材、勤務守則或法規講義，自動轉換為標準教案、測驗卷、演練程序腳本與 NotebookLM 學習指引包的本機端 Agent 工作流專案。

## 📂 目錄結構
```text
ai-learning-curator/
├── .gitignore         防洩漏設定（隔離 input/ 與 output/，符合個資法第27條）
├── README.md          本說明文件
├── AGENTS.md          給 Agent 讀的執行指令與流程
├── .agents/
│   └── skills/
│       └── ai-learning-curator/
│           └── SKILL.md  核心教案規劃、命題測驗與實兵劇本設計規則
├── input/             放置教材原料（請在此放入 training_source.txt）
└── output/            產出之教案說明書、測驗試卷、演練劇本、NotebookLM指引包
```

## 🛠️ 使用說明
1. **輸入材料**：將原始講義、手稿或法令全文寫入 `input/training_source.txt`。
2. **啟動工作流**：在對話中呼叫 `/ai-learning-curator` 指令。
3. **取得成品**：完成後，Agent 會將教案、QA 測驗及 NotebookLM 指引包輸出至 `output/`。