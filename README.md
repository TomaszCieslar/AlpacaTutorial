# Alpaca Trading Course - Tutorial 7: Simple Moving Average (SMA)

This tutorial demonstrates how to calculate Simple Moving Average (SMA) technical indicators using pandas and Alpaca API.

## Prerequisites

- Completed Tutorial 3 (fetching historical data)
- Python 3.7+
- Alpaca paper trading account

## Setup

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Create `config.py` file with your Alpaca API credentials:
```python
API_KEY = "your_api_key_here"
SECRET_KEY = "your_secret_key_here"
BASE_URL = "https://paper-api.alpaca.markets"
```

## Usage

Run the script:
```bash
python calculate_sma.py
```

The script will:
- Fetch 100 days of historical data for AAPL
- Calculate 20-day and 50-day Simple Moving Averages
- Display the results with price data and SMA values

## What is SMA?

Simple Moving Average is the average price over a specific number of periods. It helps:
- Smooth out short-term price fluctuations
- Identify underlying trends
- Generate trading signals (when used in crossover strategies)

## Security Note

⚠️ **Never commit `config.py` to version control!** It contains sensitive API credentials.

