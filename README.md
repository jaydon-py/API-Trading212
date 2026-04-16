# Trading 212 API Explorer

A set of Python scripts for pulling data from the Trading 212 Public API (Live environment) into clean DataFrames and CSV exports.

---

## Files

```
api_syntax.py        # Experimenting with some basic syntax
endpoint_dfs.py      # Dumps all major API endpoints to CSV files
keys_config.py       # API credentials (not committed)
```

---


## API credentials

Create a `keys_config.py` file in the project root:

```python
api_key    = "your_api_key"
secret_key = "your_secret_key"
```

DO NOT COMMIT THIS FILE. It should not be public. Save it locally.

Your API key is generated in the Trading 212 app under **Settings → API (Beta)**. 
Note: This project targets the **Live** environment only.
Another Note: Trading 212 only shows the secret key once, when it is initially generated with your API key.

---

## Endpoints Explored

Hits six API endpoints and saves each as a CSV:

| File | Endpoint |
|---|---|
| `positions.csv` | Current open positions |
| `account_summary.csv` | Account summary |
| `orders.csv` | Active orders |
| `historical_orders.csv` | Full order history |
| `historical_transactions.csv` | Deposits, withdrawals, dividends |
| `instruments.csv` | Tradeable instrument metadata |
