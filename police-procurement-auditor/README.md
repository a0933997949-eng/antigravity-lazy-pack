# 警政採購與合規審計專家 (police-procurement-auditor)

本專案是一個針對保安科警用裝備、通訊器材或監視系統招標規格書，進行政府採購法合規性比對、防範行政違失，並生成議事答詢與申訴說明書的本機端 Agent 工作流專案。

## 📂 目錄結構
```text
police-procurement-auditor/
├── .gitignore         防洩漏設定（隔離 input/ 與 output/，符合個資法第27條）
├── README.md          本說明文件
├── AGENTS.md          給 Agent 讀的執行指令與流程
├── .agents/
│   └── skills/
│       └── police-procurement-auditor/
│           └── SKILL.md  核心採購法比對與答詢稿生成規則
├── input/             放置審查原料（請在此放入 audit_target.txt）
└── output/            產出之採購法合規檢核報告、議事答詢稿
```

## 🛠️ 使用說明
1. **輸入材料**：將待審查的招標規格書、質詢問題或廠商異議書寫入 `input/audit_target.txt`。
2. **啟動工作流**：在對話中呼叫 `/police-procurement-auditor` 指令。
3. **取得成品**：完成後，Agent 會將合規檢核表或答詢說明稿輸出至 `output/` 資料夾。