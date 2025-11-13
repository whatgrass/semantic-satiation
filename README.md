# 語義飽和實驗 (Semantic Satiation Experiment)

這是一個使用 jsPsych 建立的語義飽和實驗網頁。

## 功能說明

- 誘導階段：重複顯示主題詞 10 次
- 測試階段：判斷兩個目標詞是否都屬於該主題類別
- 自動記錄反應時間和正確率
- 實驗結束後自動下載 CSV 數據檔案

## 如何使用

### 本地測試
1. 雙擊 `啟動實驗.bat` 啟動本地伺服器
2. 或使用 Python: `python -m http.server 8000`
3. 在瀏覽器開啟 `http://localhost:8000`

### 線上部署（GitHub Pages）

1. **建立 GitHub 儲存庫**
   - 登入 GitHub
   - 點擊右上角 "+" → "New repository"
   - 命名為 `semantic-satiation-experiment`（或您喜歡的名稱）
   - 選擇 Public（GitHub Pages 免費版需要公開儲存庫）
   - 點擊 "Create repository"

2. **上傳檔案**
   - 使用 GitHub Desktop：
     - 開啟 GitHub Desktop
     - 點擊 "File" → "Add Local Repository"
     - 選擇此資料夾
     - 輸入 commit 訊息（例如："Initial commit"）
     - 點擊 "Publish repository"
   
   - 或使用命令列：
     ```bash
     git init
     git add index.html README.md
     git commit -m "Initial commit"
     git branch -M main
     git remote add origin https://github.com/您的帳號/semantic-satiation-experiment.git
     git push -u origin main
     ```

3. **啟用 GitHub Pages**
   - 在 GitHub 儲存庫頁面，點擊 "Settings"
   - 左側選單找到 "Pages"
   - 在 "Source" 選擇 "Deploy from a branch"
   - 選擇 "main" 分支和 "/ (root)" 資料夾
   - 點擊 "Save"
   - 等待幾分鐘，GitHub 會提供網址：`https://您的帳號.github.io/semantic-satiation-experiment/`

## 檔案說明

- `index.html` - 主要的實驗網頁
- `README.md` - 本說明檔案
- `啟動實驗.bat` - Windows 批次檔，用於本地測試
- `啟動實驗.ps1` - PowerShell 腳本，用於本地測試

## 注意事項

- 實驗需要網路連線（載入 jsPsych 庫）
- 建議使用 Chrome 或 Edge 瀏覽器
- 實驗數據會自動下載為 CSV 格式

