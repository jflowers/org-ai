# Chrome DevTools MCP Server

Instructions for setting up the Chrome DevTools MCP server for browser interaction and debugging.

## Prerequisites

1. **Chrome Browser**: Installed and running.
2. **Remote Debugging**: Chrome must be started with remote debugging enabled on port 9222.

### Starting Chrome with Remote Debugging

#### macOS
```bash
/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --remote-debugging-port=9222
```

#### Linux (Fedora/CentOS-Stream/RHEL)
```bash
google-chrome --remote-debugging-port=9222
```

## Configuration

To configure the Chrome DevTools MCP server in your client settings (e.g., Gemini, Claude):

```json
"chrome-devtools": {
  "command": "npx",
  "args": [
    "chrome-devtools-mcp@latest",
    "--browser-url=http://127.0.0.1:9222"
  ]
}
```

## Features
- Inspect page content
- Run JavaScript in the browser
- Take screenshots
- Navigate to URLs
