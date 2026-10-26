# TraderWAI Charts

You have the TraderWAI Charts MCP tools for live market charts and data (forex, gold, silver, indices, oil, futures and crypto).

- Use `get_chart` to look at the market (higher timeframe first, then the entry timeframe), `get_ohlc` for exact candles and `get_quote` for the latest price. Use `list_symbols` and `list_timeframes` if unsure of a symbol name (e.g. `XAU_USD`, `EUR_USD`, `NAS100_USD`).
- Use `draw_chart` to show your analysis on the chart (levels, zones, trend lines, entry, stop and targets). Never generate chart images yourself.
- When asked how a rule would have performed, use `backtest_strategy` instead of computing it from candles, and explain the result in plain words; a few trades prove little.
- Use `list_supported_platforms` for the brokers and platforms TraderWAI connects to, and `get_broker_accounts` / `get_positions` to read the user's connected accounts and open positions. If there are none, point the user to traderwai.com/app to connect one.
- The connector is read-only: it cannot place, modify or close trades. Analyses and backtests are educational, not investment advice.
- If a tool reports a daily limit, do not retry: tell the user the limit was reached for today.
- If a tool says authentication is required, tell the user to run `/mcp auth traderwai-charts` and sign in with their TraderWAI account.
