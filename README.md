<p align="center"><img src="assets/logo.png" width="96" alt="TraderWAI"></p>

# TraderWAI Charts for Gemini CLI

Live trading charts, exact market data and strategy backtests inside Gemini CLI, from [TraderWAI](https://traderwai.com).

![Gemini draws its analysis on a live gold chart](assets/ai-draws-on-your-chart.png)

- **Charts:** candlestick images for 40 symbols (major and cross forex pairs, gold, silver, oil, natural gas, stock indices, index and energy futures, Bitcoin and Ethereum), from 1 minute to monthly.
- **Marked charts:** Gemini draws its analysis on a real chart: support and resistance, zones, trend lines, entry, stop and targets.
- **Exact data:** OHLC candles and the latest price, so the levels in the analysis are precise.
- **Backtests:** describe a rule in plain language (range breakouts, moving average or level crosses, fair value gap retests, liquidity sweeps, time windows) and get every trade, the win rate, the total result in R and the drawdown.

TraderWAI Charts is **read-only**: it does not connect to brokerage accounts, cannot place or manage orders and never moves money.

## Install

```bash
gemini extensions install https://github.com/leonardo-mazzitelli/traderwai-charts
```

Then start Gemini CLI and sign in once with your TraderWAI account (free to create):

```
/mcp auth traderwai-charts
```

## Try it

- `Show me the gold chart on H4 and mark the key levels`
- `Analyze EUR/USD on the daily and hourly charts`
- `Backtest buying the London open range breakout on GBP/USD M15 over the last 7 days`

## Tools

| Tool | What it does |
|---|---|
| `get_chart` | Candlestick chart image for a symbol and timeframe |
| `draw_chart` | Chart image with the analysis drawn on it |
| `get_ohlc` | Exact OHLC candles |
| `get_quote` | Latest price |
| `backtest_strategy` | Backtest of a rule-based strategy on historical data |
| `list_symbols` / `list_timeframes` | Available markets and timeframes |
| `get_upgrade_url` | Plan page link when a daily limit is reached |

Viewing charts and data is unlimited on every plan. Marked charts and backtests have daily limits on the free plan. See [plans](https://traderwai.com/en/pricing).

## Links

- Documentation: https://traderwai.com/en/docs
- Status: https://traderwai.com/en/status
- Privacy: https://traderwai.com/en/privacy · Terms: https://traderwai.com/en/terms
- Support: info@traderwai.com

Analyses and backtests are educational and are not investment advice. Past results do not guarantee future results.

© FLEXIN AGILE LTD. Documentation licensed under CC BY 4.0.
