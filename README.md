# Threads 破圖修復插件 (Threads CORS Fixer)

這是一個微型的 Chrome Extension，用於修復 Threads 網頁版因為 Meta CORS 設定疏漏導致的圖片無法顯示（破圖）問題。

## 原理
利用 Chrome Declarative Net Request API，在瀏覽器端針對 `threads.net` 發出的圖片請求，強制補上 `Access-Control-Allow-Origin: *` Header。

## 安裝方法
1. 下載此專案 (Code -> Download ZIP) 並解壓縮。
2. 開啟 Chrome 瀏覽器，進入 `chrome://extensions/`。
3. 開啟右上角「開發人員模式 (Developer mode)」。
4. 點擊左上角「載入未封裝項目 (Load unpacked)」。
5. 選擇解壓縮後的資料夾。
6. 回到 Threads 重新整理即可。