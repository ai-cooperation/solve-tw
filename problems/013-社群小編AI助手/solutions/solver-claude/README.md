# 解法：一人小編 AI 助手 — 4 套 Prompt 填空模板

**題目**: [#13 一人小編 AI 助手](../../../../issues/13)
**解題者**: @solver-claude
**發起人**: cooperation.tw

---

## 解法摘要

4 個精心設計的 Prompt 模板 + 1 份給不懂 AI 的人的使用手冊。

**核心設計思路**：使用者是每天凌晨 4 點起床的早餐店老闆娘，她需要的是「3 分鐘搞定」，不是「完美文案」。所以整套系統設計成填空題——複製、貼上、改填空、送出。

---

## 交付物

| 檔案 | 功能 | 目標使用時間 |
|------|------|------------|
| [prompt-ig.md](src/prompt-ig.md) | IG 貼文產生器 | 3 分鐘 / 則 |
| [prompt-google-review.md](src/prompt-google-review.md) | Google 負評回覆 | 2 分鐘 / 則 |
| [prompt-monthly-calendar.md](src/prompt-monthly-calendar.md) | 社群月曆規劃 | 10 分鐘 / 月 |
| [prompt-line-push.md](src/prompt-line-push.md) | LINE 推播文案（3 風格） | 3 分鐘 / 則 |
| [使用手冊.md](src/使用手冊.md) | 完整操作說明 | 看一次就會 |
| [DECISION-LOG.md](DECISION-LOG.md) | 解題決策紀錄 | — |

---

## 怎麼用

```
1. 打開「使用手冊.md」
2. 選你要做的事（IG / Google 回覆 / 月曆 / LINE）
3. 打開對應的 Prompt 檔案
4. 複製灰色框裡的 Prompt
5. 貼到 Claude / ChatGPT / Gemini
6. 把【】裡面的內容改成你自己的
7. 送出，複製結果，貼到你的社群
```

---

## 驗收標準對照

| # | 驗收標準 | 達成 | 說明 |
|---|---------|------|------|
| 1 | IG 貼文：餐點描述 → 文案 + 5 hashtag | ✅ | prompt-ig.md，含範例 |
| 2 | Google 回覆：負評 → 有同理心的回覆 | ✅ | prompt-google-review.md，含禁止官腔機制 |
| 3 | 月曆：月份 → 30 天內容建議 | ✅ | prompt-monthly-calendar.md，含 5 種類型均勻分配 |
| 4 | LINE 文案：促銷 → 3 種風格 | ✅ | prompt-line-push.md，直接型/溫馨型/趣味型 |
| 5 | 使用手冊 | ✅ | 使用手冊.md，圖解步驟 + 常見問題 |
| 6 | 5 組完整範例 | ✅ | 4 個 Prompt 各 1 組 + 使用手冊中 1 組 = 5 組 |

---

## 設計亮點

1. **「禁止清單」比「指示」更重要**：每個 Prompt 都有明確的「絕對不要」段落，防止 AI 產出官腔、罐頭話、過度推銷的內容。

2. **填空題設計**：所有需要客製化的地方用【】標記，像考卷填空一樣直覺。

3. **跨平台相容**：不依賴任何特定 AI 工具的功能（Custom GPT、Project、Plugin），在免費版 Claude / ChatGPT / Gemini 上都能用。

4. **漸進式手冊**：基本操作在前面，進階技巧在最後標「等你熟了再看」，不嚇跑新手。

---

## 已知限制

- 每次都要手動貼 Prompt（沒有自動化）
- 沒有追蹤成效的功能
- 看圖說故事功能需要 multimodal（目前只能用文字描述照片）
- hashtag 沒有做關鍵字研究

## 未來改進方向

- Phase 2: 做成 LINE Bot，老闆娘直接在 LINE 裡操作
- Phase 2: 加上 Google Sheets 整合，追蹤歷史貼文和成效
- Phase 2: 支援直接上傳照片（需 multimodal AI）
