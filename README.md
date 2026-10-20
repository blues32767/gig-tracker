# 聽團網 TING TUAN — 下一場，在現場見。

<p align="center">
  <img src="https://img.shields.io/badge/%E8%81%BD%E5%9C%98%E7%B6%B2-Live%20Gig%20Tracker-d4f55a?style=for-the-badge&logoColor=111111&labelColor=111111" alt="聽團網 TING TUAN">
  <br>
  <strong>INDEPENDENT MUSIC FIELD NOTES / TAIWAN</strong>
  <br>
  <em>從第一首到最後一次安可，把喜歡的現場，排進你的生活節奏。</em>
</p>

<p align="center">
  <a href="https://blues32767.github.io/gig-tracker/"><img src="https://img.shields.io/badge/Live_Demo-線上體驗網站-111111?style=flat-square&logo=githubpages&logoColor=d4f55a" alt="Live Demo"></a>
  <img src="https://img.shields.io/badge/Style-Neo--Brutalism-black?style=flat-square" alt="Style">
  <img src="https://img.shields.io/badge/Platform-Web%20%7C%20Mobile%20Optimized-16a34a?style=flat-square" alt="Platform">
  <img src="https://img.shields.io/badge/Sync-Google%20Apps%20Script-4285F4?style=flat-square&logo=google" alt="Sync">
</p>

---

## 📖 專案簡介

