# Movie-Showtimes-Finder
基於Selenium和Tkinter的台灣威秀影城電影場次查詢工具

## 專案概述
這是一個自動化查詢威秀影城電影場次的工具，使用Selenium進行網頁爬蟲，並提供Tkinter圖形用戶界面。用戶可以選擇日期和影院，系統會自動抓取並顯示當日所有放映場次信息，大幅提高查詢效率。

## 功能特點
- 🎬 支持全台25家威秀影城查詢
- 📅 自定義日期選擇功能
- 🔍 實時獲取最新放映場次
- 💾 數據緩存功能，提高查詢效率
- 🖥️ 直觀易用的圖形界面

## 技術堆疊
- Python
- Selenium (網頁爬蟲)
- Beautiful Soup (HTML解析)
- Tkinter & ttk (GUI界面)
- tkcalendar (日期選擇組件)
- Chrome WebDriver (無頭瀏覽器)

## 安裝與使用
1. 克隆此倉庫
```bash
git clone https://github.com/您的用戶名/Movie-Showtimes-Finder.git
```

2. 安裝依賴包
```bash
pip install selenium beautifulsoup4 tkinter tkcalendar
```

3. 下載Chrome WebDriver
- 前往 https://sites.google.com/chromium.org/driver/
- 下載與您Chrome瀏覽器版本匹配的WebDriver
- 確保WebDriver在系統PATH中或指定完整路徑

4. 運行應用程序
```bash
python 電影查詢器_程式設計概論.py
```

## 使用說明
1. 從日期選擇器中選擇您想查詢的日期
2. 從下拉菜單選擇威秀影城分店
3. 點擊「提交」按鈕
4. 查看結果列表中顯示的電影場次信息

![使用演示](/api/placeholder/600/400)

## 系統架構
```
使用者界面（Tkinter）→ 爬蟲引擎（Selenium）→ 數據處理（BeautifulSoup）→ 結果展示
```

## 技術細節
- 使用Selenium模擬瀏覽器操作，解決動態加載內容問題
- 實現緩存機制減少重複請求，提高響應速度
- 無頭模式（Headless）運行瀏覽器，減少資源佔用
- 精確日期格式轉換，匹配威秀網站查詢要求

## 數據使用聲明
- 本工具僅用於個人學習和研究目的
- 爬取的數據僅限於公開的電影場次信息
- 請尊重威秀影城的使用條款和robots.txt規定
- 不應用於商業目的或高頻次的自動化查詢

## 開發筆記
- 處理AJAX動態加載的內容是主要技術挑戰
- 使用WebDriverWait確保頁面元素完全加載
- 使用異常處理機制提高程序穩定性
- 緩存系統大幅提升重複查詢效率

## 未來改進計劃
- [ ] 添加電影詳細信息查詢
- [ ] 實現電影類型和評分過濾
- [ ] 優化UI界面設計
- [ ] 添加自動購票連結
- [ ] 支持更多電影院線

## 授權
本專案採用MIT授權 - 詳見LICENSE檔案
