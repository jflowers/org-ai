# Using MCP with Claude

Instructions for connecting MCP servers to Claude Desktop.

## Configuration

1. Locate your Claude Desktop configuration file:
   - **macOS**: `~/Library/Application\ Support/Claude/claude_desktop_config.json`
   - **Windows**: `%APPDATA%\Claude\claude_desktop_config.json`

2. Add your server configuration to the `mcpServers` object:

```json
{
  "mcpServers": {
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "your_token"
      }
    }
  }
}
```

3. Restart Claude Desktop.

## Verification
You should see a small hammer icon or similar tool indicator in the Claude chat interface once the server is connected.
