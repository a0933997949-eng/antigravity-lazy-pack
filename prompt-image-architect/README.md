# AI 提示詞與生圖指令架構師 (prompt-image-architect)

本專案是一個將長官指令想法自動升級為高強度 Skill 系統提示詞，並針對簡報或宣導手冊設計英文生圖 Prompt、自動調用 `draw.py` 生成插圖的本機端 Agent 工作流專案。

## 📂 目錄結構
```text
prompt-image-architect/
├── .gitignore         防洩漏設定（隔離 input/ 與 output/）
├── README.md          本說明文件
├── AGENTS.md          給 Agent 讀的執行指令與流程
├── .agents/
│   └── skills/
│       └── prompt-image-architect/
│           └── SKILL.md  核心提示詞優化與 draw.py 自動呼叫規則
├── input/             放置設計需求（請在此放入 design_prompt.txt）
└── output/            產出之系統提示詞 MD 檔、生圖英文指令、自動產出之實體圖片
```

## 🛠️ 使用說明
1. **輸入材料**：將生圖情境或新 AI 角色提示詞想法寫入 `input/design_prompt.txt`。
2. **啟動工作流**：在對話中呼叫 `/prompt-image-architect` 指令。
3. **取得成品**：完成後，Agent 會在背景執行生圖腳本，將實體圖片儲存至 `output/`。