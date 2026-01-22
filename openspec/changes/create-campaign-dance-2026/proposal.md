# 變更提案：建立 2026 會員召集舞夠有禮 活動頁面

## 原因 (Why)
配合國泰產險 2026 年行銷活動「會員召集舞夠有禮」，需建立一個全新的靜態活動頁面。
該活動旨在透過舞蹈挑戰與豐富獎品（Switch 2, Dyson, Marshall），吸引使用者註冊會員並參與社群互動。
活動期間預計為：2026/03/18 - 04/12。

## 變更內容 (What Changes)
- **建立新目錄**: `new-campaign-2026/` (暫定名稱，避免混淆)。
- **實作頁面**: 基於提供的 `page-reference.jpg` 視覺設計，參考 `old-project` 的技術實作（Tailwind, Header/Footer），但進行程式碼優化。
- **功能區塊**:
  1. **主視覺 (Hero)**: 包含標題、活動時間、CTA 按鈕。
  2. **活動步驟 (Steps)**: 三步驟教學（學舞、註冊、分享）。
  3. **誘因與教學 (Incentives)**: LINE POINTS 100點、舞蹈教學影片連結。
  4. **MV 專區 (Video)**: 嵌入 YouTube 影片或 HTML5 Video。
  5. **獎品展示 (Prizes)**: 頭獎 Switch 2、二獎 Dyson、三獎 Marshall。
  6. **活動辦法 (Rules)**: 詳細規則說明條款。

## 影響範圍 (Impact)
- 新增靜態檔案與資源。
- 不影響現有 `old-project` 運作。
- 需確保與國泰產險現有 Header/Footer 樣式相容。
