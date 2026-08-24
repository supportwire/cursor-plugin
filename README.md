# SupportWire

Cursor plugin for the [SupportWire](https://supportwire.com) inbox, via the official remote MCP server.

Search conversations, reply in-thread, and pull customer or teammate context.

## Install

1. Open **Cursor Settings → Plugins**.
2. Search for **SupportWire**.
3. Click **Install**, then complete the SupportWire sign-in prompt.

Or run `/add-plugin supportwire` in chat.

## MCP

```json
{
  "mcpServers": {
    "supportwire": {
      "type": "http",
      "url": "https://mcp.supportwire.ai/mcp"
    }
  }
}
```

Auth is OAuth 2.0 (DCR + PKCE). Cursor registers itself and prompts for SupportWire sign-in. No API key.

Tool calls run as the signed-in user and cannot exceed that user's permissions.

## Docs

- Product: https://supportwire.com
- MCP: https://mcp.supportwire.ai/mcp

## License

MIT
