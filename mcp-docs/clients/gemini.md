# Using MCP with Gemini

Instructions for connecting MCP servers to Gemini-based tools (e.g., Gemini Advanced, AI Studio).

## Configuration

### Via Google AI Studio
1. Open [Google AI Studio](https://aistudio.google.com/).
2. Look for the "Tools" or "MCP" section in the settings/sidebar.
3. Add a new server by providing the command (e.g., `npx -y @modelcontextprotocol/server-github`).

### Via Local Settings
If using a local environment that supports Gemini:
```json
{
  "mcpServers": {
    "github": {
      "httpUrl": "https://api.githubcopilot.com/mcp/",
      "headers": {
        "Authorization": "Bearer your_token_here"
      }
    },
    "chrome-devtools": {
      "command": "npx",
      "args": [
        "chrome-devtools-mcp@latest",
        "--browser-url=http://127.0.0.1:9222"
      ]
    }
  }
}
```
