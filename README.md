# Alpaca Trading Course - Tutorial 4

## Place Market Order Script

This tutorial demonstrates how to place a MARKET order to buy or sell a stock using the Alpaca Trading API.

### Prerequisites

1. **Completed Tutorial 2**: You must have a working `config.py` file with your API keys
2. **Paper Trading Account**: Use your Alpaca Paper Trading Account to test this script. Running it on a Live Account will execute a real trade with real money.

### Project Structure

```
alpaca_bot_project/
├── config.py              # API credentials (NOT in version control)
├── place_order.py         # Main script for placing orders
├── requirements.txt       # Python dependencies
├── README.md              # This file
└── instructions.md        # Detailed tutorial instructions
```

### Setup

1. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

2. **Configure API Keys**
   - Copy `config.py` and add your Alpaca API credentials
   - Get your API keys from: https://app.alpaca.markets/paper/dashboard/overview
   - **IMPORTANT**: Never commit `config.py` to version control

3. **Run the Script**
   ```bash
   python place_order.py
   ```

### What This Script Does

1. **Checks Market Status**: Verifies that the market is open before attempting to place an order
2. **Places Market Order**: Executes a buy or sell order at the current market price
3. **Displays Confirmation**: Shows order details including Order ID, Symbol, Quantity, and Status

### Order Parameters

- **Symbol**: Stock to trade (default: "AAPL")
- **Quantity**: Number of shares (default: 1)
- **Side**: 'buy' to purchase, 'sell' to sell
- **Type**: 'market' - executes immediately at best available price
- **Time in Force**: 'day' - order valid until end of trading day

### Important Notes

- ⚠️ **Paper Trading**: This script uses the paper trading environment by default
- ⚠️ **Market Hours**: Orders can only be placed when the market is open
- ⚠️ **Error Handling**: All API calls are wrapped in try/except blocks for reliability

### Learning Objectives

- Understanding market orders
- Checking market status before trading
- Placing orders through the Alpaca API
- Handling order confirmations and errors

### Next Steps

After completing this tutorial, you can:
- Modify the script to trade different stocks
- Experiment with different order types
- Add more sophisticated error handling
- Implement order status tracking