[聽團網 (ting-tuan)](https://blues32767.github.io/gig-tracker/) 是一個專為台灣獨立音樂樂迷與現場聽團仔量身打造的 **現代化演出時程探索與個人參戰足跡 Web App**。

結合跨樂團演出行事曆、歷史場次歌單（Setlist）、台灣雙模現場地圖，以及免帳號密碼的 Google 雲端無縫同步機制，讓樂迷隨時掌握全台 Livehouse、音樂祭與專場動態，輕鬆記錄每一趟熱血奔赴的現場記憶。

---

## 🌟 核心特色與功能亮點

### 1. 🎨 Neo-Brutalism 潮流新野獸派美學
- **高對比幾何美學**：以俐落黑框（`2px solid #111`）、粗體字體、深硬陰影與高識別度的螢光萊姆黃（`#d4f55a`）跳色呈現。
- **全站深色模式（Dark Mode）**：支援一鍵切換日/夜間模式，搭配極簡細網格底紋（Hero Grid），夜間看演出排程不刺眼。
- **行動優先（Mobile-First）**：全面針對手機垂直視窗與 iOS Safe-Area 進行動態高度鎖定，軟鍵盤彈出自動優化。

### 2. 🎛️ 智慧雙軌篩選與左右滑軌系統（Dual-Track Stream）
- **第一軌（主控列）**：常駐「全部」、「自訂分組膠囊」與「挑選藝人/分組」。
- **第二軌（成員左右滑軌）**：當分組內有十幾甚至數十組藝人時，自動轉化為**單排平滑橫向滾動軌道**，並帶有優雅的右側微淡出漸層提示（Gradient Fade）。
- **徹底告別版面膨脹**：將篩選列垂直高度鎖定在極致的雙排之內，絕不推擠下方核心演出清單。

### 3. 📁 自訂藝人分組（Custom Artist Groups）
- 支援建立多達 **8 組個人專屬分類**（例如：「女偶像」、「獨立龐克」、「今年必看」等）。
- 彈窗工作區內一鍵增減成員，首頁膠囊秒切專屬組別時間表，快速掌握本命樂團動向。

### 4. 🗺️ 台灣現場足跡版圖（雙模地圖切換）
- **向量手繪 SVG 台灣島嶼圖**：獨家手繪全台縣市節點，依各城市演出場次動態顯示「呼吸脈衝光暈（Pulse）」與即時側邊預覽清單。
- **街道實景地圖（Leaflet.js + 免費國土測繪/OSM）**：支援全台實景導航。當放大至縣市（Zoom ≥ 10）時，自動標記全台各大 Livehouse、展演場館與大學校園真實座標，並附帶一鍵 Google Maps 導航連結。

### 5. 📅 多維度時程檢視模式
- **預告列表（Upcoming）**：卡片式緊湊排版，演出日期黑塊、時間、時長、備註與購票連結一覽無遺。
- **月曆模式（FullCalendar 整合）**：以月份全觀掌握全台檔期；點選日期直接彈出「單日現場清單浮動視窗（Day Events Modal）」，附帶膠囊快速跳轉錨點。
- **歷史場次與歌單庫（Setlist Archive）**：完整收錄過去場次的演出名單與曲目歌單（Setlist），支援即時展開與折疊。

### 6. ☁️ 雲端帳號無縫同步（Google Apps Script 後端）
- **極簡登入機制**：無需複雜註冊或密碼，輸入專屬自訂 ID 與暱稱即可登入。
- **全自動跨裝置同步**：已標記的「參戰足跡」、自創的「自訂藝人分組」與「關注清單」自動即時同步至雲端，換手機或電腦打開立即載入。
- **離線韌性與本地備份**：具備本機快取（Offline Cache），斷網依然可看排程；同時支援標準 JSON 檔案匯出與還原。

### 7. ⏱️ 現場足跡與聽團時數分析
- 點擊卡片左側的「＋足跡」即可標記親臨現場。
- 專屬分析面板自動換算**已參戰累積總場次**、**累積聽團總時數（精確至各團演出分鐘數）**以及個人專屬的**參戰樂團排行**。

---

## 🛠️ 技術架構

| 領域 | 使用技術 |
| :--- | :--- |
| **前端架構** | HTML5, Vanilla JavaScript (ES6+), Modern CSS (Variables / Flexbox / Grid) |
| **設計風格** | Neo-Brutalism (新野獸派), 響應式佈局 (Mobile Responsive) |
| **地圖視覺** | 內建手繪向量 SVG 台灣島嶼地圖 + [Leaflet.js](https://leafletjs.com/) (國土測繪中心 / OSM 圖資) |
| **日曆套件** | [FullCalendar 5](https://fullcalendar.io/) (客製化深色主題與單日浮層視窗) |
| **後端 / 雲端同步** | Google Apps Script (GAS) Web App + Google Sheets 雲端資料庫 |
| **資料來源** | `data.json` 靜態快取 + GAS 即時同步 API |
| **部署發佈** | GitHub Pages |

---

## 📂 專案檔案結構

```bash
├── index.html          # 主頁面：整合所有介面、雙軌篩選、地圖、日曆與足跡邏輯
├── admin.html          # 管理者後台：演出資料管理與維護介面
├── Code.gs             # Google Apps Script 雲端同步後端腳本（處理 GET/POST API）
├── appsscript.json     # Apps Script 專案設定檔
├── data.json           # 樂團清單、預告活動與歷史演出資料庫快取
├── 聽團網.xlsx         # 本地演出資料工作表記錄
└── README.md           # 專案說明文件
```

---

## 🚀 本地開發與預覽

本專案採原生純前端架構，無須複雜建置流程，亦可搭配任何本機靜態伺服器運行：

1. **Clone 專案庫**：
   ```bash
   git clone https://github.com/blues32767/gig-tracker.git
   cd gig-tracker
   ```

2. **啟動本機伺服器（以 VS Code Live Server 或 Python 為例）**：
   ```bash
   # 使用 Python 內建伺服器
   python -m http.server 8000
   ```
   瀏覽器開啟 `http://localhost:8000/index.html` 即可預覽。

---

## 👨‍💻 開發者與社群連結

歡迎聽團仔交流、反饋現場活動資訊或提出功能建議：

- **GitHub**：[@blues32767](https://github.com/blues32767)
- **Threads**：[@blues_.g](https://www.threads.com/@blues_.g)
- **Instagram**：[@blues_.g](https://www.instagram.com/blues_.g/)

---

## 💡 免責聲明

本網站為個人獨立開發之音樂愛好者非營利資訊工具。所有演出時程、演出卡司、演出時間與票務資訊，請一律以各大樂團官方社群及售票主辦單位最終公告為準。
