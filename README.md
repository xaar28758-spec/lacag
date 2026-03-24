# Meme Coin Launch Analyzer

A conservative, risk-aware analyzer for early-stage meme coin launches on Solana (via DexScreener).

## Setup

1. **Install Dependencies**
   Ensure you are in the project directory:
   ```bash
   pip install -r requirements.txt
   ```

2. **Configuration**
   Edit `config.py` to adjust:
   - `SEARCH_QUERY`: The chain or term to scan (default: "solana")
   - `MAX_PAIR_AGE_MINUTES`: How 'fresh' the pairs must be.
   - `MIN_LIQUIDITY_USD`: Minimum liquidity to consider.

## Usage (Live Scraper)

The bot now uses **Playwright** to scrape `dexscreener.com/new-pairs` directly.

Run the scanner:
```bash
python main.py
```

### Configuration
In `config.py`, you can toggle `HEADLESS = False` if you want to watch the browser window (good for debugging).


