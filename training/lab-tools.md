# 培訓 5：實驗室工具鏈

## 學習目標

1. 使用 SSH 連線到實驗室 GPU 主機
2. 理解 Docker 容器的基本概念和操作
3. 使用 nvidia-smi 確認 GPU 狀態
4. 在 GPU 主機上執行 Python 程式

## 預備知識

- 已完成 Linux 培訓和 Python 培訓
- 老師已分配 GPU 主機帳號

## SSH 連線

```bash
# 從 WSL 或 Terminal 連線
ssh 你的帳號@主機IP

# 確認連線成功
hostname
whoami
nvidia-smi
```

### SSH 金鑰設定（免密碼登入）

```bash
# 1. 在本機產生金鑰（如果還沒有）
ssh-keygen -t ed25519 -C "你的email"

# 2. 將公鑰複製到主機
ssh-copy-id 你的帳號@主機IP

# 3. 測試免密碼登入
ssh 你的帳號@主機IP
```

## Docker 基礎

### 為什麼用 Docker？

每個人的電腦環境不同（Python 版本、套件版本），容易遇到「在我電腦可以跑」的問題。Docker 建立統一的執行環境，確保程式在任何地方都能跑。

### 常用指令

```bash
# 查看有哪些映像檔
docker images

# 查看正在執行的容器
docker ps

# 啟動一個 Python 容器
docker run -it python:3.10 bash

# 在容器中安裝套件
pip install pandas numpy

# 離開容器
exit
```

### 使用 GPU 的 Docker

```bash
# 啟動帶 GPU 的容器
docker run --gpus all -it nvidia/cuda:12.1.0-base-ubuntu22.04 bash

# 確認容器內可以看到 GPU
nvidia-smi
```

## 練習作業

完成以下任務，將結果放在 `members/你的學號/lab-setup.md`：

```markdown
# 實驗室工具鏈練習

## 基本資訊

| 項目 | 內容 |
|------|------|
| 姓名 | （填入） |
| 學號 | （填入） |
| 分配的主機 | （填入 IP 或主機名稱） |
| 完成日期 | （填入） |

## 練習 1：SSH 連線

ssh 你的帳號@主機IP
hostname
whoami

（貼上結果）

## 練習 2：確認 GPU

nvidia-smi

（貼上結果）
你的主機有什麼 GPU？顯存多少？

## 練習 3：Docker 基本操作

docker images | head -5
docker ps -a | head -5

（貼上結果）

## 練習 4：在主機上執行 Python

# 建立一個簡單的測試程式
cat > ~/test_gpu.py << 'EOF'
import sys
print(f"Python version: {sys.version}")
try:
    import torch
    print(f"PyTorch version: {torch.__version__}")
    print(f"CUDA available: {torch.cuda.is_available()}")
    if torch.cuda.is_available():
        print(f"GPU: {torch.cuda.get_device_name(0)}")
except ImportError:
    print("PyTorch not installed")
EOF

python3 ~/test_gpu.py

（貼上結果）

## 練習 5：SSH 金鑰設定

設定免密碼登入後，確認可以不輸入密碼就連線：
ssh 你的帳號@主機IP "echo 連線成功"

（貼上結果）
```

## 完成標準

- [ ] SSH 連線到實驗室主機成功
- [ ] nvidia-smi 確認 GPU 可用
- [ ] Docker 基本指令可執行
- [ ] Python 程式在主機上執行成功
- [ ] SSH 金鑰免密碼登入設定完成
