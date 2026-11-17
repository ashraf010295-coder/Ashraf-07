QUOTEX SIGNAL PRO — DEMO-ONLY PWA

WHAT THIS IS
A lightweight installable web app for strict technical setup screening. It displays UP, DOWN, or NO TRADE. It does not connect to Quotex, execute trades, or fetch live prices. You must supply completed OHLC candles from a data source matching the instrument/timeframe.

IMPORTANT
- The built-in demo candles are simulated, not real market data.
- The score is a setup-quality checklist score, NOT a statistical win probability.
- OTC prices are proprietary/platform-specific; ordinary forex feeds cannot verify Quotex OTC candles.
- This is educational software, not financial advice. Never use real money based on an unvalidated signal.

INSTALL ON WINDOWS + ANDROID
This is a Progressive Web App (PWA). PWA installation requires HTTPS hosting (localhost also works for testing).
1. Upload the contents of this folder to a static HTTPS host such as GitHub Pages or Netlify.
2. Open the hosted HTTPS address in Chrome or Edge.
3. Windows: click the install icon in the address bar, or browser menu > Install app.
4. Android: open in Chrome > menu (⋮) > Install app / Add to Home screen.
5. Once installed, it can open as an app and the interface shell works offline.

LOCAL TEST
You can open index.html directly to test the interface, but install-as-app/offline PWA features require HTTPS hosting.

CSV FORMAT
At least 60 completed candles, oldest first:
time,open,high,low,close
2026-11-17 10:00,1.1600,1.1610,1.1595,1.1608

STRICT RULE
UP only when EMA 9 > EMA 21 > EMA 50 and price above EMA 9, RSI 52–68 and MACD histogram positive, volatility filter passes, and latest candle is strongly bullish.
DOWN uses the inverse conditions (RSI 32–48).
Otherwise NO TRADE.
These are heuristic filters and require out-of-sample testing before any reliance.
