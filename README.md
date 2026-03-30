# SolveTW 解題公社

> **真實問題。開放解法。信任資產。**

企業出真題，學生用 AI 解題，業師 Review，解法開源永存。
在作品集已經無法證明實力的時代，用「被誰認可」取代「做了什麼」。

---

## 這是什麼？

SolveTW 是一個讓**解題過程變成可複用資產**的開放平台：

```
企業出真題 → 學生解題 → 業師 Review → 解法開源存檔 → 後人複用改進
                              ↓
                    累積「被業界認可」的信任資產
```

- **不是作業** — 題目來自真實企業的真實痛點
- **不是比賽** — 解法開源共享，不是贏者全拿
- **不是外包** — 有教育價值閘門，企業不能把學生當免費勞工
- **AI 友善** — 用 AI 解題不是作弊，但你必須記錄判斷過程

## 為什麼需要？

AI 把「產出及格成果」的門檻壓到幾乎為零。當每個求職者的作品集都看起來一樣好：

- 履歷跟作品都是 AI 做的 → 僱主無法區分能力
- 篩選退化為學校品牌和人脈推薦
- 私立大學學生即使學會所有 AI 工具，競爭位置不變

**SolveTW 的解法**：讓學生在畢業前累積「被業界決策者認可」的紀錄。
不是 GPA，不是證照，而是一張**「誰看過你的作品，並且願意背書」**的信任網絡。

---

## 角色

| 角色 | 你是誰 | 你在這裡做什麼 | 入門指南 |
|------|--------|-------------|---------|
| **出題者 (PO)** | 企業主管、產業顧問 | 把真實問題丟出來，學期末 review 解法 | [出題者指南](docs/for-problem-owners.md) |
| **解題者 (SV)** | 大學生、自學者、轉職者 | 解真實問題，累積聲望 | [解題者指南](docs/for-solvers.md) |
| **評審 (RV)** | 業師、技術主管 | 用碎片時間 review，發掘人才 | [評審指南](docs/for-reviewers.md) |
| **促進者 (FC)** | 大學老師、育成中心 | 把題目帶進課堂 | [教師指南](docs/for-teachers.md) |

## 核心機制

### Decision Log — 判斷力的紀錄

每份解法必須附帶 [Decision Log](docs/decision-log-template.md)，記錄：
1. 你怎麼理解問題
2. 考慮過哪些方案（至少 2 個）
3. AI 做了什麼、你判斷了什麼
4. 犧牲了什麼（trade-offs）
5. 失敗的嘗試
6. 後人複用指南

> 程式碼不值錢（AI 都能寫）。值錢的是「為什麼選這個方案」。

### 聲望系統 — 被誰認可比做了多少重要

```
聲望 = 解題分(35%) + Review權重分(30%) + 複用分(20%) + 貢獻分(15%)
```

- 業界主管的認可 **10 倍**權重於一般互評
- 解法被後人 Fork 改進，原作者持續獲得複用分
- 聲望等級：🌱 Newcomer → 🔧 Contributor → 🏗️ Builder → ⚡ Expert → 🏆 Master

完整規則：[聲望計算規則](docs/reputation-rules.md)

### 解法複用 — 花掉的 Token 變成投資

- 所有 Approved 解法開源存檔
- 可以 Fork 前人的解法改進（必須引用來源）
- 被 Fork 3+ 次自動升級為 Solution Template
- 引用鏈讓原作者持續獲得聲望

---

## 題目瀏覽

### 依難度

| 難度 | 適合誰 | AI 依賴度 |
|------|--------|-----------|
| [⭐ Beginner](../../labels/difficulty%3A%20beginner) | 會用 AI 對話工具 | 90% AI + 10% 判斷 |
| [⭐⭐ Intermediate](../../labels/difficulty%3A%20intermediate) | 會串接工具 + 基本 coding | 70% AI + 30% 判斷 |
| [⭐⭐⭐ Advanced](../../labels/difficulty%3A%20advanced) | 會 API 整合 + 系統設計 | 50% AI + 50% 設計 |
| [⭐⭐⭐⭐ Expert](../../labels/difficulty%3A%20expert) | 架構設計 + 產品思維 | 30% AI + 70% 架構 |

### 依產業

製造業 | 零售服務 | 醫療健康 | 農業 | 教育 | 金融 | 社會創新 | 通用

### 依類型

| 類型 | 時間 | 適合 |
|------|------|------|
| ⚡ Quick Fix | 1-3 天 | 個人 |
| 🏃 Sprint | 1-2 週 | 個人或 2 人 |
| 📋 Project | 1-3 月 | 3-5 人團隊 |
| 🎓 Capstone | 一學期 | 課堂團隊 |

---

## 快速開始

### 我是企業，想出題

1. 點擊 [New Issue → 出題](../../issues/new?template=new-problem.yml)
2. 填寫題目表單（約 30 分鐘）
3. 等學生解題
4. 學期末花 1 小時 Review 解法

### 我是學生，想解題

1. 瀏覽 [題目列表](problems/)，找到感興趣的
2. 在題目 Issue 下留言報名
3. Fork repo，在 `problems/<題目>/solutions/<你的名字>/` 下工作
4. 完成後提交 PR，附上 [Decision Log](docs/decision-log-template.md)
5. 等待 Review，根據回饋改進

### 我是老師，想嵌入課程

1. 閱讀 [教師指南](docs/for-teachers.md)
2. 從題目庫選題，或邀請業界朋友出題
3. 將解題作為課程專案
4. 學期末邀請出題企業做 Final Review

---

## 目錄

```
solve-tw/
├── problems/           ← 題目與解法存放處
├── templates/          ← 被 Fork 3+ 次的解法模板
├── hall-of-fame/       ← 被企業採用的解法
├── leaderboard/        ← 聲望排行榜
└── docs/               ← 指南與規則
    ├── for-problem-owners.md
    ├── for-solvers.md
    ├── for-reviewers.md
    ├── for-teachers.md
    ├── decision-log-template.md
    ├── decision-log-guide.md
    └── reputation-rules.md
```

---

## 授權

- **解法程式碼**：MIT License（可自由使用、修改、商用）
- **Decision Log 與文件**：CC BY-SA 4.0（可自由使用，需引用來源，衍生作品同授權）
- **題目內容**：由出題者決定，預設 CC BY-NC 4.0

---

## 聯絡

- 發起人：[cooperation.tw](https://cooperation.tw)
- 問題回報：[Issues](../../issues)
- 合作洽談：[Discussions](../../discussions)

---

*SolveTW — 讓解題成為資產，讓信任可以累積。*
