# #18 發票整理助手 (v2)

## 這是什麼

一個 Web App，解決中小企業每月花 3 天處理發票的問題。

**核心不是 OCR，是整理** — 分類、對帳、查找、報表。

**[▶ 直接打開 index.html 試用](index.html)**

## v1 → v2 學到什麼

| v1 的錯誤 | v2 的修正 |
|----------|----------|
| 把 OCR 辨識當主角 | OCR 只是輸入方式之一，整理才是核心 |
| 沒搜競品就做 | 研究了 TaxHacker、Akaunting、PaddleOCR |
| 每張發票都問 AI 分類 | 規則學習：人工分類幾筆後系統自動學會 |
| 只有發票 vs 訂單 | 三方對帳：發票 vs 訂單 vs 銀行帳單 |
| 沒有查找功能 | 全文搜尋 + 科目/日期篩選 |
| 結果只能看 | 匯出 Excel CSV |

## 功能

| Tab | 做什麼 |
|-----|--------|
| 📥 匯入 | CSV（主要）/ 拍照 Vision API（紙本）/ 手動輸入 |
| 🏷️ 分類 | 智慧分類引擎（規則學習，不是每張都問 AI）|
| 🔗 對帳 | 三方比對：發票 vs 訂單 vs 銀行 + 異常偵測 |
| 🔍 查找 | 全文搜尋 + 科目/日期篩選 |
| 📊 報表 | 科目統計 + 供應商排行 + 月度趨勢 + 異常標記 |

## 參考了誰

| 專案 | 學了什麼 |
|------|---------|
| [TaxHacker](https://github.com/vas3k/TaxHacker) | 分類規則可學習、LLM 只在不確定時才用 |
| [invoice-processing](https://github.com/ruizguille/invoice-processing) | 匯出 Excel、財務分析自動化 |
| [Akaunting](https://github.com/akaunting/akaunting) (9k⭐) | 知道不該重做完整會計系統 |

完整 Decision Log：[DECISION-LOG.md](DECISION-LOG.md)
