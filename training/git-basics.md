# 培訓 1：Git/GitHub 協作基礎

## 學習目標

1. 理解 Git 版本控制的基本概念
2. 熟練 clone、add、commit、push、pull 操作
3. 會使用 Fork + PR 流程繳交作業
4. 會用 Issue 追蹤工作

## 預備知識

- 已安裝 Git（`git --version` 確認）
- 已有 GitHub 帳號
- 已安裝 VS Code

## 教材

本培訓的教材直接使用課程 Repo 的內容，不重複撰寫：

| 主題 | 教材位置 |
|------|---------|
| Git 基本流程 | [114-2_BigDataCC README.md](https://github.com/pychang-ai/114-2_BigDataCC#git-基本流程) |
| Git 基本指令 | [114-2_BigDataCC README.md](https://github.com/pychang-ai/114-2_BigDataCC#git-基本指令) |
| 小組協作指南 | [project-template collaboration-guide.md](https://github.com/pychang-ai/114-2_BigDataCC-project-template/blob/main/collaboration-guide.md) |
| 小組協作練習 | [project-template collaboration-exercise.md](https://github.com/pychang-ai/114-2_BigDataCC-project-template/blob/main/collaboration-exercise.md) |

## 練習作業

完成以下任務，將結果放在你的 Fork 的 `members/你的學號/git-exercise.md`：

```markdown
# Git 練習

## 基本資訊

| 項目 | 內容 |
|------|------|
| 姓名 | （填入） |
| 學號 | （填入） |
| GitHub 帳號 | （填入） |
| 完成日期 | （填入） |

## 練習 1：Fork 並 Clone

請描述你完成以下步驟的過程：
1. Fork 本 Repo（edu-capstone-113）
2. Clone 到本機
3. 建立 members/你的學號/ 資料夾

（描述過程，貼上你使用的指令）

## 練習 2：建立 profile.md 並 Push

在 members/你的學號/ 中建立 profile.md，包含：
- 姓名、學號
- 為什麼加入海事 AI 實驗室
- 你最想學的技能

Push 後貼上 git log --oneline -3 的結果：
（貼上結果）

## 練習 3：發 PR

發一個 PR 將你的 profile.md 繳交回主 Repo。
PR 標題格式：學號_姓名_git-exercise

貼上你的 PR 網址：
（貼上）

## 練習 4：觀察 commit 紀錄

執行以下指令並貼上結果：
git log --oneline -5
git shortlog -sn

（貼上結果）
```

## 完成標準

- [ ] 成功 Fork 並 Clone 本 Repo
- [ ] 建立 members/學號/profile.md 並 Push
- [ ] 建立 members/學號/git-exercise.md 並 Push
- [ ] 發 PR 繳交，標題格式正確
