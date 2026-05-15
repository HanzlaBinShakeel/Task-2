# Task 2: Predict Future Stock Prices (Short-Term)

## Objective
Predict the next day's closing price using historical OHLCV data.

## Dataset
**Apple (AAPL)** from Yahoo Finance via `yfinance` (2022–2025).

## Models Applied
| Model | Role |
|-------|------|
| Linear Regression | Baseline interpretable model |
| Random Forest Regressor | Non-linear ensemble |

**Features:** Open, High, Low, Volume → **Target:** next day Close

## Key Results
- Time-based train/test split (80/20) preserves temporal order
- Both models achieve strong R² on test period; Random Forest often lower MAE
- Actual vs predicted plots show tracking of price trends

## Files
| File | Description |
|------|-------------|
| `stock_price_prediction.ipynb` | Full pipeline notebook |

## Run
```bash
jupyter notebook stock_price_prediction.ipynb
```
