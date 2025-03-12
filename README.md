# n x n 網格地圖應用

這是一個基於Flask的網格地圖應用，實現了強化學習中的策略評估演算法。

## 功能

- 生成可自定義大小的網格（3x3 到 10x10）
- 設置起點（綠色）和終點（紅色）
- 添加障礙物（灰色）
- 生成隨機策略
- 計算並顯示每個單元格的價值

## 使用Docker運行

### 使用Docker Compose (推薦)

1. 確保已安裝Docker和Docker Compose
2. 在專案根目錄下運行：

```bash
cd grid_app
docker-compose up -d
```

3. 在瀏覽器中訪問 `http://localhost:5000`


## 本地運行（不使用Docker）

1. 安裝依賴：

```bash
pip install -r requirements.txt
```

2. 運行應用：

```bash
python app.py
```

3. 在瀏覽器中訪問 `http://localhost:5000`
