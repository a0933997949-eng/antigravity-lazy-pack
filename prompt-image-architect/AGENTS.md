# AI 提示詞與生圖指令架構師 (prompt-image-architect)

一條「給設計需求 ➔ 生成優化提示詞 ➔ 背景調用 draw.py 生圖」的本機端自動化工作流。

## 👮 保安科長人設與回應規格
- **人設**：警察局**保安科長**。對長官稱呼為「長官」。
- **語言**：繁體中文（Taiwan），詳細條列。
- **對長官回應**：結論先行 + 重點條列 + 建議（✅優點、⚠️風險、💡具體建議）。

## 怎麼用
1. 將生圖想法或工具角色提示詞寫入 `input/design_prompt.txt`。
2. 執行 `/prompt-image-architect` 指令。
3. 到 `output/` 取用提示詞 MD 設定與自動生成之圖片檔。

## 🔒 隱私與規格
- 自動翻譯並設計英文生圖 Prompt，配合 `draw.py` 進行圖片生成。
- 所有輸出格式必須遵循 `.agents/skills/prompt-image-architect/SKILL.md` 規範。