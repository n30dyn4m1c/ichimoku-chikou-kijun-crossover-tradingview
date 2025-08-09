# 🌥️📈 Ichimoku Chikou-Kijun Cross Alert (TradingView)

A lightweight TradingView Pine Script indicator that detects Chikou Span (Lagging Line) crossovers against the historical Kijun-sen line. Designed for traders who want precise, closed-bar alerts of potential momentum shifts without repainting.

---

## 🧰 Tech Stack

- **Platform**: TradingView  
- **Language**: Pine Script v6  
- **Alert System**: `alertcondition()` + optional `alert()` popups  
- **Signal Logic**: Ichimoku Chikou × historical Kijun crossover  
- **Symbol Coverage**: Any TradingView chart  
- **Timeframes**: All TradingView-supported timeframes (M1–M)  

---

## 🚀 Key Features

- ✅ Detects Chikou Span crossovers over the *historical* Kijun (lenKijun bars back)  
- ✅ Bullish and Bearish crossover alerts  
- ✅ Optional Ichimoku cloud & line plots for context  
- ✅ Optional debug table showing calculation values  
- ✅ Epsilon filter to avoid false signals on flat Kijun lines  
- 🔒 Closed-bar confirmation to avoid repainting  

---

## 📊 Signal Logic

This indicator checks for Ichimoku crossovers using historical alignment:  

### 🔼 Bullish Signal
- Chikou Span closes **above** Kijun-sen on the same historical bar it is plotted against.

### 🔽 Bearish Signal
- Chikou Span closes **below** Kijun-sen on the same historical bar it is plotted against.

Signals only trigger once the bar closes.

---

## 🗂 Included Files

| File                                                | Description                                          |
|----------------------------------------------------|------------------------------------------------------|
| `ichimoku-chikou-kijun-crossover.pine`           | Main TradingView Pine v6 indicator with alert logic  |

---

## 🛠️ Setup Instructions

1. Open TradingView  
2. Go to **Pine Editor**  
3. Paste `ichimoku-chikou-kijun-cross-alert.pine`  
4. Click **Add to chart**  
5. Adjust Tenkan/Kijun/Senkou lengths if needed  
6. Enable alerts:  
   - `Right-click → Add Alert`  
   - Choose Bullish/Bearish condition from the dropdown  
7. (Optional) Enable `useAlerts` to get immediate popups  

---

## ⏰ When to Use

- Intraday and swing trading for momentum shifts  
- Works well with XAUUSD, US30, NAS100, BTCUSD, and volatile FX pairs  
- Can be used as a confirmation filter in multi-indicator strategies  

---

## 📸 Screenshot

To be added.

---

## 🎓 Lessons Learned

- Historical Chikou-Kijun crossovers give cleaner signals than same-bar comparisons.  
- Avoid taking trades when Chikou is obstructed by price action or the Kumo cloud.  
- Epsilon filtering reduces noise on flat Kijun.  
- Use higher timeframe bias for lower timeframe entries.  
- Closed-bar confirmation is key to avoiding repainting.

---

## 🎯 Future Improvements

- 🧠 Add Kumo breakout filter for higher probability signals  
- 📩 Add webhook/push notification templates  
- 🎯 Option to mark past crossovers on chart history  
- 🗃️ Export signal history for backtesting  
- 📊 Multi-timeframe dashboard of Chikou-Kijun status  

---

## 📝 License & Acknowledgments

- © 2025 **Neo Malesa** – [@n30dyn4m1c on X](https://www.x.com/n30dyn4m1c)  
- Made for Ichimoku traders seeking precision in TradingView  
- Inspired by classic Ichimoku theory and adapted for Pine Script v6  
