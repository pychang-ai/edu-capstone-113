# Git 練習

## 基本資訊

| 項目 | 內容 |
|------|------|
| 姓名 | 郭晉銘 |
| 學號 | 113181144 |
| GitHub 帳號 | mycowbei69 |
| 完成日期 | 2026/4/2 |

## 練習 1：Fork 並 Clone

請描述你完成以下步驟的過程：
1. Fork 本 Repo（edu-capstone-113）
2. Clone 到本機
3. 建立 members/你的學號/ 資料夾

1.透過老師船的GitHub的連結，並按fork到我的GitHub裡面。
2.透過這3個指令clone到本機。
  git config --global user.name "mycowbei69"
  git config --global user.email "C113181144@nkust.edu.tw"   
  git clone https://github.com/mycowbei69/edu-capstone-113
3.利用「mkdir members/C113181144」來建立資料夾。

## 練習 2：建立 profile.md 並 Push

在 members/你的學號/ 中建立 profile.md，包含：
- 姓名、學號
- 為什麼加入海事 AI 實驗室
- 你最想學的技能

- 1.姓名:郭晉銘，學號:C113181144
- 2.為什麼加入海事 AI 實驗室: 因為對AI相關技術與知識感興趣，提升自己資訊相關的能力。
- 3.你最想學的技能:利用AI的能力，熟悉各種AI模型。

Push 後貼上 git log --oneline -3 的結果：
（貼上結果）
PS C:\Users\User\OneDrive\Desktop\githubpractice\edu-capstone-113> git log --oneline -3
dfcfa7f (HEAD -> main, origin/main, origin/HEAD) firsttest
4bb4729 update: 培訓週次對齊學期週次（W6–W18+）
a34efa8 add: 113屆專題成員名單（5人，組長王智弘）

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
