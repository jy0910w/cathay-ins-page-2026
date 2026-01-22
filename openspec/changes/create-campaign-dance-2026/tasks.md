## 1. 專案建置與結構優化
- [x] 1.1 建立專案目錄結構 `new-campaign-2026/` (含 `css/`, `js/`, `images/`)
- [x] 1.2 引入 `static/cathay/` 共用資源 (Header, Footer, Tailwind 設定)
- [x] 1.3 **優化：** 建立語意化的 HTML 骨架 (`<header>`, `<main>`, `<section>`, `<footer>`)，避免 `div` 湯

## 2. 頁面區塊實作 (依視覺動線)
- [x] 2.1 **主視覺區 (Hero Section)**
    - 實作標題與人物插圖佈局
    - 實作「了解任務」、「看看大獎」CTA 按鈕
- [x] 2.2 **步驟引導區 (Steps Section)**
    - 實作「步驟 1/2/3」卡片佈局
    - 實作步驟間的箭頭指引設計
    - 實作對應的行動呼籲按鈕區塊
- [x] 2.3 **行銷誘因區 (Incentive Banner)**
    - 實作「新會員獲得 LINE POINTS」的橫幅視覺
- [x] 2.4 **影音專區 (Video Section)**
    - 實作「簡單點！國泰產險Online MV」標題
    - 嵌入響應式影片播放器
- [x] 2.5 **獎品展示區 (Prize Section)**
    - 實作獎品卡片 (Switch 2, Dyson, Marshall)
    - 確保手機版與桌機版的響應式排版 (Grid/Flex)
    - 實作底部 CTA 按鈕組
- [x] 2.6 **活動辦法區 (Rules Section)**
    - 實作條款文字排版
    - 確保可讀性與清單樣式正確

## 3. 樣式與互動優化
- [x] 3.1 **優化：** 重構 CSS 策略
    - 優先使用 Tailwind Utility Classes 處理佈局 (Layout) 與間距 (Spacing)
    - 僅將特殊視覺效果 (漸層、特殊圓角、裝飾圖) 寫入 `custom.css`
- [x] 3.2 **優化：** 圖片資源管理
    - 使用佔位圖片 (Placeholders) 先行切版，並標註圖片尺寸需求
    - 確保圖片具備 `alt` 屬性 (無障礙優化)
- [x] 3.3 **優化：** JavaScript 模組化
    - 避免全域變數汙染，使用 IIFE 或 ES Modules 封裝活動邏輯
