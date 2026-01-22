# 專案情境 (Project Context)

## 目的 (Purpose)
**國泰產險 (Cathay Insurance) - 簡單點！(Simple Point!) 活動**
本專案是國泰產險「簡單點！」活動 (2025/02/11 ~ 04/30) 的推廣網站。活動旨在鼓勵使用者：
1. 加入國泰產險會員。
2. 預約車險到期提醒（「車險小秘書」）。
完成這些任務的使用者可獲得抽獎機會，獎品包括 RIMOWA 行李箱和 Marshall 藍牙喇叭。

## 技術堆疊 (Tech Stack)
- **前端:** HTML5, CSS3, JavaScript (ES5/ES6 混合)。
- **CSS 框架:**
  - Tailwind CSS (推測自 `tw-` 前綴)。
  - 自定義 CSS (`static/cathay/*.css`, `old-project/css/20250116.css`)。
- **函式庫:**
  - jQuery (v1.x/2.x，由 `jquery-ui` 和舊有模式推測)。
  - Swiper.js (用於輪播)。
  - RequireJS (模組載入)。
  - Skrollr (視差捲動)。
- **分析與行銷:**
  - Google Analytics (GA4/GTM)。
  - Meta Pixel。
  - Celebrus (程式碼中引用)。
- **後端:** 無 (靜態網站服務)。表單提交至 `https://www.cathay-ins.com.tw/...`。

## 專案慣例 (Project Conventions)

### 程式碼風格 (Code Style)
- **HTML:** 語意化 HTML5，大量使用工具類別 (`tw-*`)。
- **CSS:**
  - 共用樣式位於 `static/cathay/`。
  - 活動專屬樣式位於 `old-project/css/`。
  - 工具類別前綴為 `tw-` 以避免衝突。
- **JavaScript:**
  - 全域腳本位於 `static/cathay/`。
  - 活動邏輯位於 `old-project/js/`。
  - 使用 `document.addEventListener('PageReady', ...)` 進行初始化。

### 架構模式 (Architecture Patterns)
- **靜態網站:** 專案結構扁平，HTML 檔案位於 `old-project/` 根目錄，資源位於子目錄。
- **資源分離:**
  - `static/cathay/`: 企業共用資源（頁首、頁尾、共用函式庫）。
  - `old-project/{images,css,js}`: 活動專屬資源。

### Git 工作流程 (Git Workflow)
- [待使用者定義 - 建議使用標準功能分支工作流程]

## 領域情境 (Domain Context)
- **保險產品:** 汽車險、旅遊險、寵物險等。
- **活動機制:** 使用者必須完成特定動作（註冊、預約）以獲得「抽獎機會」。
- **法規:** 條款與細則至關重要，必須顯示（例如：「活動注意事項」區塊）。

## 外部相依性 (External Dependencies)
- **國泰系統:**
  - `besafe.cathay-ins.com.tw` (產品頁面)。
  - `www.cathay-ins.com.tw` (表單提交、登入)。
- **CDN:** Google Fonts, GTM, Facebook Pixel。
