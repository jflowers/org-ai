# Chrome MCP Server

Instructions for setting up the Chrome MCP server for browser interaction.

## Prerequisites

1. **Chrome Browser**: Installed and running.
2. **Remote Debugging**: Chrome must be started with remote debugging enabled.

## Configuration

### Windows
```cmd
"C:\Program Files\Google\Chrome\Application\chrome.exe" --remote-debugging-port=9222
```

### macOS
```bash
/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --remote-debugging-port=9222
```

### Running the Server
```bash
npx -y @modelcontextprotocol/server-chrome
```
