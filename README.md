# Trader Behavior vs Market Sentiment Analysis

## Project Overview
This project analyzes how **trader behavior** changes under different **market sentiment conditions (Fear vs Greed)**.

Using historical trading data and the Bitcoin Fear & Greed Index, the analysis focuses on understanding:
- Profitability changes
- Trading volume behavior
- Buy/Sell activity during Fear and Greed periods

The goal is to identify sentiment-driven patterns that help explain trader decision-making.

---

## Datasets Used

### 1. Historical Trader Data
This dataset contains trade-level information including:
- Account
- Coin
- Execution Price
- Trade Size (USD)
- Buy/Sell Side
- Timestamp (IST)
- Closed Profit and Loss (PnL)

### 2. Bitcoin Fear & Greed Index
This dataset provides daily market sentiment information with:
- Date
- Sentiment classification (Fear / Greed)

---

## Data Preprocessing
The following preprocessing steps were performed:
- Converted timestamp columns into datetime format.
- Extracted date from trade timestamps.
- Aligned trader data with sentiment data using the date field.
- Merged both datasets based on the date column.
- Verified data consistency after merging.

---

## Sentiment-Based Analysis Performed

### Profitability Analysis
- Compared average **Closed PnL** during Fear and Greed periods.
- Observed higher average PnL during Greed phases.

### Trading Volume Analysis
- Analyzed average trade size (USD) under different sentiment conditions.
- Found that traders generally take larger positions during Greed periods.

### Trade Side Behavior
- Studied Buy vs Sell distribution across Fear and Greed phases.
- Observed noticeable differences in trade behavior based on sentiment.

---

## Visualizations Generated
- Average PnL vs Market Sentiment
- Average Trade Size (USD) vs Market Sentiment
- Buy/Sell distribution across Fear and Greed
- PnL distribution by sentiment

All visual outputs are stored in the `outputs/` folder.

---

## Project Structure

ds_akhil/
├── notebook_1.ipynb # Data loading, cleaning, merging, and analysis
├── outputs/ # Saved charts and plots
├── ds_report.pdf # Final summarized insights
└── README.md # Project documentation

---

## Tools Used
- Python
- Pandas
- Matplotlib
- Google Colab

---

## Dataset Access
Due to GitHub file size limitations, the datasets are not uploaded directly to this repository.

The datasets are accessed through Google Drive and loaded within Google Colab notebooks. All notebooks are shared with access set to **"Anyone with the link can view"**.

---

## Conclusion
The analysis shows that market sentiment has a clear impact on trader behavior.  
Greed periods are associated with higher trade sizes and increased profitability, while Fear periods reflect more cautious trading behavior.

This highlights the importance of considering market sentiment when analyzing trading behavior.
