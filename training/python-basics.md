# 培訓 3：Python + Pandas 入門

## 學習目標

1. 在 WSL 或本機建立 Python 開發環境
2. 使用 Pandas 讀取、清洗、分析資料
3. 使用 Matplotlib 產出基本圖表
4. 使用 Jupyter Notebook 做互動式分析

## 預備知識

- 已完成 Linux 培訓
- 已安裝 VS Code

## 環境建置

```bash
# 安裝 Miniconda（WSL 或 Linux）
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh

# 建立專用環境
conda create -n capstone python=3.10 -y
conda activate capstone

# 安裝套件
pip install pandas numpy matplotlib seaborn jupyter
```

## 教材

| 主題 | 教材/資源 |
|------|---------|
| Python 基礎語法 | [W3Schools Python](https://www.w3schools.com/python/) |
| Pandas 入門 | [Pandas Getting Started](https://pandas.pydata.org/docs/getting_started/index.html) |
| Matplotlib 入門 | [Matplotlib Tutorials](https://matplotlib.org/stable/tutorials/index.html) |

## 練習作業

完成以下任務，將結果放在 `members/你的學號/python-exercise.md`：

```markdown
# Python + Pandas 練習

## 基本資訊

| 項目 | 內容 |
|------|------|
| 姓名 | （填入） |
| 學號 | （填入） |
| 完成日期 | （填入） |
| Python 版本 | （python --version 的結果） |

## 練習 1：環境確認

conda activate capstone
python --version
pip list | grep -E "pandas|numpy|matplotlib"

（貼上結果）

## 練習 2：Pandas 資料操作

撰寫一個 Python 程式，完成以下任務：
1. 用 Pandas 建立一個 DataFrame，包含至少 5 筆資料（主題自選，例如：船舶資料、氣象資料）
2. 顯示 DataFrame 的 shape、dtypes、describe()
3. 篩選出符合某條件的資料（例如：速度 > 10 的船舶）
4. 新增一個計算欄位

貼上你的程式碼和執行結果：
（貼上）

## 練習 3：讀取 CSV 檔案

1. 到政府開放資料平台（data.gov.tw）下載一個和海事/海洋相關的 CSV 檔案
2. 用 pd.read_csv() 讀取
3. 顯示前 5 筆資料
4. 檢查有沒有缺失值（isnull().sum()）
5. 做一個簡單的統計分析（例如：groupby 後計算平均值）

資料來源網址：
（貼上）

程式碼和結果：
（貼上）

## 練習 4：視覺化

用上一題的資料，產出至少 2 張圖表：
1. 一張折線圖或長條圖
2. 一張其他類型的圖（散佈圖、圓餅圖、熱力圖等）

將圖表儲存為 PNG 檔案，放在 members/你的學號/ 資料夾中。

使用的程式碼：
（貼上）

圖表檔名：
（列出）
```

## 完成標準

- [ ] Python + Pandas 環境建置成功
- [ ] DataFrame 建立和基本操作完成
- [ ] 成功讀取外部 CSV 檔案並分析
- [ ] 產出至少 2 張視覺化圖表（PNG 檔案附在 Fork 中）
