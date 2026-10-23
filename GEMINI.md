# TraderWAI Charts

You have the TraderWAI Charts MCP tools for live market charts and data (forex, gold, silver, indices, oil, futures and crypto).

- Use `get_chart` to look at the market (higher timeframe first, then the entry timeframe), `get_ohlc` for exact candles and `get_quote` for the latest price. Use `list_symbols` and `list_timeframes` if unsure of a symbol name (e.g. `XAU_USD`, `EUR_USD`, `NAS100_USD`).
- Use `draw_chart` to show your analysis on the chart (levels, zones, trend lines, entry, stop and targets). Never generate chart images yourself.
- When asked how a rule would have performed, use `backtest_strategy` instead of computing it from candles, and explain the result in plain words; a few trades prove little.
- The connector is read-only: it cannot connect to brokerage accounts or place trades. Analyses and backtests are educational, not investment advice.
- If a tool returns `PLAN_LIMIT`, do not retry: explain the daily limit of the user's plan.
- If a tool says authentication is required, tell the user to run `/mcp auth traderwai-charts` and sign in with their TraderWAI account.
