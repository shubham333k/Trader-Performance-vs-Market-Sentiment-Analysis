**Trader Performance vs Market Sentiment Analysis**

Project Overview-
This project analyzes how Bitcoin market sentiment (Fear vs Greed) influences trader behavior and performance on Hyperliquid.

The objective is to uncover statistically supported patterns linking sentiment regimes to trader profitability, behavioral intensity, and risk characteristics — and to derive actionable trading insights.

This submission fulfills the requirements of the Data Science / Analytics Intern Round-0 Assignment.

Assignment Objectives Covered
✔ Data cleaning and correct timestamp alignment
✔ Creation of required performance metrics
✔ Sentiment-based performance comparison
✔ Behavioral analysis across regimes
✔ Trader segmentation (2+ segments)
✔ Statistical validation
✔ At least 3 data-backed insights
✔ 2 actionable strategy recommendations
✔ Clean, reproducible notebook structure

Datasets Used-
1️⃣ Bitcoin Market Sentiment Dataset
Dat
Classification (Fear / Greed)
2️⃣ Hyperliquid Historical Trader Dataset
Includes:
Account
Execution Price
Size (USD & Tokens)
Direction (Long / Short)
Timestamp
Closed PnL
Transaction metadata

Methodology-
1️⃣ Data Preparation
Converted timestamps to datetime format
Aggregated trade-level data to daily level
Merged trader data with daily sentiment classification
Verified missing values and duplicates

2️⃣ Feature Engineering
Constructed trader-daily metrics:
Daily PnL
Total trades per day
Win rate
Average trade size
Total traded volume
Long/short ratio
Profitability indicator

3️⃣ Sentiment-Based Performance Analysis
Compared Fear vs Greed performance
Analyzed distribution differences
Evaluated trade frequency and position sizing
Conducted Welch’s t-test for statistical validation

4️⃣ Trader Segmentation
Segmented traders into:
High vs Low Activity
Consistent vs Inconsistent (based on win rate)
Analyzed how each segment behaves under different sentiment regimes.

Key Insights-
1️⃣ Greed regimes support profitability expansion
Average daily PnL and trading activity are higher during Greed periods.
2️⃣ Fear regimes increase downside dispersion
Loss volatility and performance variability widen during Fear environments.
3️⃣ High-activity traders are sentiment-sensitive
Aggressive trading strategies amplify both upside and downside exposure.
4️⃣ Consistent traders show regime resilience
High win-rate traders maintain more stable performance across sentiment shifts.

Strategy Recommendations-
Strategy 1 — Sentiment-Aware Risk Scaling
Reduce exposure and trade frequency during Fear regimes
Expand controlled participation during Greed regimes

Strategy 2 — Segment-Based Capital Allocation
Allocate greater capital weight to consistent traders
Limit exposure of inconsistent traders during Fear periods
These rules improve downside containment while maintaining upside participation.

Statistical Validation-
Welch’s t-test was conducted to evaluate whether performance differences between Fear and Greed periods are statistically significant.
This ensures conclusions are evidence-driven rather than visual-only observations.

Project Structure-
Trader-Sentiment-Analysis/
│
├── data/
│   ├── sentiment.csv
│   ├── trader_data.csv
│
├── analysis.ipynb
├── README.md
└── requirements.txt
▶️ How to Run

Clone the repository
Install dependencies:
pip install pandas numpy matplotlib seaborn scipy
Place datasets inside the data/ folder
Open analysis.ipynb
Run all cells sequentially

Conclusion-
Market sentiment acts as a structural regime variable influencing trader profitability and behavioral intensity.
Incorporating sentiment-aware exposure management and segment-based allocation improves capital efficiency and downside protection.

Author: Shubham
Role Applied: Data Science / Analytics Intern
Submission Type: GitHub Repository
