# 📉 Gap Down Recovery Trading Strategy – Python Backtest (5-Year Data)

This project simulates a simple **price-action-based trading strategy** on Indian stocks (e.g., TCS) using **5 years of historical stock data**.

It identifies buying opportunities based on a 3-step pattern and tracks the performance of each trade using Python, with output exported to Excel.

---

## 📌 Project Objective

To test a **gap down + recovery breakout** strategy on Indian stocks and evaluate the trade performance over the last 5 years using actual historical data.

---

## 🧠 Strategy Logic (Simplified)

1. A stock **gaps down by 2% or more** compared to the previous day's close.
2. It **recovers** to the previous close (on the same day or later).
3. It then **breaks out** by rising another 2% or more.
4. **Buy Trigger**: Enter trade at this 2% breakout price.
5. **Exit Conditions**:
   - 🎯 **Target**: Exit at +10% profit
   - 🛑 **Stop Loss**: Exit at -5% loss
   - ⏱️ **Max Hold**: Exit after 60 calendar days if no target or stop hit

---

## ✅ Output

The script generates a table with each simulated trade:

| Stock   | Entry Date | Entry Price | Exit Date | Exit Price | P&L (%) | Days Held | Outcome     |
|---------|------------|-------------|-----------|------------|---------|-----------|-------------|
| TCS.NS  | 2021-06-01 | ₹102.00     | 2021-06-10| ₹112.20    | +10.0%  | 9         | Target Hit  |

You can export this to Excel for analysis. (there is a .csv file that has 300 nifty data with same format)

---

## 📁 Files

- `nifty500.ipynb` – Python script to simulate the strategy
- `ind_nifty500list.xlsx` – Excel output with trades and results
- `Trading_Strategy_Explanation.pdf` – Simple explanation of strategy for non-technical users

---

## 🚀 How to Run

1. Open the notebook or script in **Google Colab** or **Jupyter Notebook**
2. Make sure required libraries (`yfinance`, `pandas`, `openpyxl`) are installed
3. Run the script
4. Check the output or download Excel results

---

## 🔧 Technologies Used

- Python
- yFinance (for historical stock data)
- pandas
- Excel output via `openpyxl`

---

## 📊 Future Enhancements

- Apply strategy to full Nifty 500 list
- Add RSI/MACD filter to refine entries
- Connect with Interactive Brokers for paper trading
- Streamlit dashboard for visualization

---

## 👨‍💻 Created By

Nikhil – Technical Analysis Intern at Paterson Securities  
📅 June 2025

---

## 📬 Contact

Want to collaborate or use this strategy on your data?  
Reach out on [LinkedIn](https://linkedin.com/analystnikhil) or email me.

