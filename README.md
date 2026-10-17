# TradeMind AI — Mobile Crypto Lab

A mobile-first static web app/PWA. It can be deployed entirely from a phone using GitHub Pages.

## Features
- Public Binance spot candles
- RSI, EMA 20/50, MACD and a basic volume comparison
- Simplified EMA crossover + RSI long-only historical backtest
- Return, buy-and-hold comparison, win rate, max drawdown, trade count and profit factor
- Position-size/risk calculator
- Optional public crypto news feed (may be blocked/unavailable in some browsers)

## Phone-only deployment with GitHub Pages
1. Extract this ZIP on your phone (Files app or an archive app).
2. In Chrome, sign in to GitHub and create a **public** repository named `trademind-mobile`.
3. Open the repository, choose **Add file → Upload files**, and upload `index.html`, `manifest.json`, `sw.js`, and `README.md` from the extracted folder. Commit the upload.
4. In the repository, open **Settings → Pages**.
5. Under Build and deployment, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
6. Wait a few minutes. The Pages screen will show the website URL. Open it in Chrome.
7. In Chrome's menu (⋮), choose **Add to Home screen** or **Install app** if offered.

If GitHub's mobile interface hides an option, enable **Desktop site** in Chrome. Do not share passwords, API keys, or account credentials.

## Limitations and safety
- No login, exchange connection, order execution, or trading API keys.
- Uses public Binance spot candle data; endpoint availability can vary by region/network.
- News retrieval is best-effort and may fail because of network or browser restrictions.
- Backtest is a simplified demonstration, not a validated trading system. It omits spread, slippage, market impact, funding, liquidation, and realistic intrabar execution; it should not be used to claim a real probability of profit.
- It is long-only, uses a simple EMA crossover with RSI filter, and does not use leverage.
- A service worker caches the app shell; live market data still requires internet.
