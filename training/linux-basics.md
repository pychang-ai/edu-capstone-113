# 培訓 2：Linux 基礎 + WSL

## 學習目標

1. 在 WSL 環境中操作 Linux 基本指令
2. 理解檔案權限與使用者管理
3. 會使用 SSH 連線到遠端主機
4. 理解 WSL 與 Windows 的檔案互通

## 預備知識

- 已安裝 WSL（Ubuntu）
- 已完成 Git 培訓

## 教材

| 主題 | 教材位置 |
|------|---------|
| Linux 指令、權限、目錄結構 | [114-2_BigDataCC week06/lecture.md](https://github.com/pychang-ai/114-2_BigDataCC/blob/main/week06/lecture.md) |
| WSL 操作 | 同上（第六部分） |
| Linux 常用指令 | [114-2_BigDataCC week04/README.md](https://github.com/pychang-ai/114-2_BigDataCC/blob/main/week04/README.md) |
| nano + Shell Script | [114-2_BigDataCC week05/lecture.md](https://github.com/pychang-ai/114-2_BigDataCC/blob/main/week05/lecture.md) |

## 練習作業

完成以下任務，將結果放在 `members/你的學號/linux-exercise.md`：

```markdown
# Linux 練習

## 基本資訊

| 項目 | 內容 |
|------|------|
| 姓名 | （填入） |
| 學號 | （填入） |
| 完成日期 | （填入） |

## 練習 1：WSL 環境確認

執行以下指令並貼上結果：
wsl --version（在 PowerShell 執行）
uname -a（在 WSL 執行）
whoami
id

（貼上結果）

## 練習 2：基本指令操作

在 WSL 中依序執行並貼上結果：

# 建立目錄結構
mkdir -p ~/capstone/data ~/capstone/code ~/capstone/docs
tree ~/capstone（如果沒有 tree，用 ls -R ~/capstone）

# 建立檔案
echo "My Capstone Project" > ~/capstone/README.txt
cat ~/capstone/README.txt

# 查看系統資訊
df -h | head -5
du -sh ~

（貼上結果）

## 練習 3：檔案權限

# 查看權限
ls -l ~/capstone/README.txt

# 改權限
chmod 755 ~/capstone/README.txt
ls -l ~/capstone/README.txt

chmod 644 ~/capstone/README.txt
ls -l ~/capstone/README.txt

（貼上每步結果，說明權限的變化）

## 練習 4：SSH 連線到實驗室主機

（此題待老師提供主機 IP 和帳號後完成）
ssh 你的帳號@主機IP
uname -a
nvidia-smi（如有 GPU）

（貼上結果）

## 練習 5：WSL 與 Windows 檔案互通

# 從 WSL 查看 Windows 桌面
ls /mnt/c/Users/你的帳號/Desktop/ | head -5

# 從 WSL 建立檔案到 Windows 桌面
echo "Created from WSL" > /mnt/c/Users/你的帳號/Desktop/wsl-test.txt

# 確認
cat /mnt/c/Users/你的帳號/Desktop/wsl-test.txt

# 清理
rm /mnt/c/Users/你的帳號/Desktop/wsl-test.txt

（貼上結果）
```

## 完成標準

- [ ] WSL 環境確認正常
- [ ] 基本指令操作完成
- [ ] 理解檔案權限並能解讀 ls -l 輸出
- [ ] SSH 連線成功（待老師提供帳號）
- [ ] WSL 與 Windows 檔案互通測試完成
