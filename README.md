# 🦒 麒麟鹿player (Ki-lin-lok uan-ka)

> 專為實體英語教科書課後複習打造的極簡隨身聽 · 雙欄位純數字輸入 · 手機大數字鍵盤 · GitHub Pages 零配置即開即播

### 🌐 線上即用網址 (Live Demo)
👉 **[https://vaalrl.github.io/Ki-lin-lok-uan-ka/](https://vaalrl.github.io/Ki-lin-lok-uan-ka/)**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Online%20(即開即用)-brightgreen?style=for-the-badge&logo=github)](https://vaalrl.github.io/Ki-lin-lok-uan-ka/)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Active-blue?style=for-the-badge)](https://vaalrl.github.io/Ki-lin-lok-uan-ka/)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-0%20(Pure%20Vanilla)-success)](#)
[![Mobile Optimized](https://img.shields.io/badge/Mobile-iOS%20%2F%20Android-orange)](#)

---

## 📖 專案簡介 (Introduction)

**麒麟鹿player** 是一個單檔純前端（Single-file Vanilla Web App）的輕量級音訊播放器，專門解決學童與家長在課後複習實體英語教材時，原廠掃描介面繁瑣、操作不便、按鈕過小的痛點。

使用者只需翻開正版實體課本，依照內頁印製的課次與曲目號碼（如 `1-1`、`3-2`），在手機上直接鍵入數字，即可一鍵直連播放對應音軌，支援單曲循環、連續播放與語音變速，讓課後跟讀與聽力練習變得無比流暢。

---

## ✨ 核心特色 (Key Features)

### 1. 📱 手機觸控極致優化
- **雙格切分純數字輸入**：將「幾之幾」切分為 `[ 課次 (Lesson) ] — [ 曲目 (Track) ]` 兩個獨立欄位，中間自動連接橫槓，**徹底免除手動輸入標點符號的麻煩**。
- **強制喚出純數字九宮格鍵盤**：雙欄位均配置 `inputmode="numeric"` 與 `pattern="[0-9]*"`，在 iPhone (iOS Safari) 與 Android (Chrome) 上點擊**直接彈出全螢幕大按鈕純數字鍵盤**。
- **點擊即全選與自動換格**：點擊欄位自動全選現有數值，輸入課次後游標自動跳至曲目格，按下 Enter 直接發動播放。

### 2. 🎵 專業洗鍊的極簡控制面板
- **純圖示控制按鈕（零文字干擾）**：
  - `⏮` **上一首**（跨冊自動退回上一本最後一首）
  - `↺5s` **快退 5 秒**（即時重聽上一句英語會話）
  - `( ▶ / ⏸ )` **中央大播放鍵**（狀態自動切換）
  - `5s↻` **快進 5 秒**（快速略過已知段落）
  - `⏭` **下一首**（跨冊自動進入下一本第一首）
- **核取方塊（Checkbox）模式控制**：
  - `☑ 🔁` **單曲循環**：打勾即可鎖定單首精聽跟讀。
  - `☑ ⏩` **接續播放**：打勾即可一首播完自動播放下一首（磨耳朵首選）。
- **英語聽力倍速切換**：提供 `0.8x（初學慢速）`、`1.0x（原速）`、`1.2x（挑戰聽力）` 即時無損變速。

### 3. 📚 涵蓋 28 大系列、221 本教材完整書庫
- 🌟 **旗艦主教材**：Action (1~8 冊)、Bingo Phonics (1~4 冊)、Stage (1~5 冊)、Highlight (1~5 冊)、Get Ready (1~4 冊)。
- 👶 **幼兒啟蒙與成長**：Hello Giraffe (10 冊)、Go! Go! Giraffe (10 冊)、Caterpillar (12 冊)、Bravo Giraffe (10 冊)、WOW! Starter (3 冊)、WOW! Little Sun (24 冊) 等。
- 🚀 **進階少兒與青少**：WOW! Big Sky (24 冊)、WOW! Reach Your Goal (24 冊/CD)、Twinkle (30 冊/CD)、Giraffe Leaders (3 冊)。
- 📖 **自然發音與主題**：Giraffe Phonics (8 冊)、Children's Favorite Stories (9 冊)、My G-Book (8 冊)、KK 音標、My ABC、My 123 等。

### 4. 🔍 雲端曲目清單抽屜
- 點擊「▼ 展開曲目清單」，即可瀏覽該本書籍的所有真實歌曲標題（如 `Opening`、`Dialogue`、`Chant` 等）。
- 內建即時關鍵字搜尋框，點擊任一曲目即刻跳轉播放。

### 5. 🌗 長頸鹿美語官方品牌色系與深淺雙模式
- **官方 CI 視覺傳承**：取樣官方標準招牌亮橘（`#ff8800`）、溫暖蜜桃奶白與可可大地深木色調。
- **一鍵切換與快取持久化**：右上角提供深色（🌙）/ 淺色（☀️）無縫切換，設定自動保存於瀏覽器 `localStorage`，隨開即用不閃爍。

### 6. 🎧 Media Session API 行動鎖屏與耳機線控
- **鎖定螢幕教材顯示**：手機鎖屏或下拉通知列可直接看見長頸鹿專屬 App 圖示、教材系列、冊次與曲目名稱。
- **AirPods / 藍牙耳機線控**：支援耳機實體按鍵直接進行「播放 / 暫停」、「下一首」、「上一首」與「快退 5 秒」精聽操作。

### 7. 🔗 網址即時同步與一鍵複製分享 (Deep Linking)
- 播放時瀏覽器網址列自動同步當前進度（如 `?s=AC&b=BOOK1&t=1-1`）。
- 提供「📋 複製本曲分享連結」按鈕，家長或教師可一鍵複製專屬直連網址傳至 LINE，對方點開即可精準載入該課該曲。

### 8. ⚡ 零相依單檔架構
- 100% 原生 HTML5 + CSS3 + Vanilla JavaScript。
- **無任何外部相依套件**（No jQuery, No React, No CDN libraries），體積僅約 40KB，完全離線/本地亦可執行。

---

## 🚀 快速上手指南 (Quick Start)

### 方式 A：透過 GitHub Pages 直接使用（全家手機隨開即用）
 
- 🌐 **已部屬上線，點擊即用**：[https://vaalrl.github.io/Ki-lin-lok-uan-ka/](https://vaalrl.github.io/Ki-lin-lok-uan-ka/)
- 本專案已配置 GitHub Pages 自動託管，每次更新 `main` 分支將自動同步最新版本。
- 📱 **在手機上建立 App 圖示（推薦）**：
   - **iPhone (iOS)**：用 Safari 開啟該網址 ➔ 點擊底部「分享」圖示 ➔ 點選 **「加入主畫面」**。
   - **Android**：用 Chrome 開啟 ➔ 點擊右上角選單 ➔ 點選 **「加到主螢幕」**。
   - 桌面即會生成一個全螢幕獨立運行的隨身聽圖示！

### 方式 B：單一檔案手機本機執行（100% 離線私密）

1. 直接將本專案中的 `index.html` 透過通訊軟體、AirDrop 或傳輸線放進手機。
2. **Android**：以檔案管理員開啟 ➔ 選擇「Chrome」瀏覽器開啟。
3. **iPhone**：儲存至「檔案」後，使用免費的 **Documents by Readdle** 或支援 HTML 檢視的瀏覽工具開啟。

---

## ⚖️ 免責聲明與合理使用聲明 (Legal Disclaimer & Fair Use)

本專案之開發與開源僅作為**個人家庭課後自主學習與無障礙介面優化之技術研究用途**。請詳閱完整的 [DISCLAIMER.md](DISCLAIMER.md)：

1. **非營利教育輔助性質**：本專案為開源非商業專案，不收取任何費用，無任何廣告、贊助或商業盈利行為。
2. **非官方與無關聯宣告**：本專案為個人獨立開發之第三方工具，與「長頸鹿美語」或任何特定出版機構無任何官方合作、代言、商業隸屬或授權關係。
3. **無伺服器端音訊託管**：本專案 Repository **未儲存、未複製、未託管、亦未散布** 任何具版權之音訊實體檔案。所有音訊資源均由使用者客戶端瀏覽器直接與公開之雲端 CDN 進行連線。
4. **實體教材必備性與正版倡議**：本工具播放之音軌多為課堂練習指令與聽力配合題，**若無配合正版實體課本，實質上無法產生學習輔助效果**。本專案強烈呼籲並倡導使用者購買合法正版之紙本教材。
5. **著作權歸屬**：所有相關教材內容、錄音、圖片與商標之智慧財產權，均歸原出版機構或其權利人所有。

---

## 📄 開源授權 (License)

本專案程式碼基於 [MIT License](LICENSE) 條款開源發布。
