# Alpaca Trading Course - Complete Tutorial Series

A complete educational course on algorithmic trading using the Alpaca API. The course consists of 30 lessons that guide you from the basics (generating API keys) to advanced strategies (statistical arbitrage, pairs trading).

## Course Overview

The course is divided into several thematic sections that systematically build knowledge and skills in algorithmic trading:

### Section 1: Fundamentals (Lessons 1-5)
**Fundamentals - Setup and First Steps**

- **Lesson 1: Generating API Keys in Alpaca** - Creating an Alpaca account and generating API keys for paper trading
- **Lesson 2: "Hello, Alpaca!" - Connect & Check Your Account Status** - First connection to the Alpaca API and account verification
- **Lesson 3: Fetching Market Data – Your First Candlestick** - Fetching historical OHLCV data (Open, High, Low, Close, Volume)
- **Lesson 4: Place Market Order** - Placing your first buy/sell order
- **Lesson 5: What Happened to My Order? – Checking Status & Positions** - Checking order status and positions

### Section 2: Building a Bot (Lessons 6-10)
**Bot structure and basic strategies**

- **Lesson 6: Anatomy of a Bot - The Main Loop** - Creating the main bot loop for continuous operation
- **Lesson 7: Simple Moving Average (SMA)** - Calculating moving averages for technical analysis
- **Lesson 8: Moving Average Crossover Detector** - Detecting moving average crossovers (Golden Cross / Death Cross)
- **Lesson 9: Simple Exit Logic – Selling on a Reversal Signal** - Implementing exit logic for positions
- **Lesson 10: Moving Average Crossover Strategy - Complete Bot** - A complete, working trading bot

### Section 3: Risk Management (Lessons 11-15)
**Capital protection and position management**

- **Lesson 11: Bracket Orders - Stop-Loss & Take-Profit** - Automatic capital protection using bracket orders
- **Lesson 12: Take Your Profits! – Setting a Take-Profit Order** - Automatically securing profits
- **Lesson 13: Never Risk Too Much – Calculating Position Size** - Dynamic position size calculation (the foundation of professional risk management)
- **Lesson 14: Trailing Stop-Loss Bot** - Trailing stop-loss that protects profits as price moves in a favorable direction
- **Lesson 15: Implementing a Trailing Stop-Loss in Code** - Advanced implementation of trailing stop-loss from scratch

### Section 4: Advanced Indicators (Lessons 16-20)
**Technical analysis and advanced strategies**

- **Lesson 16: Relative Strength – Building an RSI-Based Bot** - Bot based on the RSI (Relative Strength Index) indicator for mean-reversion trading
- **Lesson 17: The Magic of Volatility – A Bollinger Bands® Bot** - "Squeeze breakout" strategy using Bollinger Bands
- **Lesson 18: The Power of Momentum – Implementing a MACD Strategy** - Bot using MACD (Moving Average Convergence Divergence) to detect momentum changes
- **Lesson 19: Signal Confirmation – Combining Two Indicators** - Combining multiple indicators for signal confirmation
- **Lesson 20: The Bigger Picture – Analyzing Multiple Timeframes** - Multi-timeframe analysis - a technique used by professional traders

### Section 5: Production and Professionalism (Lessons 21-25)
**Preparing the bot for production**

- **Lesson 21: The Bot's "Black Box" – Logging Every Decision to a File** - Comprehensive logging of all trading decisions
- **Lesson 22: Stop Digging in the Code – Using an External Config File** - Separating configuration from code (professional practice)
- **Lesson 23: What If the Bot Restarts? – Managing Position State** - Position state management - a bot with memory that survives restarts
- **Lesson 24: Stay Updated – Sending Real-Time Notifications to Discord** - Real-time notifications via Discord
- **Lesson 25: Making Your Bot Resilient – Handling API and Connection Errors** - Error handling and creating a resilient bot ready for production

### Section 6: Testing and Optimization (Lessons 26-28)
**Strategy validation and real-time data**

- **Lesson 26: Time Travel – The Basics of Backtesting Your Strategy** - Basics of backtesting strategies on historical data
- **Lesson 27: Understanding Your Results – Analyzing a Backtest Report** - Analyzing backtest results like a professional (Annual Return, Max Drawdown, Sharpe Ratio)
- **Lesson 28: Faster Than HTTP – Streaming Real-Time Data with WebSockets** - Transitioning from polling to WebSockets for real-time data

### Section 7: Deployment and Advanced Strategies (Lessons 29-30)
**Deployment and professional strategies**

- **Lesson 29: Your Bot Online 24/7 – Deploying to a VPS Server** - Deploying the bot to a VPS server for 24/7 operation
- **Lesson 30: A Step Towards PRO – Statistical Arbitrage (Pairs Trading)** - Advanced market-neutral strategy: pairs trading using cointegration

