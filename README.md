# Alpaca Trading Course - Tutorial Series

This repository contains a series of tutorials for learning algorithmic trading with the Alpaca API.

## 📚 Tutorials

- **[Alpaca02](Alpaca02/)** - "Hello, Alpaca!" - Connect & Check Your Account Status
  - Learn how to connect to the Alpaca API and retrieve basic account information

- **[Alpaca04](Alpaca04/)** - Place Market Order
  - Learn how to place a MARKET order to buy or sell a stock
  - Files: `place_order.py`, `instructions.md`

- **[Alpaca05](Alpaca05/)** - What Happened to My Order? – Checking Status & Positions
  - Learn how to check the status of your submitted orders and view your current open positions
  - Files: `check_status.py`, `instructions.md`

- **[Alpaca06](Alpaca06/)** - Anatomy of a Bot – The Main Loop
  - Learn about the most critical component of any automated bot: the main loop
  - Build a simple, infinite loop that serves as the bot's "heartbeat"
  - Files: `main_loop_bot.py`, `instructions.md`

- **[Alpaca07](Alpaca07/)** - Calculating Your First Indicator – Simple Moving Average (SMA)
  - Learn how to calculate one of the most fundamental technical indicators, the Simple Moving Average (SMA)
  - Calculate 20-day and 50-day SMAs using pandas on market data
  - Files: `calculate_sma.py`, `instructions.md`

## 🚀 Getting Started

Each tutorial is in its own folder. Navigate to the tutorial folder you want to follow and check the `README.md` file in that folder for specific instructions.

### Prerequisites

- Python 3.8 or higher (Python 3.10+ recommended)
- An Alpaca Paper Trading Account
- Alpaca API Keys (Paper Trading)
- pandas library (for Tutorial 7)

### General Setup

1. Navigate to the tutorial folder (e.g., `Alpaca02`, `Alpaca04`, `Alpaca05`, `Alpaca06`, or `Alpaca07`)
2. Install dependencies: `pip install -r requirements.txt`
3. Configure your API keys in `config.py` (create from template if needed)
4. Run the tutorial script

## 📁 Repository Structure

```
AlpacaTutorial/
│
├── Alpaca02/              # Tutorial 2: Hello Alpaca
│   ├── hello_alpaca.py   # Main script
│   ├── README.md         # Tutorial-specific documentation
│   ├── requirements.txt  # Python dependencies
│   └── ...
│
├── Alpaca04/              # Tutorial 4: Place Market Order
│   ├── place_order.py    # Main script
│   ├── README.md         # Tutorial-specific documentation
│   ├── requirements.txt  # Python dependencies
│   ├── instructions.md   # Detailed tutorial instructions
│   └── ...
│
├── Alpaca05/              # Tutorial 5: Check Order Status & Positions
│   ├── check_status.py   # Main script
│   ├── README.md         # Tutorial-specific documentation
│   ├── requirements.txt  # Python dependencies
│   ├── instructions.md   # Detailed tutorial instructions
│   └── ...
│
├── Alpaca06/              # Tutorial 6: Anatomy of a Bot - The Main Loop
│   ├── main_loop_bot.py  # Main script
│   ├── README.md         # Tutorial-specific documentation
│   ├── requirements.txt  # Python dependencies
│   ├── instructions.md   # Detailed tutorial instructions
│   └── ...
│
├── Alpaca07/              # Tutorial 7: Simple Moving Average (SMA)
│   ├── calculate_sma.py  # Main script
│   ├── README.md         # Tutorial-specific documentation
│   ├── requirements.txt  # Python dependencies
│   ├── instructions.md   # Detailed tutorial instructions
│   └── ...
│
└── README.md             # This file
```

## 🔒 Security

- **Never commit `config.py`** - It contains your API keys
- Each tutorial folder has its own `.gitignore` to protect sensitive files
- Always use Paper Trading keys for tutorials

## 📝 License

This tutorial series is part of an educational course on algorithmic trading with Alpaca.
