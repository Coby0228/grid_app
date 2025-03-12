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
docker-compose up
```

3. 在瀏覽器中訪問 `http://localhost:5000`

### 手動構建和運行Docker容器

1. 構建Docker映像：

```bash
docker build -t grid-app .
```

2. 運行容器：

```bash
docker run -p 5000:5000 grid-app
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

## 目錄結構

```
.
├── app.py              # Flask應用入口
├── templates/          # HTML模板
│   └── index.html      # 主頁面
├── Dockerfile          # Docker配置
├── docker-compose.yml  # Docker Compose配置
└── requirements.txt    # Python依賴
```

## 使用方法

1. 輸入網格尺寸（3-10）並點擊「生成網格」按鈕
2. 點擊某個單元格設置為起點（綠色）
3. 點擊另一個單元格設置為終點（紅色）
4. 點擊其他單元格設置障礙物（灰色），最多可設置n-2個
5. 點擊「生成策略與價值」按鈕來產生策略和價值評估