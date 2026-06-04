# 警政法規與勤務規劃諮詢專家 (police-law-planner)

本專案是一個將警政想定、重大勤務需求或法律個案事實，自動進行法源檢索、適法性評估並草擬結構化勤務計畫與處置方案的本機端 Agent 工作流專案。

## 📂 目錄結構
```text
police-law-planner/
├── .gitignore         防洩漏設定（隔離 input/ 與 output/，符合個資法第27條）
├── README.md          本說明文件
├── AGENTS.md          給 Agent 讀的執行指令與流程
├── .agents/
│   └── skills/
│       └── police-law-planner/
│           └── SKILL.md  核心警政法規分析與勤務計畫生成規則
├── input/             放置想定與任務輸入（請在此放入 task_description.txt）
└── output/            產出之勤務計畫草案、適法性評估報告
```

## 🛠️ 使用說明
1. **輸入材料**：將待推演的警務任務或法規諮詢需求（如：選舉維安、重大人為危安、集會遊行防處）寫入 `input/task_description.txt`。
2. **啟動工作流**：在對話中呼叫 `/police-law-planner` 指令或請 Agent 依據 `AGENTS.md` 執行處理。
3. **取得成品**：完成後，Agent 會將結構化的勤務計畫草案或法規分析報告輸出至 `output/` 資料夾。

## 🔒 隱私與安全守則
1. **個資法合規**：本專案嚴格遵守我國《個人資料保護法》第 27 條之防護義務，`input/` 與 `output/` 內的任何檔案皆已被 `.gitignore` 隔離，**絕不上傳或推送到 GitHub 等公開儲存庫**。
2. **推送到公開庫**：非經使用者之明確指示與授權，**絕對禁止推送到任何公開儲存庫**。
