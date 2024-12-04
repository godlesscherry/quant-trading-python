# Quantitative Trading with Python

This project is a hands-on guide for learning quantitative trading using Python. It provides tools and scripts for data analysis, strategy development, backtesting, and visualization.

## Project Structure
```
quant_trading_python/
│
├── data/                # Store raw and processed datasets
├── notebooks/           # Jupyter Notebooks for analysis
├── src/                 # Core Python scripts
│   ├── data_fetcher.py  # Scripts to fetch and process data
│   ├── strategies.py    # Implementation of trading strategies
│   ├── backtest.py      # Backtesting engine
│   ├── utils.py         # Utility functions
│
├── tests/               # Unit tests for the project
├── requirements.txt     # Dependency file
├── README.md            # Project documentation
└── .gitignore           # Git ignore file
```

## Features
- Fetch historical stock data
- Implement trading strategies (e.g., Moving Average Crossover)
- Backtest strategies
- Visualize performance

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
    ```
2. Create and activate a virtual environment:
```bash     
python3 -m venv quant_env
source quant_env/bin/activate
```
3. Install dependencies:
```bash 
pip install -r requirements.txt
```
Run scripts or explore the notebooks.

#Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

#License
This project is licensed under the MIT License.