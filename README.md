# Python_Kite_PnL
📈 KITE_PNL – Intraday Trading PnL & Charges Analysis
📌 Project Overview

This project analyzes intraday equity trades (MIS orders) executed by a trader using data exported from the Kite trading platform. The objective is to calculate transaction-level charges, stock-wise summaries, and overall Profit & Loss (PnL) by applying NSE intraday brokerage and statutory charges as defined by Zerodha.

The solution processes raw trade data and generates a multi-sheet Excel summary for clear financial and performance analysis 

Kite PnL Problem Statment

.

🎯 Objectives

Analyze intraday (MIS) equity trades only

Exclude Rejected orders and handle Cancelled / Partially executed orders correctly

Calculate turnover, brokerage, taxes, and statutory charges per trade

Generate stock-wise and overall PnL summaries

Export results into a structured Excel workbook

📊 Input Data

The input dataset contains trade-level order information including:

Timestamp of trade execution

Buy / Sell type

Stock instrument

Product type (MIS / CNC)

Executed quantity

Average trade price

Order execution status (Completed, Cancelled, Rejected)

Only Completed and partially executed MIS trades are considered for calculations 

Kite PnL Problem Statment

.

⚙️ Methodology

Cleaned and filtered raw trade data to retain valid intraday (MIS) trades

Calculated trade turnover using executed quantity and average price

Applied NSE intraday charges including:

Brokerage

STT / CTT

Exchange Transaction Charges (ETC)

SEBI charges

GST

Stamp duty

Aggregated data to compute:

Trade-level charges

Stock-wise and Buy/Sell type-wise weighted average price and charges

Overall Gross PnL, Total Charges, Net PnL, and % Charges on Gross PnL

All charge calculations follow Zerodha Equity Intraday pricing rules (NSE) 

Kite PnL Problem Statment

.

📑 Outputs (Excel Workbook)

The final Excel file contains three sheets:

1️⃣ Individual Trade Charges
Detailed breakdown of turnover and all applicable charges per trade

2️⃣ Stock-wise & Type-wise Analysis
Weighted average price, total quantity, and aggregated charges by stock and Buy/Sell type

3️⃣ Overall Stock Summary
Gross PnL, total charges, net PnL, and percentage of charges on Gross PnL

🛠️ Tech Stack

Python (Pandas, NumPy), Excel, Financial Data Analysis

📁 Repository Structure
├── kite_pnl.ipynb
├── orders.csv
└── README.md

📌 Use Cases

Intraday trading performance analysis

Brokerage and tax impact assessment

Financial reconciliation and reporting

Data Analyst / Finance Analytics portfolio project

⚠️ Disclaimer

This project is created for analytical and educational purposes only and does not provide trading or investment advice.
