# Mappin — 線上照片地圖標記工具

把照片依 EXIF 的座標與時間標在地圖上，並可手動補座標、無損寫回 JPG。純前端、單一檔案，照片不會上傳，全部在瀏覽器本機處理。

🔗 **線上版**：https://win-hs.github.io/mappin/

## 功能

- 上傳 JPG／JPEG（可複選、累加保留），自動讀取 GPS、拍攝時間、相機資訊
- 地圖上以照片 pin 顯示，鄰近自動聚合；點 pin 選取、放大檢視
- 無座標照片可從清單拖到地圖補座標
- 編輯檔名、拍攝時間、緯度、經度、海拔（含小地圖點選座標）
- 旋轉（只改 EXIF Orientation 旗標，無損）
- 勾選打包下載（zip），座標以 piexifjs **無損**寫回 JPG
- 匯出 CSV（檔名、拍攝時間、緯度、經度、海拔）
- 底圖切換：標準（OpenStreetMap）／衛星空照（Esri）／地形圖（OpenTopoMap）
- 資料存於瀏覽器 IndexedDB，重新整理後保留

## 使用方式

直接開啟 `index.html` 即可，無需安裝。所有相依套件（Leaflet、Leaflet.markercluster、exifr、piexifjs、JSZip）由 CDN 載入。

## 限制

- 僅支援 JPG／JPEG。HEIC／PNG／影片不處理。
- 瀏覽器無法覆蓋原始檔，只能下載寫好座標的新檔。
- 資料存在本機瀏覽器，換瀏覽器或清除瀏覽資料即不保留。

## 授權

MIT
