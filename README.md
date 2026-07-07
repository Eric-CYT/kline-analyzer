# ▣ 加密貨幣 K線量化分析系統

純前端無依賴的加密貨幣 K 線型態分析工具，支援 **Binance / Bybit / OKX** 三大交易所即時資料。

🚀 **[線上使用](https://YOUR_USERNAME.github.io/kline-analyzer/)**（部署後替換連結）

---

## 功能特色

| 功能 | 說明 |
|------|------|
| 📊 K線圖表 | 自繪 SVG K線，疊加 BB、MA200、MA50、POC |
| 📈 技術指標 | MACD(12,26,9)、RSI(14)、成交量分析 |
| 🎯 形態識別 | 自動偵測 6 種強勢型態 |
| 📋 回測引擎 | 歷史訊號回測，計算勝率、風報比、平均損益 |
| 🔍 任意搜尋 | 支援 50+ 常見幣種 + 任意 USDT 交易對 |
| ⚡ 零依賴 | 純 HTML/CSS/JS，無需安裝任何工具 |

### 支援形態
- 🔨 強力錘子線（下影線 + RSI超賣 + 布林下軌 + MA200支撐）
- 🟢 看漲吞噬（吞噬 + MACD柱轉正 + 成交量）
- 📈 MACD 黃金交叉（金叉 + RSI動能 + MA200多頭）
- 🚀 布林上軌突破（突破 + 成交量放大確認）
- 🔄 RSI 超賣反彈（RSI回升 + MA200支撐 + 布林彈升）
- 🏛️ 三白兵（連續三根陽線 + 量能 + 未超買）

---

## 架設到 GitHub Pages（5分鐘完成）

### 方法一：直接上傳（推薦新手）

1. 登入 [GitHub](https://github.com) → 點右上角 **+** → **New repository**
2. Repository name 填 `kline-analyzer`，選 **Public**，點 **Create repository**
3. 點 **uploading an existing file** → 把 `index.html` 和 `.nojekyll` 拖進去 → **Commit changes**
4. 進入 **Settings** → 左側 **Pages** → Source 選 **Deploy from a branch** → Branch 選 `main` → **Save**
5. 等約 2 分鐘，網址 `https://<你的帳號>.github.io/kline-analyzer/` 即上線 🎉

### 方法二：Git 指令

```bash
git clone https://github.com/YOUR_USERNAME/kline-analyzer.git
cd kline-analyzer
# 複製 index.html 和 .nojekyll 進此資料夾
git add .
git commit -m "feat: 加密貨幣K線分析系統"
git push origin main
```

---

## 本機執行

直接雙擊 `index.html` 開啟即可。

若遇到 CORS 問題（部分瀏覽器在 `file://` 下限制跨域）：

```bash
# Python 3
python -m http.server 8080

# Node.js
npx serve .
```

開啟 → http://localhost:8080

---

## 搜尋使用說明

- **快速幣種**：點選 BTC / ETH / SOL 等 12 個常用按鈕
- **搜尋框**：輸入任意幣種代號（如 `PEPE`、`WIF`、`ORDI`），按 Enter 或 GO
- **鍵盤快捷鍵**：按 `/` 快速聚焦搜尋框，`↑↓` 選擇建議，`Esc` 關閉
- **最近搜尋**：點擊搜尋框會顯示最近查詢記錄

---

## 免責聲明

本工具僅供學習研究使用，不構成任何投資建議。  
加密貨幣交易具有高度風險，請自行評估並承擔相應責任。
