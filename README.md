# TradeMind AI — Advanced Mobile Crypto Lab v4

## What's new
- Mobile-first dark interface and clearer explanations.
- Dynamic directory of active Binance spot pairs quoted in USDT (loaded from the public exchange-info API; fallback list if unavailable).
- Embedded TradingView chart synchronized to selected Binance symbol and selected timeframe. TradingView's symbol search can be used to inspect other supported markets/exchanges.
- Structure + ATR-based illustrative stop reference and selectable R-multiple targets.
- Risk calculator with account size from 0 to 1,000 USDT, adjustable risk %, long/short planning, stop method, and 1R/1.5R/2R/3R targets.
- Educational concept matching inspired by well-known public frameworks: trend following (Jesse Livermore/classic trend principles), Turtle-style breakouts, Wyckoff market structure, Dow Theory, mean reversion and momentum confirmation.
- Concept matches are heuristic rule alignment, not backtested claims of profitability or exact reproductions of anyone's complete strategy.

## Deploy from a phone
1. Extract this ZIP.
2. In the `Dakshff21/Trademind` GitHub repository, replace `index.html`, `manifest.json`, `sw.js`, and `README.md` in the repository root with these files.
3. Commit the changes and wait for GitHub Pages to redeploy.
4. Open https://dakshff21.github.io/Trademind/ and refresh. If an older build remains, clear the site cache or unregister its service worker.

## Important limitations
This is a static educational research page, not a trained AI model, financial adviser, or execution platform. Binance's public API provides spot candle data; the symbol list is active Binance USDT spot pairs, not literally every token on every exchange. TradingView availability and chart data may differ from Binance. The rules do not have calibrated win probabilities. Stops can slip, and results do not include all fees, spread, funding, liquidation or market impact. No derivatives, order-book or comprehensive fundamentals engine is included. Verify everything independently and do not use leverage based only on these signals.


## v5 update
- Added 5-minute candle timeframe to Binance candle retrieval and TradingView chart interval.
- Added a separate Smart Money Concepts chart with heuristic swing highs/lows, potential BOS, fair-value gaps, and a simple order-block candidate.
- SMC markings are approximations from OHLC candles, not institutional order-flow data or a validated strategy.
