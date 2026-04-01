# 113 屆大學部專題

## 基本資訊

| 項目 | 說明 |
|------|------|
| 屆別 | 113 屆（113 學年度入學） |
| 指導教授 | 張珀銀 助理教授 |
| 實驗室 | 海事 AI 實驗室（Maritime AI Lab） |
| 專題期間 | 114-2 學期 ~ 115-1 學期 |
| 本 Repo 用途 | 培訓教材、進度追蹤、共用資源 |

## 使用方式

本 Repo 採用 **Fork + PR** 流程，和課程作業繳交方式相同：

1. **Fork** 本 Repo 到你的 GitHub 帳號
2. 在你的 Fork 中建立 `members/你的學號/` 資料夾
3. 完成培訓任務 → 放在你的 Fork
4. 每月進度報告 → 發 PR 回主 Repo
5. 老師審閱 PR → 合併或回饋

## 成員

| 姓名 | 學號 | 督導 | 角色 | 備註 |
|------|------|------|------|------|
| 王智弘 | ⚠️ 待補 | 潘其恩 | 組長 | 班代 |
| 郭柏辰 | ⚠️ 待補 | 邱麟翔 | 組員 | — |
| 郭晉銘 | ⚠️ 待補 | 潘其恩 | 組員 | — |
| 林千琪 | ⚠️ 待補 | 邱麟翔 | 組員 | 新進 RA |
| 郭韋廷 | ⚠️ 待補 | 潘其恩 | 組員 | 新進 RA |

## 培訓時程

### 第一階段：基礎能力（4 月）

| 週 | 培訓項目 | 教材 | 繳交 |
|----|---------|------|------|
| W1 | Git/GitHub 協作 | training/git-basics.md | members/學號/git-exercise.md |
| W2 | Linux 基礎 + WSL | training/linux-basics.md | members/學號/linux-exercise.md |
| W3 | Python + Pandas 入門 | training/python-basics.md | members/學號/python-exercise.md |
| W4 | 論文閱讀方法 | training/paper-reading.md | members/學號/paper-summary.md |

### 第二階段：計畫導入（5 月）

| 週 | 培訓項目 | 教材 | 繳交 |
|----|---------|------|------|
| W5 | 實驗室工具鏈（Docker + GPU） | training/lab-tools.md | members/學號/lab-setup.md |
| W6 | 依計畫分流：跟做模式啟動 | — | members/學號/weekly-log.md |
| W7 | 跟做 + 碩士生帶做 | — | members/學號/weekly-log.md |
| W8 | 跟做 + 碩士生帶做 | — | members/學號/weekly-log.md |

### 第三階段：獨立運作（6-7 月）

| 週 | 目標 | 繳交 |
|----|------|------|
| W9-W12 | 碩士生口試後，開始獨立操作 | members/學號/weekly-log.md |
| W13+ | 暑假：獨立跑實驗、處理行政 | progress/月份-進度報告.md (PR) |

## 進度報告

每月 1 號前，在你的 Fork 中建立進度報告，發 PR 繳交：

```
progress/
├── 04-進度報告.md
├── 05-進度報告.md
└── ...
```

格式見 `progress/template.md`。

## Repo 結構

```
edu-capstone-113/
├── README.md              ← 本檔案
├── training/              ← 培訓教材
│   ├── git-basics.md
│   ├── linux-basics.md
│   ├── python-basics.md
│   ├── paper-reading.md
│   └── lab-tools.md
├── progress/              ← 進度報告
│   └── template.md
├── resources/             ← 共用資源
│   └── reading-list.md
└── members/               ← 學生個人資料夾（Fork 後建立）
    └── （學號）/
        ├── profile.md
        ├── git-exercise.md
        ├── linux-exercise.md
        ├── python-exercise.md
        ├── paper-summary.md
        ├── lab-setup.md
        └── weekly-log.md
```