## Course Goals

After completing the course, you will be able to:

- Configure a development environment and connect to the Alpaca API
- Fetch and analyze market data (OHLCV)
- Build complete, working trading bots
- Implement various trading strategies (trend-following, mean-reversion, momentum)
- Manage risk professionally (position sizing, stop-loss, take-profit)
- Use advanced technical indicators (SMA, RSI, MACD, Bollinger Bands)
- Combine multiple indicators and timeframes for better signals
- Create resilient bots ready for production (error handling, logging, state management)
- Test strategies on historical data (backtesting)
- Deploy bots to VPS servers for 24/7 operation
- Implement advanced strategies (pairs trading, statistical arbitrage)

## Requirements

### Basic Requirements

- **Python 3.8+** (Python 3.10+ recommended)
- **Alpaca Paper Trading Account** - [Sign up here](https://alpaca.markets/)
- **Basic Python knowledge** - variables, functions, loops, lists
- **Basic Git knowledge** (optional, for code management)

### Required Python Libraries

Each lesson contains a `requirements.txt` file with required dependencies. Main libraries used in the course:

- `alpaca-py` / `alpaca-trade-api` - Official Alpaca SDK
- `pandas` - Data manipulation
- `numpy` - Numerical computations
- `pandas-ta` - Technical indicators
- `statsmodels` - Statistical analysis (for pairs trading)
- `backtesting` - Strategy backtesting
- `requests` - HTTP requests (for Discord webhooks)

## Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/TomaszCieslar/AlpacaTutorial.git
cd AlpacaTutorial
```

### 2. Start with Lesson 1

```bash
cd Alpaca01
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API Keys

```bash
# Copy the example configuration file
cp config.example.py config.py

# Edit config.py and add your Alpaca API keys
# WARNING: NEVER commit config.py to Git!
```

### 5. Run Example Code

```bash
# For lesson 2:
python hello_alpaca.py

# For lesson 3:
python fetch_data.py

# For lesson 4:
python place_order.py

# etc...
```

## Project Structure

```
AlpacaTutorial/
├── Alpaca01/              # Lesson 1: Generating API keys
├── Alpaca02/              # Lesson 2: API connection
├── Alpaca03/              # Lesson 3: Fetching market data
├── Alpaca04/              # Lesson 4: Placing orders
├── Alpaca05/              # Lesson 5: Checking status
├── Alpaca06/              # Lesson 6: Main bot loop
├── Alpaca07/              # Lesson 7: Calculating SMA
├── Alpaca08/              # Lesson 8: Crossover detection
├── Alpaca09/              # Lesson 9: Exit logic
├── Alpaca10/              # Lesson 10: Complete bot
├── Alpaca11/              # Lesson 11: Bracket orders
├── Alpaca12/              # Lesson 12: Take-profit
├── Alpaca13/              # Lesson 13: Position sizing
├── Alpaca14/              # Lesson 14: Trailing stop
├── Alpaca15/              # Lesson 15: Manual trailing stop
├── Alpaca16/              # Lesson 16: RSI bot
├── Alpaca17/              # Lesson 17: Bollinger Bands
├── Alpaca18/              # Lesson 18: MACD strategy
├── Alpaca19/              # Lesson 19: Signal confirmation
├── Alpaca20/              # Lesson 20: Multi-timeframe
├── Alpaca21/              # Lesson 21: Logging
├── Alpaca22/              # Lesson 22: External config
├── Alpaca23/              # Lesson 23: State management
├── Alpaca24/              # Lesson 24: Discord notifications
├── Alpaca25/              # Lesson 25: Error handling
├── Alpaca26/              # Lesson 26: Backtesting
├── Alpaca27/              # Lesson 27: Backtest analysis
├── Alpaca28/              # Lesson 28: WebSockets
├── Alpaca29/              # Lesson 29: VPS deployment
├── Alpaca30/              # Lesson 30: Pairs trading
├── Instructions/          # Detailed instructions for each lesson
├── README.md              # This file
└── templateReadmy.md      # Template for lesson documentation
```

## Course Philosophy

### Clarity Over Cleverness

The course prioritizes **clarity over cleverness**:

- **Full, descriptive variable names** - `take_profit_price` instead of `tp`
- **Comments explain "WHY"** - not just "WHAT"
- **One line = one action** - we avoid complex, nested expressions
- **Each function does one thing** - Single Responsibility Principle
- **No "magic"** - we prefer verbal and explicit code

### Educational Code Principles

- **Education before optimization** - code is readable, not necessarily fastest
- **Explicit over implicit** - everything is clearly written
- **Error handling** - all API calls in try/except blocks
- **Paper Trading First** - always start with safe testing

## Security

### Critical Rules

1. **NEVER commit API keys!**
   - The `config.py` file is in `.gitignore`
   - Use `config.example.py` as a template
   - Never share keys publicly

2. **Always use Paper Trading during learning**
   - By default, all examples use `https://paper-api.alpaca.markets`
   - Test strategies without financial risk
   - Switch to live trading only after thorough testing

3. **Protect your API keys**
   - Treat them like passwords
   - Rotate keys if you suspect compromise
   - Use separate keys for paper and live trading

## Recommended Learning Path

### For Beginners

1. **Start with Lessons 1-5** - Basics of setup and first operations
2. **Go through Lessons 6-10** - Building your first working bot
3. **Focus on Lessons 11-15** - Risk management is crucial
4. **Experiment** - Modify parameters, test different symbols
5. **Always use Paper Trading** - Don't risk real money while learning

### For Advanced Users

- **Lessons 16-20** - Advanced indicators and strategies
- **Lessons 21-25** - Production preparation
- **Lessons 26-28** - Testing and optimization
- **Lessons 29-30** - Deployment and advanced strategies

## Key Concepts Taught in the Course

### Trading Basics

- **Market Orders** - Basic buy/sell orders
- **OHLCV Data** - Candlestick data (Open, High, Low, Close, Volume)
- **Position Management** - Managing positions
- **Order Status** - Tracking order status

### Technical Analysis

- **Simple Moving Average (SMA)** - Moving averages
- **Relative Strength Index (RSI)** - Relative strength indicator
- **MACD** - Moving Average Convergence Divergence
- **Bollinger Bands** - Bollinger Bands for volatility measurement
- **Crossover Signals** - Crossover signals (Golden Cross, Death Cross)

### Risk Management

- **Position Sizing** - Dynamic position size calculation
- **Stop-Loss Orders** - Automatic protection against losses
- **Take-Profit Orders** - Automatic profit securing
- **Bracket Orders** - Combination of entry, stop-loss and take-profit
- **Trailing Stops** - Stop-loss that follows price

### Advanced Techniques

- **Multi-Timeframe Analysis** - Multi-timeframe analysis
- **Signal Confirmation** - Confirming signals with multiple indicators
- **Mean-Reversion Trading** - Mean-reversion strategies
- **Trend-Following** - Trend-following strategies
- **Pairs Trading** - Statistical arbitrage (market-neutral)

### Production and Deployment

- **Error Handling** - Error handling and bot resilience
- **Logging** - Comprehensive decision logging
- **State Management** - Position state management
- **External Configuration** - Separating configuration from code
- **Discord Notifications** - Real-time notifications
- **VPS Deployment** - Deployment to a server for 24/7 operation
- **Backtesting** - Testing strategies on historical data
- **WebSockets** - Streaming real-time data

## Important Warnings

### This is Education Only

- **This is not financial advice** - The course is for educational purposes only
- **Paper Trading Only** - Use only a test account while learning
- **Risk** - Trading in markets involves the risk of capital loss
- **Test thoroughly** - Before thinking about real trading, test everything in paper trading

### Safety Rules

- **Never trade with money you cannot afford to lose**
- **Always test in paper trading before live trading**
- **Understand the strategy before implementing**
- **Monitor your strategies regularly**
- **Use proper security practices**
- **Back up your configuration**

## Additional Resources

### Alpaca Documentation

- [Alpaca API Documentation](https://alpaca.markets/docs/)
- [Alpaca Python SDK](https://github.com/alpacahq/alpaca-trade-api-python)
- [Alpaca Market Data API](https://alpaca.markets/docs/api-documentation/market-data-api/)

### Support

- [Alpaca Support Center](https://alpaca.markets/support)
- [Alpaca Status Page](https://status.alpaca.markets/)
- [GitHub Issues](https://github.com/TomaszCieslar/AlpacaTutorial/issues) - Report problems and questions

## Contributing to the Project

Educational project open to:

- Reporting issues
- Suggestions for improvements
- Sharing educational experiences
- Pull requests with fixes

## License

MIT License - Free use for educational purposes

## Summary

This course guides you from zero to an advanced level in algorithmic trading. After completing all 30 lessons, you will have:

- A complete, resilient trading bot running 24/7
- Knowledge of many trading strategies (directional and market-neutral)
- Risk management and position sizing skills
- Ability to backtest strategies
- Ability to deploy a bot to a VPS server
- Advanced statistical arbitrage strategies

**"Risk comes from not knowing what you're doing." - Warren Buffett**

Start with Lesson 1 and build your knowledge step by step. Remember: always test in paper trading and never risk more than you can afford to lose.

---

**Happy Trading!**

*Alpaca Trading Course - Complete Tutorial Series*  
*30 lessons from basics to advanced strategies*
