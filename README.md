# n8n-stocks-tracker-gsheets
Using a n8n workflow, tracking stocks prices in real time on Google Sheets


# 📈 Yahoo Finance Stocks Tracker for n8n

Fetches real-time prices for **5 stocks** from **Yahoo Finance** and stores them in **Google Sheets** using n8n.

## 🎯 What it tracks

- **MC.PA** (Eurofins)  
- **GOOGL** (Alphabet)  
- **PATH** (UiPath)  
- **RGTI** (Rigetti Computing)  
- **RKLB** (Rocket Lab)  

**Data extracted**: Price, % change, volume, timestamp.

## 🚀 Quick Setup

1. **Import** `yahoo-stocks-5tickers-sheets.json` into n8n
2. **Configure** Google Sheets credentials  
3. **Enable** Schedule Trigger (every X minutes)
4. **Test** → 5 rows added to your sheet

## 🔧 Required nodes
✅ Google Sheets (OAuth2)
✅ Schedule Trigger (Cron)
✅ 5x HTTP Request (Yahoo Finance API)
✅ 1x Code JS (merge data)
✅ 1x Google Sheets (Append)
