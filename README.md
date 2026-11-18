# InstaService MCP

InstaService is a home-services marketplace in the United States. This repo holds the assistant
plugins that connect to it, plus a generic config for any other MCP client.

## Packages

- [`claude-plugin/`](claude-plugin/) — the Claude plugin. Connects to
  `https://www.api.instaservice.com/mcp/claude`.
- [`chatgpt-plugin/`](chatgpt-plugin/) — the ChatGPT app. Connects to
  `https://www.api.instaservice.com/mcp/chatgpt`.

Each folder has its own README with setup steps and the full list of things you can ask.

## Other MCP clients

Any other MCP client — Cursor, Windsurf, Claude Desktop's manual setup, and so on — can use
InstaService too. Copy the `mcpServers` block from [`mcp.json`](mcp.json) into your client's own
MCP config.

## What both plugins do

- Check whether InstaService serves a ZIP code.
- Price a cleaning, handyman or plumbing job, and show open arrival windows.
- Send a quote request to local Pros, then compare and answer their quotes.
- Show your bookings, recurring cleanings and quote requests.
- Cancel a booking or a recurring cleaning, when cancelling costs nothing.

Booking and payment always happen on [instaservice.com](https://www.instaservice.com). Neither
plugin takes a payment in the chat.

## License

MIT. See [LICENSE](LICENSE).
