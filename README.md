# DATASET_ANALYSIS(BINANCE)

## Overview
This project analyzes historical trading data from Binance accounts over a 90-day period to evaluate performance metrics and rank trading portfolios. It processes trade history data, calculates key financial metrics, and generates comprehensive reports and visualizations.

## Features
- Processes trade history from multiple portfolios
- Calculates key financial metrics:
  - ROI (Return on Investment)
  - PnL (Profit and Loss)
  - Sharpe Ratio
  - Maximum Drawdown (MDD)
  - Win Rate
  - Position Analysis
- Generates detailed performance reports
- Creates visualizations for performance analysis
- Ranks portfolios based on combined performance metrics
- Identifies top 20 performing portfolios

## Requirements
- python
- pandas
- numpy
- matplotlib
- seaborn

## Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/binance-trading-analyzer.git
cd binance-trading-analyzer
```

2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn
```

## Usage
1. Prepare your data:
   - Ensure your trade history data is in CSV format
   - Required columns:
     - Port_IDs: Unique portfolio identifiers
     - Trade_History: JSON-formatted trade details

2. Run the analysis:
```bash
python trading_analyzer.py
```

3. Check the output files:
   - `trading_analysis_report.txt`: Detailed analysis report
   - `top_20_portfolios.csv`: Top performing portfolios data
   - `portfolio_analysis.png`: Visualization of key metrics

## Input Data Format
The input CSV file should contain:
- Port_IDs: Unique identifiers for trading accounts
- Trade_History: JSON string containing:
  - timestamp
  - asset
  - side (BUY/SELL)
  - positionSide
  - price
  - quantity
  - realizedProfit

## Output
1. Analysis Report:
   - Overall portfolio statistics
   - Performance metrics
   - Top 20 performing portfolios

2. Visualizations:
   - ROI vs Win Rate scatter plot
   - PnL Distribution
   - Sharpe Ratio vs MDD comparison
   - Win Rates by Portfolio

3. CSV Export:
   - Detailed metrics for top 20 portfolios
   - Complete performance data

## Metrics Calculated
- **ROI (Return on Investment)**: Percentage return on invested capital
- **PnL (Profit and Loss)**: Total realized profit/loss
- **Sharpe Ratio**: Risk-adjusted return metric
- **Maximum Drawdown (MDD)**: Largest peak-to-trough decline
- **Win Rate**: Percentage of profitable trades
- **Position Analysis**: Breakdown of trading positions

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments
- Thanks to Binance for providing the trading data structure
- Inspired by quantitative trading analysis techniques