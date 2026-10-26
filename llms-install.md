# Installing TraderWAI Charts

TraderWAI Charts is a hosted remote MCP server. There is nothing to clone, build or run.

1. Add this to the MCP settings (Streamable HTTP):

```json
{
  "mcpServers": {
    "traderwai-charts": {
      "url": "https://mcp.traderwai.com/charts/v2",
      "type": "streamableHttp"
    }
  }
}
```

2. On first use the client opens the TraderWAI sign-in page in the browser (OAuth 2.1 with dynamic client registration). The user signs in with Google; a free account is created if needed. No API key.
3. Test it: ask "Show me the gold chart on H4 and mark the key levels".

The server is read-only: charts, OHLC data, quotes, backtests and a view of the user's connected broker accounts and positions. It cannot place, modify or close trades.
