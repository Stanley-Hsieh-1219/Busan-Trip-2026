# 2026 Busan Trip Planning

這是一個為 2026 年釜山家族旅遊規劃的單頁網頁應用程式 (Single Page Application)。

## 功能特色

- **行程總覽**: 每日詳細行程、交通方式、餐飲安排與備註。
- **天氣預報**: 整合 Open-Meteo API，自動顯示釜山未來七日天氣。
- **資訊整合**: 內建旅遊成員、航班住宿、行程目標、教學參考與購票連結。
- **景點集**: 包含景點與美食清單，支援關鍵字搜尋。
- **互動備註**:
    - 特殊備註欄位支援超連結自動辨識，點擊即可開啟網頁。
    - 每日行程皆可展開查看詳細內容。
- **響應式設計**: 手機與電腦皆可完美瀏覽，支援深色模式 (Dark Mode) 預備。

## 專案結構

目前專案主要由單一檔案組成：
- `index.html`: 包含所有的 HTML 結構、CSS 樣式 (Tailwind CSS)、以及 React 應用程式邏輯。

## 技術堆疊

此專案設計為無需編譯即可直接運行 (No-Build Setup)，方便快速修改與部署：
- **React 18**: 使用 UMD 版本，透過 CDN 引入。
- **Tailwind CSS**: 使用 CDN 版本進行樣式切版。
- **Babel**: 在瀏覽器端即時編譯 JSX (注意：此方式適合開發與小型專案)。
- **Lucide Icons**: 提供向量圖示。
- **Open-Meteo API**: 獲取釜山當地即時天氣資訊。

## 部署

本專案目前託管於 GitHub Pages：
[https://stanley-hsieh-1219.github.io/Busan-Trip-2026/](https://stanley-hsieh-1219.github.io/Busan-Trip-2026/)

## 如何修改

1. 直接編輯 `index.html` 檔案中的 `tripData` 物件即可更新行程內容。
2. 儲存後，將變更 commit 並 push 到 GitHub repository。
3. GitHub Pages 會自動更新 (可能需要幾分鐘)。

## 注意事項

- **天氣資訊**: 首頁的天氣預報是抓取「即時/未來七天」的釜山天氣，並非 2026 年的預測天氣。
- **本地開發**: 您可以直接用瀏覽器打開 `index.html` 進行預覽。
