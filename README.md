# Alpaca Trading Course - Tutorial Series

This repository contains a series of tutorials for learning algorithmic trading with the Alpaca API.

## 📚 Tutorials

- **[Alpaca02](Alpaca02/)** - "Hello, Alpaca!" - Connect & Check Your Account Status
  - Learn how to connect to the Alpaca API and retrieve basic account information

## 🚀 Getting Started

Each tutorial is in its own folder. Navigate to the tutorial folder you want to follow and check the `README.md` file in that folder for specific instructions.

### Prerequisites

- Python 3.8 or higher (Python 3.10+ recommended)
- An Alpaca Paper Trading Account
- Alpaca API Keys (Paper Trading)

### General Setup

1. Navigate to the tutorial folder (e.g., `Alpaca02`)
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
└── README.md             # This file
```

## 🔒 Security

- **Never commit `config.py`** - It contains your API keys
- Each tutorial folder has its own `.gitignore` to protect sensitive files
- Always use Paper Trading keys for tutorials

## 📝 License

This tutorial series is part of an educational course on algorithmic trading with Alpaca.
