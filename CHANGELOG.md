# 珍北平電子名片（nfc-card）CHANGELOG

## 2026-06-15 — v2：編輯雜誌風打掉重練 + 餡餅 Lottie

### 改了什麼
- **結構重構**：從「linktree 按鈕牆」改成「**一螢即名片 + 往下翻故事**」。第一螢直接給核心三動作（加LINE / 撥電話 / 找最近的店），往下才是雜誌式故事。
- **視覺**：冷海軍藍 emoji 版 → **暖色牛皮紙編輯風**（拉珍北平 Design System 色票：招牌紅 #D7261D、墨褐 #2E2017、牛皮紙 #F4ECDB、金 #C77B1E、宋體大標 Noto Serif TC）。
- **大正方形頭照**（取代小圓角框，氣場拉滿、浮水印裁掉）。
- **餡餅 Lottie 招牌動畫**（`xianbing.json`，手寫向量 5.5KB、lottie-web 載入，slot 已 bake 成內聯色 + 透明底）。
- **大數字塊**：35 年 / 10 間分店 + 「2025 入選《台灣 500 碗》小吃名店」獎項徽章（先前誤植成「500 碗/日」已修）。
- **全幅爆餡特寫**（`xianbing-closeup.jpg`）配宋體文案。
- **菜單修正**：`menu-03-flatbread`↔`menu-04-butter` 檔名標反，改標籤對到正確的圖（03=奶油、04=山東大餅），大餅裁切往上露出餅本體。
- **emoji 全換 SVG 線條圖示**（LINE/FB/IG/Email/電話/地圖/媒體）。
- **補大埔店**（原本只列 9 家、漏第 10 家）。

### 給未來 Claude 該知道
- 部署：GitHub Pages，`main` 分支 path `/`，push main 自動 build（~1-2 分）。網址 https://weifu0716.github.io/nfc-card/
- 用到的素材檔：`avatar.jpg`、`menu-01~06`、`xianbing.json`、`xianbing-closeup.jpg`。`storefront.jpg`（夜景門市）一度當背景，後因含**八方雲集競品招牌**+ 改走亮版而移除——門面素材要逐張掃競品。
- Lottie 改動見 [[reference_text_to_lottie_animation_library]]：嵌 lottie-web 前要 bake 掉 Skia 專屬 slot。
- 大埔店導航目前是 Google Maps 搜尋暫代，待換正式連結。
- 舊版保留：`index.backup.html`、`index.舊版備份-20260615.html`（git 歷史也有）。

## 2026-03-24 — v1：初版（GitHub Pages，深色 emoji linktree）
詳見 `部署筆記.md`。
