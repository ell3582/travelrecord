行程規劃 App (Okinawa Trip Planner)

這是一個使用純 HTML、JavaScript 和 Tailwind CSS 開發的單頁應用程式（SPA），用於多人協作規劃旅行行程。

核心功能

實時協作： 行程數據儲存在 Firestore 資料庫中，所有用戶（透過同一個 Canvas 環境）都可以即時看到更新。

響應式設計： 介面專為移動設備優化，方便旅行中隨時查看。

按日分類： 輕鬆切換和查看不同日期的行程。

快速導航： 每個行程項目都包含 Google 地圖連結，可直接開啟導航。

自帶認證： 使用 Canvas 提供的自定義 Token 進行認證，保證數據安全。

如何運行 (How to Run)

由於這個 App 依賴於一個特殊的 Canvas 環境變量 (__app_id, __firebase_config, __initial_auth_token) 進行 Firestore 初始化和認證，它不能在本地直接運行。

如果您想在本地預覽介面，您必須替換 index.html 中 Firebase 相關的全局變量為模擬數據，或者在一個支持 Firebase 環境變量注入的平台上運行。

項目文件

index.html: 包含所有 HTML, CSS, JavaScript (包括 Firebase 邏輯) 的單一檔案。

Powered by Gemini
